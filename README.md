# ADR-template

Markdown template for Architecture Decision Records (ADRs).

### Usage guidelines 
 - Each ADR is a plain text, 1-2 page document
 - ADRs should be numbered
 - ADRs should be stored within each software project repo
 - Create a separate repo for crosscutting ADRs
 - Track ADRs in the backlog
 - Review ADRs
 - Create ADRs for *significant* design decisions
 - This template is a suggestion that you may want to adopt or adapt. In any case, establishing and sharing a template for ADRs in your team or organization is a good idea.

### Examples of ADRs using this template
 - [Use of the BFF pattern](https://github.com/miyagis-forests/farmacy-food-kata/blob/main/ADRs/ADR003-bff-pattern.md)
 - [Use CQRS](https://github.com/miyagis-forests/farmacy-food-kata/blob/main/ADRs/ADR005-cqrs-pattern.md)
 - [Use AWS as cloud provider](https://github.com/miyagis-forests/farmacy-food-kata/blob/main/ADRs/ADR006-aws-as-cloud-provider.md)
 - [Use Payment Gateway in self-hosted mode](https://github.com/miyagis-forests/farmacy-food-kata/blob/main/ADRs/ADR002-payment-gateway.md)
 - [Use the Wrapper pattern](https://github.com/miyagis-forests/farmacy-food-kata/blob/main/ADRs/ADR004-wrapper-pattern.md)

(These examples are project-specific, of course. The decision and rationale make sense in that project's context.) 
 
### References
This template is based on: 
 - [Documenting Architecture Decisions](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions). Blog post by Michael Nygard, 2011.
 - [Architecture Decision Records in Action](https://saturn2017.sched.com/event/9k2y/architecture-decision-records-in-action). SATURN 2017 presentation by Michael Keeling and Joe Runde.
 
See also this [post and conference presentation by Ken Power](https://kenpower.ie/2021/02/10/architecture-decision-records-being-agile-with-architecture-decisions/).  
 
### Why this template?
- This template addresses a subtle yet fundamental deficiency of the [ADR structure originally proposed by Michael Nygard]((http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions)):  
his proposed structure (Context; Decision; Status; Consequences) has no evident placeholder for the **rationale** 
behind the **design decision**. 
- The justification, the rationale, the "why" behind the design decision should stand out as a separate section in the
template for at least three reasons:
    - It is remarkably important! (Authors cited further below agree.)
    - A separate section reminds the author of the ADR that that information must be captured. 
    - The rationale section avoids cluttering other sections with rationale discussion. Devs may reference the ADRs several 
     times to re-read the decision and consequences. They need to read the rationale just once, so rationale should not 
     be mixed in the other sections.
- Mark Richards and Neal Ford say "Why is more important than how" is the *Second Law of Software Architecture* ([Fundamentals of Software Architecture](https://learning.oreilly.com/library/view/fundamentals-of-software/9781492043447/)).
- We say in our book "Record Rationale" is *Rule 5* of the *Seven Rules for Sound Documentation* ([Documenting Software Architectures, Second Edition](https://www.informit.com/store/documenting-software-architectures-views-and-beyond-9780321552686)).
- George Fairbanks proposed *[Architecture Haiku](https://www.slideshare.net/matthewmccullough/architecture-haiku)*, 
which can be seen as an alternative approach to ADR. Haiku contents includes "design rationales". 
