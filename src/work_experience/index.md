# Work Experience

## Research experience

### RA for Federated Learning project (2023/03 - )

Supervisor: Dr. Bing Luo.

Lead our project, [*FedCampus*][fedcampus], to develop a federated machine
learning (FL) platform for mobile devices,
to enable FL experiments on DKU campus using health data from smartwatches.

#### Work summary for FedCampus

- Developed [FedKit][fed_kit], an open source FL framework for mobile devices,
    supporting on-demand training, model deployment from the backend,
    model check-pointing, and Android on-device training.
- Supervised and mentored two undergraduate student in the development of
    *the FedCampus app*, a cross-platform mobile application to conduct FL
    experiments using personal health data.
- Investigated, proposed, and lead the adoption of core technologies including
    [Flower][flower] for FL scheduling, [TensorFlow Lite][tflite] for Android
    on-device training, and [Flutter][flutter] for rapid cross-platform app
    development.
- Revamped Flower's Android example and upstreamed the contribution.
- Interviewed and recruited a UI programmer and a designer.
<!-- - Leveraged Django REST Framework to spawn and manage Flower servers
    in separate background processes on demand. -->
<!-- - Investigated Flower server source code and applied customizations to save
    intermediate states into database. -->
<!-- - Demonstration using HTTP, MQTT, and gRPC to communicate
    between Android clients and Python servers.
- Investigated and tried potential on-device training options on Android such
    as ONNX, MNN, PyTorch Mobile, FedML, and TensorFlow Lite, and landed on the
    latter. -->

#### Knowledge and skills gained from FedCampus

Mobile development, backend development, and FL.

- Android development experience: on-device training,
    HTTP communication, SQLite3 database, and user interface in Kotlin.
- Backend development: JSON APIs and database management via Django ORM.
- Ideas and implementations of FL.

### Independent network research project (2023/04 - )

Supervisor: Dr. Italo Cunha.

Ran [Internet Route Verification][irv] (IRV), a project to provide network
administrators a tool to find network routing anomalies.

#### Work summary for IRV

Parsed Routing Policy Specification Language (RPSL) into efficient data
structures.
Matched actual internet routes against RPSL to find routing anomalies.

<!-- - Studied Internet Engineering Task Force (IETF) RFC 4012 and 2622 for RPSL -->
<!--     syntax and semantics. -->
- Developed the lexer in Python with [PyParsing][pyparsing] to produce
    abstract syntax tree (AST) and controlled them in Rust via pipes.
- Developed a parser in Rust that instantly parses the AST in parallel and
    produces efficient recursive intermediate representations.
- Developed a comprehensive Rust module to compare Border Gateway Protocol (BGP)
    routes against RPSL policies,
    checking especially the filters and peerings of each autonomous system.
<!-- - Cached parsing result efficiently for extremely fast reloading by utilizing
    parallelism.
    Only 1sec to reload parsing result of the whole [RIPE Database][ripe]. -->

#### Knowledge and skills gained from IRV

High performance parallel programming in Rust, programming language parser,
string processing.

- Used Rust in Jupyter Notebook and REPL interactively with [Evcxr][evcxr]
    under its lifetime restrictions.
<!-- - Experienced string processing in Python using [PyParsing][pyparsing].
    - Used detailed docstrings to make up for the lack of a strong type system
        in Python. -->
- Designed custom types with clean programming interface to generate
    comparison reports, applying abstract algebra ideas and utilizing the `?`
    operator in Rust for guaranteed-correct early returns.
- Gained better understanding of StdIO locking using Stdin and Stdout to
    dynamically pipe data between the Rust parser and the Python lexer.
- Gained hands-on experience on file system operation performance
    characteristics.
    <!-- - Split and serialized the parsing result into multiple JSON strings in
        parallel and saved them to disk sequentially for maximum speed. -->

### RA for search engine research project (2021/12 - 2023/05)

Supervisor: Dr. Jiang Long.

The SSO project aims to produce a search engine to search among DKU sites
and intranet.

#### Work summary for SSO

My main work was to gather source information for the search engine by scraping
DKU intranet.
I also helped improve our web server.

- Developed a web scraper in the Rust programming language.
    - Sent asynchronous and parallel web requests using Tokio and Reqwest.
    - Developed rich features including saving documents and scraping rings of
        web pages outside of the whitelist.
        <!-- TODO: What is this? -->
    - Made it stable so it ran daily, flawlessly since deployment.
    - Fine-tuned the Regular Expression (regex) filter and blacklist for the
        best set of web pages.
- Helped the team with search engine front end and back end development.
    - Created a modern-looking search interface.
    - Improved HTML processing code in Python.
        Cleaned up noisy HTML tags using BeautifulSoup.

#### Knowledge and experience gained from SSO

- Gained real-world experience of asynchronous programming in Rust.
- Learned to use Django views and Tailwindcss for the search interface.
- Learned to use Django's Object-Relational Mapping (ORM) to manipulate the
    database.
- Practiced Git for version control and teamwork.
    - Handled large Git merge conflicts due to parallel development on the
        same files.

The project slowed down dramatically and the project goal became vague in the
quests for features.
I learned much more from the downfall of SSO.

- Learned how a well-defined and well-scoped goal is crucial for any project
    at any time.
- Witnessed how hype and motivation of the members are essential for any
    project.
- Experienced the importance of coding best practices for long-term
    maintainability.
- Saw the danger of proprietary research projects and the beauty of open source
    in its immortality.
    [Rewrote the scraper and released it as open source][scraper_project].

### iGEM 2022 DKU team (2021/11 - 2022/10)

Our team won a silver medal in the International Genetically Engineered Machine
(iGEM) Biology competition.

#### Work summary for iGEM

I joined as a modeling team member, but ended up working as a Wiki developer
and IT support.

- Developed [the team Wiki][igem_wiki], a static site.
    - Used [mdBook][mdBook] and [mdBook-KaTeX][mdbook-katex] to render Markdown
        with LaTeX math expressions into static HTML.
    - Used Tailwindcss to style the Wiki, and JavaScript for the animations.
    - Set up GitLab CI to build and deploy the Wiki to GitLab Pages
        automatically so non-technical members could preview their changes.
    - Organized and communicated with non-technical members for the Wiki
        content.
- Pushed the team to fully adopt Git, GitLab, Visual Studio Code, and Markdown.
    The process was hard and we had very limited success.
    - Filmed a [VS Code & Git introduction video for the team][vscode_git_intro].
- Used protein modeling software to validate teammates' protein design:
    RoseTTAFold, Robetta, PyMOL.

#### Knowledge and experience gained from iGEM

- Learned web development basics with HTML, JavaScript, CSS, and Tailwindcss.
- Hacked GitLab CI to work.
    Experienced the difficulty of debugging remote systems.
- Learned from working with non-technical Biology team members.
    - Learned how strongly ordinary people resist to exit their software comfort
        zones and learn new software.
    - Realized that Git is too complicated for most non-technical teams.
    - Understood that unicast is the only effective team communication.

## Teaching experience

### TA for COMPSCI 201 (2021/11 - 2022/03)

I accepted Professor Jiang Long's invitation to be a teaching assistant for
COMPSCI 201—Introduction to Programming and Data Structures.

- Hosted weekly Lab sessions and office hours.
- Eased students' burden to set up the environment for the course.
    - Helped simplify the Windows setup by switching from online virtual
        machines to Windows Subsystem for Linux (WSL).
    - Created text-based and [video tutorial on how to set up][cs201_setup].
        COMPSCI 201 students have been given the video tutorial ever since,
        and everyone I have asked said it was helpful.
- Learned from teaching students new to programming.
    - Learned that the fear for unfamiliar topics and fields is the biggest
        obstacle for learning.
    - Practiced approaching new concepts in easy ways such as comparing to
        day-to-day life and using analogies.
        Verified that this strategy is extremely effective.

### Academic Resource Center (ARC) tutor (2021/05 - 2022/05)

- Tutored MATH 201—Multivariate Calculus, MATH 105—Calculus, and COMPSCI 201.

## Certification

- [CRLA certificate][crla] from tutoring for two semesters in the ARC.

## Community service

- Intersections editor and translator (2021/06 - 2021/08)
    - Lead by Professor Austin Woerner.
    - Worked as a Chinese editor and translator.
        Co-translated three articles and reviewed a few.
        These articles are published on Intersections' WeChat public account and
        [its website][intersections].
    - Created a video tutorial: [using OneDrive and Microsoft Word for
        collaboration][onedrive_microsoft].
- Volunteered in the event to teach children with special need in Bacheng
    about Easter (2020/11).

[crla]: https://github.com/SichangHe/curriculum_vitae/files/11665403/CRLA_certificate.pdf
[cs201_setup]: https://www.youtube.com/watch?v=yiL-ULPBkvE
[evcxr]: https://github.com/evcxr/evcxr
[fedcampus]: https://github.com/FedCampus
[fed_kit]: https://github.com/FedCampus/FedKit
[flower]: https://flower.dev/
[flutter]: https://flutter.dev/
[igem_wiki]: https://github.com/SichangHe/igem-2022-dku-backup
[intersections]: https://sites.duke.edu/intersections/
[mdBook]: https://github.com/rust-lang/mdBook
[mdbook-katex]: https://github.com/lzanini/mdbook-katex
[onedrive_microsoft]: https://www.youtube.com/watch?v=mYPLp_gtHkM
[irv]: https://github.com/SichangHe/internet_route_verification
[pyparsing]: https://github.com/pyparsing/pyparsing/
[scraper_project]: ../side_projects/index.html#author--maintain-recursive_scraper-202206---
[tflite]: https://www.tensorflow.org/lite/
[vscode_git_intro]: https://www.youtube.com/watch?v=C-sAGuWM2JM
