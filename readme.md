# [Chris Hough](https://links.aboutchrishough.com/)

Founder and engineering leader passionate about building high-impact products, empowering remote teams, and integrating AI to push the boundaries of what’s possible. I build with Ruby, architect APIs, and engineer intelligent systems that amplify creativity, clarity, and execution.

I lead with heart and operate with intention, engineering not just software, but environments where people grow and thrive. Whether I’m mentoring a team, shipping a product, or shaping new AI-driven workflows, I approach it all with craftsmanship and care.

My philosophy is simple: optimize everything, your codebase, your body, your mindset. From chasing a Half Ironman to rebuilding myself from the inside out, I live by the belief that our greatest work starts within. I’m obsessed with growth, driven by purpose, and fueled by the thrill of crafting things that resonate, endure, and matter.

The goal isn’t just to ship software, it’s to build experiences that make people feel, teams that perform with soul, and a life I never want to escape from.

Let’s craft something that outlives us together, and enjoy the thrill while we’re at it.

## EXPERIENCE

### Founder & Principal Product Engineer, RobotsBuildingRobots, LLC  
**Remote** : Illinois, Colorado, Oregon, New York, & Nevada   
2016 - `Present`  

*  **Serenity**: Commanding an agentic build system for a client-management SaaS platform serving a timeshare-relief and financial-recovery consulting firm: 20 instruction files, 2,926 lines, govern how AI writes the code. Built on Rails 8.1 and Ruby 4.0 with Solid Queue, Cache, and Cable running on PostgreSQL 17 instead of Redis, and a 63-table domain carved into 118 service objects. Claude Code runs recurring multi-agent security audits of the live app, five agents in parallel with runtime verification; MCP-driven Playwright suites test the app in a real browser; and AI-generated summaries ship in the product itself. More test code than application code, zero RuboCop violations, clean Brakeman, 600+ PRs in 7.5 months, still building.

*  **SOFware**: Engineered the qualification-tracking and scheduling capabilities U.S. Air Force Special Warfare units (JTAC, Combat Control, Special Tactics, TACP) rely on to manage operator training readiness under AFMAN 10-3500, serving as senior full-stack engineer across two Ruby on Rails applications and a shared gem, centered on an event-driven GraphQL domain. Built operator disenrollment end to end, from GraphQL API to dossier projections; designed a designation-scoped competency-construction API that applies JTAC requirements to individual operators; and led a CMMC security-hardening pass that protects CSV exports against spreadsheet formula injection.

*  **Arthur Maxwell**: Took an offline iPad-driven eLearning management and classroom application to the web for global enterprise clients, rebuilding it on Ruby on Rails with Hotwire (Turbo + Stimulus).

*  **SafeAccess**: Built the technical hiring pipeline and personally recruited the senior Ruby on Rails engineer who succeeded the co-founder and senior technical architect, securing continuity of innovation and application development.

*  **Sidebench**: Technical Architect for the Momints NFT Marketplace: drove the research and selection of scalable components, built the MVP, and produced the marketing materials. Authored the architecture package spanning system diagrams, server infrastructure, tech stack, third-party dependencies, data models, database schemas, and API specifications, giving the build team a straight line through development.

*  **Advanced Building Technology**: Led the rearchitecture of a website to a mobile-first responsive design in Ruby, cutting hosting costs, adding precise traffic measurement and monitoring, and sharpening the experience across mobile and tablet.

*  **Eggplant**: Integrated Microsoft Active Directory (LDAP) into the authorization layer of a test-management application on the Digital Automation Intelligence platform. Ran daily pair programming sessions that mentored junior engineers and sharpened team performance, and introduced RSpec to expand test coverage across the platform.

*  **Crowd Ox**: Raised a legacy code base to over 60% test coverage with 100% model coverage, migrating the Partner application's test suite from Minitest to RSpec while expanding platform features across three Ruby on Rails engines.

*  **USA Today**: Engineered a backend CMS with frontend content-creation interfaces and a responsive design that tightened user flows and elevated the customer experience.

*  **W. W. Norton**: Architected and shipped an interactive delivery platform serving over 300 interactives globally, and set the engineering bar for the team: GitFlow, code reviews, quality guidelines, and workflow management. Mentored junior engineers, raising their productivity and contributions.

*  **Gathrly**: Partnered with the founders to set the technical product roadmap and bring agile to the team. Led the design, engineering, and ongoing evolution of a lead management system for elite brewers, building a high-performance environment and mentoring junior engineers to raise their skills and output.

**Skills**:  AI · AI-Assisted Development · Agentic Systems · LLM-Powered Pipelines · Anthropic · OpenAI · xAI · Ruby on Rails · Mentoring · Pair Programming · Engineering Leadership · Legacy Modernization · Service-Oriented Architecture (SOA) · Software Development Life Cycle (SDLC) · Product Strategy · Community Development · Product Innovation · Microservices · Technical Architecture · Software Engineering · Strategic Leadership · Entrepreneurship · Product Development · Early-stage Startups · Business Process · Heroku · Redis · PostgreSQL · Amazon Web Services (AWS) · Hotwire · Bootstrap (Framework) · Sass

### Senior Product Engineer, Rootly 
**Remote** : Nevada   
2026  

* Owned the code that decides who gets paged: correctness and reliability of paging, alerting, and on-call scheduling across Rootly's incident-management platform. Worked from customer-reported ticket to verified fix, preferring the bugs where the system looks right but quietly does the wrong thing. Shipped 152 stories across eight teams, closed 43 production bugs, and took 20 escalations routed through support. Of those stories, 51 ranked Urgent or High and 40 traced to 34 distinct enterprise customers. Landed fixes with Claude Code assistance inside Rootly's Rails codebase.

* Fixed three ways the wrong person got paged: a level scheduler that matched the right escalation path, discarded it, and paged the default; deferred alerts that woke at a rotation handoff and paged the schedule owner instead of the on-call user; and shadows that paged a step behind their primary. Stopped schedules drifting in silence across 15 scheduling stories: a rotation edit at a cycle boundary that slid every shift, a daily job that walked every rotation back to its first member each week, member-list edits that re-anchored hours-based rotations, and a rotation turn dropped when its handoff fell after end time.

* Killed a silent config corruption where an escalation-path "matches" regex conditional re-saved as "is" and quietly rewrote customer routing rules on every edit, fixed along with a missing "Is One Of" operator. Closed four access-control gaps, three of them marked Urgent: a public API that accepted schedule overrides without checking role or team policy, users removed from the organization who stayed in on-call rotations and kept receiving shift notifications, SCIM group removal that reset Incident Response roles to None, and a broken RBAC notification sync.

* Stopped the public API returning 200 while losing data: an escalation-paths PUT discarded its default path and rules, a schedules endpoint under-returned against its own total count, and a shifts endpoint ignored hours-only shadow paging. Extended the same contract and its Terraform surface: a sequential-ID filter on the List Incidents API, plus acknowledgment and resolution timestamps on alerts. Corrected blocked calls to return 403 instead of 404, closed a 400 response that leaked resource IDs, and aligned datetime handling between API and UI.

* Held alerting available under load, clearing timeouts on route updates with large rule sets, duplicate re-triggers from a second acknowledgment, "Content missing" where a manual-page escalation hit a 4xx, and blank responses from the Slack page command. Cleaned the notification path behind it: fixed HTML-to-mrkdwn rendering including preformatted blocks and whitespace, cleared snooze failures on duplicate Slack records, and enriched /rootly paging confirmations with target names and alert links across page, escalate, and re-page flows. Surfaced non-paging alerts in the mobile app (release 2.15.0) with an edge-routing tenant header.

* Built the trial onboarding and demo-seed program end to end, a 44-story arc: a survey-driven onboarding wizard, a deterministic demo seed that ran offline, AI-generated playbooks and retro templates on by default in seed data, team and user reset tooling, and seed-correctness guardrails backed by automated evals. Tightened retrospectives alongside it: comment permissions, retros skipped for canceled incidents, and flag gating.

**Skills**: AI · AI-Assisted Development · Agentic Systems · LLM-Powered Pipelines · Claude Code · Ruby on Rails · REST APIs · Slack Integrations · Incident Management · Role-Based Access Control (RBAC) · Service-Oriented Architecture (SOA) · Software Development Life Cycle (SDLC) · Amazon Web Services (AWS) · Semaphore · Software Engineering 

### Senior Software Engineer, Goldbelly
**Remote** : Nevada & Colorado   
2022 - 2026  

* Partnered with the VP of Engineering to redesign Goldbelly's API architecture and shipped Version 4 of the Rails backend API, built to the OpenAPI specification with Semantic Versioning (SemVer) for backward compatibility. The upgrade enabled decoupling the e-commerce frontend to Next.js with auto-generated TypeScript API clients.

* Co-led design and development of E-Gifting on Goldbelly's e-commerce platform: senders pre-pay for food gifts from well-known chefs and restaurants, and recipients control their own delivery details. Built the feature across a React frontend and Rails backend.

* Worked with cross-functional teams to advance AI-assisted coding practices across the engineering organization, introducing Claude for code generation and Cursor for agentic workflows. Explored Model Context Protocol (MCP) integrations to automate routine engineering tasks.

* Helped launch Goldbelly's bulk checkout experience by leading a full refactor of tax processing. Replaced a single-threaded bottleneck with a bulk processing system for high-volume orders, and added backend support for canceling individual orders post-charge.

**Skills**: Service-Oriented Architecture (SOA) · AI · AI-Assisted Development · Cursor · Anthropic · OpenAI · xAI · Ruby on Rails · Microservices · OpenAPI · REST APIs · Software Development Life Cycle (SDLC) · Pair Programming · Engineering Leadership · Product Innovation · Technical Architecture · Software Engineering · Business Process · Heroku · Amazon Web Services (AWS) · PostgreSQL · React.js · Next.js · TypeScript · Redis

### Senior Software Engineer, Dutchie      
**Remote** : Colorado & Nevada    
2020 - 2022

* Spearheaded the launch of the Chain Billing Project, owning the architecture and implementation of the backend API. Modernized legacy code and APIs to integrate with the new data model.

* Founded an industry panel, the 155-member Ruby Guild, and a Rubyist Book Club focused on advancing RSpec testing techniques.

* Reviewed PRs, paired with engineers to clear blockers, supported outage response, and introduced new coding patterns across teams.

* Held regular 1-on-1s with engineers through periods of rapid headcount growth, reinforcing an inclusive, empathetic remote culture.

**Skills**: Ruby on Rails · Mentoring · Pair Programming · Engineering Leadership · Legacy Modernization · Service-Oriented Architecture (SOA) · Software Development Life Cycle (SDLC) · Microservices · Technical Architecture · Software Engineering · Business Process · Technical Project Leadership · Redis · PostgreSQL · MongoDB · Bootstrap (Framework) · Amazon Web Services (AWS)

### Senior Software Engineer, VYNYL  
**Remote** : Colorado    
2019 - 2020

* Led design and development of key features for an enterprise lending platform processing over $110 million in financial assets annually.

* Recruited, trained, and mentored a remote team of four engineers. Raised code quality through code reviews, RSpec testing practices, and Sandi Metz's design principles in Ruby.

**Skills**: Ruby on Rails · Pair Programming · Engineering Leadership · Software Development Life Cycle (SDLC) · Microservices · Technical Architecture · Software Engineering · Business Process · PostgreSQL

### Director of Engineering, onDiem      
**Remote** : Oregon    
2019  

* Led development of an on-demand staffing platform connecting dental offices with dental professionals for flexible shift work. Partnered with the founding team, head of product, and creative director on a roadmap prioritizing monetization and user feedback, and ran the team on Scrum. 

* Built platform integrations and automations that simplified operations for customers and the internal support team. Drove the codebase migration from Bitbucket to GitHub, adding continuous integration, security scanning, and style-guide enforcement. 

* Documented platform architecture and security protocols, cutting onboarding time for new engineers.

**Skills**: Mentoring · Pair Programming · Software Development Life Cycle (SDLC) · Product Strategy · Technical Architecture · Product Development · Business Process · Engineering Leadership · Service-Oriented Architecture (SOA) · Ruby · Product Innovation · Microservices · Software Engineering · Strategic Leadership · Heroku · PostgreSQL · Redis · Bootstrap (Framework)

### Senior Application Developer, MediaPRO     
**Remote** : Oregon    
2018 - 2019

*  Led the launch of LearningLAB, a platform that strengthens enterprise workforce defenses against cyber threats and privacy breaches. Owned backend testing and established quality best practices for the team.

* Built a full-stack dependency management process for two monolithic Ruby on Rails applications, keeping libraries current and reducing upgrade risk. 

* Introduced linting across the engineering team, improving code consistency and readability.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Technical Architecture · Business Process · Engineering Leadership · Legacy Modernization · Microservices · Software Engineering · Amazon Web Services (AWS) · PostgreSQL · Redis · Heroku · Ruby on Rails

### Senior Backend Engineer, WeaveUp  
**Remote** : Oregon  
June 2017 - April 2018  

*  Grew the backend team: recruited, onboarded, and trained new engineers, including the company's first Scrum project manager. Led the multi-stage architecture and rollout of Licensing 2.0, reworking design-content handling across hundreds of files in the backend API.

* Cut CI test runtimes from 25 minutes to 8 by migrating legacy Minitest specs to RSpec and running the suite in parallel on the continuous integration platform.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Technical Architecture · Business Process · Microservices · Software Engineering · Ruby on Rails · Amazon Web Services (AWS) · PostgreSQL · Redis

### Senior Full Stack Engineer, Coding Zeal  
**Remote** : Oregon    
October 2016 - June 2017  

*  Developed a recursive patient-logic report for a medical-industry client, improving metric analysis for data-driven decisions.

* Migrated a client application off MongoDB to a lower-cost database, improving performance and reducing operational costs.

* Led a refactor of Coding Zeal's referral-program website, improving UI/UX and lead conversion.

**Skills**: Mentoring · Pair Programming · Software Development Life Cycle (SDLC) · Technical Architecture · Business Process · Service-Oriented Architecture (SOA) · Microservices · Software Engineering · Ruby on Rails · Redis · PostgreSQL

### Senior Full Stack Developer, Whiplash
**Remote** : Oregon   
April 2016 - October 2016  

*  Developed an inbound and outbound ETL microservice with an integrated API, enabling real-time communication between third-party providers and the core Rails monolith.

* Introduced Slack and GitFlow, raising code quality and test coverage and connecting on-site and remote engineering, sales, and customer service teams.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Technical Architecture · Business Process · Microservices · Software Engineering · Ruby on Rails · PostgreSQL · Extract, Transform, Load (ETL) · Web Services API

### Senior Full Stack Engineer, BilingualHire
**Remote** : Oregon  
January 2016 - May 2016  

* Re-engineered an MVP for placing bilingual candidates in jobs across the U.S.: simplified the sign-up workflow, rebuilt the user interfaces, and expanded the data model to support multiple new languages.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Technical Architecture · Business Process · Product Innovation · Software Engineering · Ruby on Rails · Bootstrap (Framework) · PostgreSQL · Heroku

### Director of Application Engineering, PlaceWise    
**Remote** : Oregon & New York  
April 2014 - December 2015  

* Spearheaded the development of a Ruby on Rails service-oriented architecture that powered content delivery across more than 600 statically generated websites, improving Black Friday traffic handling, speeding content updates, and reducing DevOps costs.

**Skills**: Mentoring · Pair Programming · Software Development Life Cycle (SDLC) · Product Strategy · Technical Architecture · Product Development · Business Process · Engineering Leadership · Legacy Modernization · Service-Oriented Architecture (SOA) · Ruby · Product Innovation · Software Engineering · Strategic Leadership · Ruby on Rails · Technical Project Leadership · Adobe ColdFusion

### Web Applications Engineer, PlaceWise  
**Remote** : Oregon & New York    
August 2009 - April 2014  

* Ran online courses, real-time pairing, and career mentoring for the team, reducing knowledge silos, accelerating junior developer growth, and shortening project timelines.

* Migrated deployments from SVN to GitFlow on GitHub, stabilizing the continuous integration environment and speeding releases.

* Replaced a decade of legacy code in the RetailHub Enterprise Content Management Software, consolidating customer tools into a unified workspace and lifting performance and client satisfaction. Rolled out Slack enterprise-wide to improve team communication.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Business Process · Product Innovation · Software Engineering · Ruby on Rails · Adobe ColdFusion · Microsoft SQL Server · PostgreSQL

### Applications Developer, SOM  
**On-site** : Illinois  
January 2008 - March 2009  

* Built the project and task tracker used to coordinate construction of the Burj Khalifa, the world's tallest building, improving management collaboration and reducing duplicated work across teams.

* Refactored internal project-management software to support international languages and character sets for global teams.

**Skills**: Pair Programming · Software Development Life Cycle (SDLC) · Business Process · Software Engineering · Microsoft SQL Server · Adobe ColdFusion · Service-Oriented Architecture (SOA)

### Web Technology Team Lead, AT&T  
**On-site** : Illinois  
August 2001 - September 2007  

*  Led a regional team of five engineers, standardizing development practices across the Midwest with software style guidelines, scalability standards, and pair programming.

* Engineered a multi-tiered, metrics-driven dashboard application that surfaced actionable data enterprise-wide, cutting expenses, raising productivity, and helping prevent fraud.

* Reduced outages and improved customer satisfaction by standardizing online process delivery and building mission-critical applications targeting 24/7 availability with real-time administrative updates.

**Skills**: Mentoring · Pair Programming · Software Development Life Cycle (SDLC) · Product Development · Business Process · Engineering Leadership · Legacy Modernization · Product Innovation · Software Engineering · Strategic Leadership · Adobe ColdFusion · Microsoft SQL Server · Oracle Database

## CONFERENCES

* Rails World  
2024, 2025, 2026    

* RubyConf    
2018, 2019, 2026  

* Ai4    
2026    

* RubyKaigi  
2026    

* Kaigi on Rails  
2026    

* SF Ruby Conference  
2026    

* Friendly.rb  
2025

* EuRuKo  
2025

* Rocky Mountain Ruby  
2024  

* RailsConf    
2013, 2014, 2017, 2019  

* Ruby on Ales    
2014, 2015  

* Cascadia Ruby    
2013  

## COMMUNITY  

* Boulder Ruby Meetup Group    
2019 - `Present`   


* Turing School of Software & Design, Mentor & Volunteer Teacher        
2020 - 2022


* Boulder Open Coffee Club Meetup Group    
2019 - 2022   


* Full Stack PDX Meetup Group, Founder   
2017 - 2019   


* Mentorship Saturdays PDX Meetup Group, Mentor      
2016 - 2019		 

## EDUCATION

* Master of Business Administration, Keller Graduate School of Management  
* Bachelor of Science in Management Information Systems, Illinois College
