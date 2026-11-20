

- Education
- Research Experience
- Teaching Experience
- Awards
- Side Projects
- Outreach
- Skills

[]

Sichang “Steven” He sichangh@usc.edu

Ph.D. Student in Computer Science GitHub & YouTube @SichangHe

Networked Systems Lab (NSL), University of Southern California
sichanghe.github.io

Interested in systems problems of the web that impact ordinary people. I
built large-scale Internet measurements.

Education

University of Southern California (USC) Aug. 2024 – 2029 (Est.) Los
Angeles, CA

Ph.D. in Computer Science (CS) Advisor: Harsha V. Madhyastha

– Also work with Ramesh Govindan.

– Selected courses with projects:

∗ Advanced Computer Networking (A+): JSphere: measure webpages’ browser
API calls to classify JavaScript.

∗ Advanced NLP (A): Reproduced an EMNLP LLM detection paper and
challenged its generalizability.

Duke Kunshan University (DKU) & Duke University Dual Degree Aug. 2020 –
May 2024

B.S. in Data Science (by DKU) & Kunshan, China &

B.S. in Interdisciplinary Studies (Subplan: Data Science, by Duke)
Durham, NC

– Completed most required courses for CS and Mathematics majors.

– Select courses with projects:

∗ Computer Network Architecture (A+): async TCP server and client in
Elixir and CLI REPL shell in Rust.

∗ Data Acquisition and Visualization (A): Poster using D3.js, Svelte,
and TypeScript.

∗ Computer Organization and Programming (A+, at Duke): Binary search
tree in MIPS assembly and ring buffer

in C; fifth place in PizzaCalc assembly length optimization competition
(68 lines).

∗ Numerical Analysis (A+); Intro Abstract Algebra (at Duke), Complex
Analysis (A).

Zhixin High School Aug. 2017 – Jun. 2020 Guangzhou, China

– Chemistry Olympiad competition team; Biology Olympiad competition
team.

Publications

[1] Sichang Steven He, Ramesh Govindan, and Harsha V. Madhyastha.
“Poster: Did I Just Browse A

Website Written by LLMs?” In: Proceedings of the 2025 ACM Internet
Measurement Conference and Student

Workshop (IMC). Video. Oct. 2025.

[2] Sichang He, Italo Cunha, and Ethan Katz-Bassett. “RPSLyzer:
Characterization and Verification of

Policies in Internet Routing Registries”. In: Proceedings of the 2024
ACM Internet Measurement Conference

(IMC). Video. Nov. 2024.

[3] Sichang He, Beilong Tang, Boyan Zhang, Jiaqi Shao, Xiaomin Ouyang,
Daniel Nata Nugraha, and

Bing Luo. “FedKit: Enabling Cross-Platform Federated Learning for
Android and iOS”. In: IEEE INFOCOM

Demo. Video. May 2024.

In Progress

[1] Sichang Steven He, Calvin Ardi, Ramesh Govindan, and Harsha V.
Madhyastha. “DeGenTWeb: A

First Look at MGT-dominant Websites”. 2026.

Research Experience

Research Assistant Aug. 2024 – present

Networked Systems Lab, USC Advisor: Harsha V. Madhyastha

– Rigorously measured how much of the web is now written by LLMs;
brought a transparent methodology and

representative samples to substantiate the folk wisdom surrounding the
use of LLM on the web.

Sichang “Steven” He | University of Southern California Page 1 of 3

[]

∗ Built DeGenTWeb, a website-level detector for websites whose textual
content is dominated by LLMs.

∗ Achieved an ultra low P90 false positive rate of 0.12% on 6k baseline
websites (90k webpages).

∗ Flagged 21% of 117k Common Crawl websites and 14% of 18k sites from
Bing search results.

∗ Substantiated the claim that the use of LLM text grew with hard
evidences.

∗ Identified clear financial incentives for websites dominated by LLM
texts.

– Surveyed usage, weakness, and extensions of the Coalition for Content
Provenance and Authenticity (C2PA).

Agentic Formal Verification for Rust/Verus Jun. 2026 – Oct. 2026

Midas Intelligence Inc. (math-for-AI startup), San Francisco (Remote)

– Invented the company’s software story: achieve both development
velocity and reliability via agents and Verus.

– Led and solely established the company’s software division. Reported
directly to the president and the CEO.

– Created Midas Lex, a tool that guides agents to write Verus
specifications and proofs.

– Found bugs in popular open source Rust projects like uutils coreutils.
Built benchmarks of unsolved Verus tasks.

Independent research, Internet Route Verification Apr. 2023 – May 2024

Federal University of Minas Gerais, Brazil (Remote) Advisor: Italo Cunha

– Conducted one of the most thorough examinations of public Internet
interdomain routing policies in the Internet

Routing Registry (IRR). The IRR underpins much of the Internet, is used
to guide public peering, aid routing issue

troubleshooting, and avoid routing misconfiguration and attacks that can
cause global Internet outages.

– Built RPSLyzer, the first operational interpreter to parse 99.99% of
routing policies in the IRR in the Routing Policy

Specification Language (RPSL), and to check whether real, observed
Border Gateway Protocol (BGP) routes follow

them per IETF RFC 2622 and RFC 4012.

∗ Efficient: parsed the entire IRR (7 GB) in under 5min; checked 779M
BGP routes under 3 hr with 2 GB of RAM.

∗ RPSLyzer correctly parses intricate RPSL constructs, including
advanced set operations and a custom regex.

∗ Completed all implementation alone, mainly using Rust.

∗ Characterized the policies of 78,701 autonomous systems (ASes). Found
a wide variation in RPSL usage: several

ASes declare thousands of policies, while 53% declare none at all.

– Checked and analyzed whether observed interdomain routes match routing
policies with RPSLyzer; identified com-

mon RPSL usage patterns and usage mistakes.

∗ Found that 40% of interconnections in observed BGP routes cannot be
verified due to missing policies.

∗ Incorporated CAIDA AS relationship data to improve verification
coverage by 19%.

∗ Provided tooling to verify routes against the RPSL, helping improve
interdomain routing security.

∗ Identified and implemented checks for 6 major explanations to why
routes fail to match the relevant RPSL.

Research Assistant, Mobile Federated Learning (FL) Mar. 2023 – May. 2024

The FedCampus Team, EdgeIntelligence Lab, DKU Advisor: Bing Luo

– Authored the FedKit SDKs, the first practical way to conduct
real-world FL experiments across Android and iOS

devices, which enables training shared ML models collaboratively without
sharing private data on phones.

∗ Streamlined research: automatically converted model formats and pushed
models directly onto the phones.

– Wrote the official Android Kotlin example for Flower, the popular FL
framework by Flower.ai, a Y-Combinator

startup founded by Cambridge University professors. Consequently, got
invited to speak at the Flower AI Summit.

∗ Helped correct the iOS example after finding that it was not training.

– Led a team of six to develop the FedCampus app, an Android & iOS app
that leverages personal health data from

over 100 participants to conduct real-world FL and federated analytics
experiments on campus.

∗ Mentored the team, 4 undergrads and 1 M.Eng. student; interviewed and
recruited 2 of which.

∗ Investigated and led core technology adoption, including Flower,
Kotlin, and Flutter.

Research Assistant, Search Engine Research Dec. 2021 – May 2023

The Search So Team, DKU Advisor: Jiang Long

– Developed a feature-rich open source web scraper in async Rust to
scrape DKU sites, intranet, and Duke sites.

– Improved backend HTML processing, frontend interface, and version
control.

Sichang “Steven” He | University of Southern California Page 2 of 3

[]

Talks

[1] Bing Luo and Sichang He. “FedCampus: a Privacy-preserving Data
Platform for Smart Campus with

Federated Learning and Analytics”. Flower AI Summit, 2024. Mar. 2024.

Teaching Experience

Teaching Assistant, Introduction to Programming, DKU Nov. 2021 – Mar.
2022

– Hosted weekly lab sessions; created the course’s first video tutorial
on development environment setup.

Math & CompSci. Tutor, Academic Resource Center, DKU May 2021 – May 2022

– Obtained CRLA’s International Tutor Training Program Certification,
Level I .

Awards

• ACM Internet Measurement Conference (IMC) Travel Grant (Sep. 2025)

• ACM Internet Measurement Conference (IMC) Student Travel Grant (Aug.
2024)

• Senior Scholar-Athlete Award through the Running Club, DKU Athletics
(Apr. 2024)

• Silver Medal, International Genetically Engineered Machine (iGEM) 2022
DKU Team (Oct. 2022)

Developed the team wiki independently; helped non-technical members
adopt Git; validated protein designs with

modeling software.

• Dean’s List (Spring 2021) & Dean’s List with Distinction (Fall 2021,
Fall 2022, Spring 2023), DKU

• Chancellor’s Scholarship & UGRD Entrance Scholarship, DKU
(merit-based, Fall 2020 – Spring 2024)

Side Projects

Open Source Developer & Maintainer of Rust Libraries Nov. 2022 – present

– mdBook-KaTeX, a math expression preprocessor for mdBook with over 200k
downloads on crates.io. Took over

maintainership when it was unmaintained. Resolved 20 old issues, added
features, improved speed 10×.

– Contributed to mdBook, cargo-binstall, pulldown-cmark-to-cmark, and
others.

– Voice control for an agent manager, Elixir-style async Rust, efficient
Rust environment, collaborative editor.

Outreach

• Chinese Editor & Translator at DKU Intersections Journal Jun. 2021 –
Aug. 2021

Co-translated three English articles into Chinese; reviewed and edited
multiple articles and Intersections’ website.

Skills

Natural Language Mandarin (native), Cantonese (fluent).

Programming Language

– Invested and proficient: Rust, Python, Elixir, JavaScript.

– Used in projects: Kotlin, Dart, Swift, Ruby, Java, Lua, TypeScript,
Svelte, HTML, CSS, C, SQL, Racket, L

A

T

E

X,

PL/pgSQL.

– Familiar: C++, Bash, Julia, Go, Erlang, Gleam, Mathematica, MATLAB,
Scala, R.

Concurrency Event-loop in Rust Tokio, JavaScript, Dart, Swift; Kotlin
coroutines; Elixir/OTP processes.

Sichang “Steven” He | University of Southern California Page 3 of 3

[]
