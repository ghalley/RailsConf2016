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
