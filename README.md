# RailsConf 2016

## Stuck in the Middle: Leverage the power of Rack Middleware

http://www.whynot.io/ruby/what-is-rack-in-ruby/

Rack sets "environment" hash

3 parts:
- Handler takes care of WEBrick
- Adapter talks to framework
- Middlewares work with request/response as it passes through stack
    + used in rails to setup cookies, flash messages, logging, and params parsing

rack-throttle on github

Middleware can deal with requests your app should never worry about
- can be protective
- sees request and response
- easily extracted to shareable tool

Middlewares run in a certain order
`rake middleware`

Doesn't belong in middleware:
- modifying the request
- knows about business logic in the app
- knows about models in the app

Always return a response
@cdwort

## Internships: Good for the intern, Great for the team
@liliealbert

### The CS Hammer
recent CS grad, far too enthusiastic about doing things themself

### The Relative
"interested" in programming, happened in a vacuum

### The Cutting-edge cat
wanted to use the cool new stuff only

### A good one
very open to learning

### Lessons
1. The CS Hammer needs guidance.  Be involved in what they're learning and doing
2. The Relative needs a clear goal and purpose to the program
3. The Cutting-edge cat needed guidance on goals and purpose
4. The good one can teach your things about what you're doing

Internships are audits of your own process.

Structure Matters

Intern could also mean apprentice or junior dev

Make the business case

Have goals for the program

Omada internship
- Pairing for a few weeks
- SOlo project
- Back to pairing

Team Composition: 3 experience to 1 intern

Pairing
- fewer silos, more communication, onboarding is easier
- doing so across skill levels is hard
- let the intern type

Don't Pair?  A solo project is good, code reviews will be vital

#### Things you'll learn from the intern
You'll learn how confusing your code is
Some people are bad teachers

#### The solo project
Useful to solidify things they learn from pairing

#### Code Review
Useful in person most, but good over github
Code Review talk from RailsConf2015

#### Mentorship
good for someone interested in management
useful when scheduled, especially during solo project phase
    can interrupt

#### Diversity
Good for attracting good interns

#### Recruiting/Interviewing
Less strenuous, simple code challenges
Pairing interview

Retention is important!

tech.omadahealth.com

## Small Team Culture Shock
@sysadmin1138

Pschological Safety

Microaggressions make things harder
- incompetence
- willful ignorance

Safety Methods:
- Reflexive Change Resistance.  Raise concerns when not included in changes ahead of time.
- Intentional Deinvestment. Stop caring? Symptom of a very broken culture.
- Compartmentalization.  Sympathizing but not helping with others' problems
- Bonding through negativity. Share pain

1. Redirect - turn reflexive negativity into feedback
2. Reengage - Get them to feel like a person and provide feedback
3. Stop hurtful negativity - It doesn't help, put a stop to it.

## Storytelling with Code

Evoking feelings through stories

"Temping"

No actors
- email
- phone
- laser printer
- the built environment

### The story
- The audience is a temp
- Cast of characters (still not actors)

The temp needs tasks to do to drive the story.

Starts with an excel spreadsheet
- update alive/dead
- update life expectancies
    + tricked into looking at your own life expectancy

### The Narrative Arc
Ordering the events

### Characterization
Understanding why these people do things

### Empathy

### Imagination
Letting audience fill in the blanks

### Choices
giving the audience room to explore the way they want

Michaelrau.com

## Making a test framework from scratch

zenspider.com/presentations/2016-railsconf.html

github.com/zenspider/microtest

learnenough.com

## Keynote: Nickolaus Means
@nmeans

## Keynote: Chanelle Henry
@chenelle777
http://www.slideshare.net/Chanelle7/rails-conference-presentation-2016-ux-rails-and-awesomeness

## ActionCable

### ActionCable is NOT:
- for non-rails apps
- step forward for more rails js integration

### ActionCable IS:
- solid feature for rails monoliths
- a way to snapify rails, like turbolinks an js responses
- easy and fun

Chat apps are the hello world of websockets
- doesn't inherently add value to an app
- most apps don't need chat between users

#### Use Cases
1. Use Case: Collaboration
2. Asynchronous Tasks

### Modules
1. Cable - actual connection
2. Channel - what to listen for on the rails side
3. Broadcast - send info out from rails through channel
4. Subscription - client side listening and receiving data from server

Best to always use ActionJob to broadcast, to help avoid missed messages
no session, only cookies
github.com/jwo

## Secrets of Testing Rails 5 Apps
https://speakerdeck.com/chaitanya/secrets-of-testing-rails-5-apps

### Test Runner
`bin/rails test`

Much better documentation

Can run multiple specific tests!
- groups by folder, too

Backtrace option: `-b`

Stop at first failure: `-f`

Colored Output!
- active by default

Integration tests are much faster
- deprecating controller tests since there is no diff in speed anymore

Backward compatible tests!

Rails 5 discourages testing controller view interface space

## Rspec and Rails 5
@searls



