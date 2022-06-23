
# How to make your team fall in love with legacy code

Umberto Brabini  
@ramtop

https://leaddev.com/legacy-technical-debt-migrations/how-make-your-team-fall-love-legacy-code

* Greenfield : build sth new, take all decision => self esteem, authoriality
* Legacy : risky, boring, hard, career dead end

> "Legacy code" often differs from its suggested alternative by actually working and scaling.


1. Convey that **working on legacy is not a career dead end**. It's an important task and management will appreciate the effort required to rejuvenate the legacy project.
2.    Invest time in **improving the infrastructure and the onboarding process before starting developing** new features. Sometimes DevOps are more important than pure developers for making old projects easy to work with.
3.    Don't rely on policies alone to ensure quality and security. Make sure any relevant use case is covered by end-to-end automated tests that run at least before every release. Having a **continuous release process does wonders to increase the confidence of not breaking things**.
4.    Organize the development work with frequent mobbing sessions to **share knowledge and collectively discuss the new design**. Proof of concepts and explorations are best done solo in separate branches.
5.    Remember that **people are much more important than technical decisions**. Working effectively on legacy code starts with the culture of your team.


## Legacy code is enjoyable if

* Legacy means working in prod and critical (otherwise kill it & redo from scratch)
* Dev are allowed to change and rejuvenate it

## Team can love legacy code if

* Team & company culture empower devs to work on legacy code
  * Counteracting frustration ("I can't change this")
  * Counteracting fear ("I will create bugs")
 * using trust, support (teamwork, pair prog)
* Company values working on legacy code (it can be fun!). Exemples :
   * Most greenfield projects fails or can end up in dead marches when legacy projects works, have users and bring value.
   * Working on an tried and true codebase you've not written makes you learn and you have quick feedback if your change works or not.
  * All successful projet will become legacy. Learning to deal with legacy helps build better projects from scratch as well.

## Work effectively with legacy code as a team  

* team work, auto discipline, knowledge sharing, pair prog, test driven dev.
* test are important. Keep them fast & focus.
* break big ball o fmud monolith into smaller low coupled modules



