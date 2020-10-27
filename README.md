# ADR-template

Markdown template for Architecture Decision Records (ADRs).

### Usage guidelines 
 - Each ADR is a plain text, 1-2 page document
 - ADRs should be numbered
 - ADRs should be stored within each software project repo
 - Create a separate repo for crosscutting ADRs
 - This template is an example. You can adapt or create your own. But do establish and share a template for ADRs in your team or organization
 - Track ADRs in the backlog
 - Review ADRs
 - Create ADRs for *significant* design decisions

### References
This template is based on: 
 - [Documenting Architecture Decisions](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions). Blog post by Michael Nygard, 2011.
 - [Architecture Decision Records in Action](https://saturn2017.sched.com/event/9k2y/architecture-decision-records-in-action). SATURN 2017 presentation by Michael Keeling and Joe Runde.

### Why this template?
- This template addresses a subtle yet fundamental deficiency of the [ADR structure originally proposed by Michael Nygard]((http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions)):  
his proposed structure (Context; Decision; Status; Consequences) has no evident placeholder for the **rationale** 
behind the **design decision**. 
- Mark Richards and Neal Ford say "Why is more important than how" is the *Second Law of Software Architecture* ([Fundamentals of Software Architecture](https://learning.oreilly.com/library/view/fundamentals-of-software/9781492043447/)).
- We say in our book "Record Rationale" is *Rule 5* of the *Seven Rules for Sound Documentation* ([Documenting Software Architectures, Second Edition](https://www.informit.com/store/documenting-software-architectures-views-and-beyond-9780321552686)).
- The justification, the rationale, the "why" behind the design decision should stand out as a separate section in the
template for at least three reasons:
    - It is remarkably important!
    - A separate section reminds the author of the ADR that that information must be captured. 
    - The rationale section avoids cluttering other sections with rationale discussion. Devs may reference the ADRs several 
     times to re-read the decision and consequences. They need to read the rationale just once, so rationale should not 
     be mixed in the other sections.   
     
     