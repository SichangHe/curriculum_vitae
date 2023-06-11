# Work Experiences

## Work at DKU

### RA for Federated Learning research project (2023/03 - )

The [*FedCampus*][fedcampus] team project aims to develop a federated machine
learning (FL) platform for mobile devices.
It also aims to use this platform to conduct privacy-related experiments on DKU
campus.
It is lead by Professor Bing Luo.

As one of the example applications, we would monitor students' health
information without directly collecting it.
We would do on-device training with their health data,
then upload and aggregate the model parameters on our server.

#### Work summary for FedCampus

My job is to build the infrastructure to enable a FL deployment workflow.
In this workflow, the platform users would be able to, easily,
deploy machine learning models they designed for FL.

- Proposed and lead the adoption of [Flower][flower], an FL framework in Python.
    - Developed a demo to use Django servers to spawn and manage Flower servers
        in separate background processes on demand.
    - Investigated Flower server source code and applied customizations to save
        intermediate states into database.
    - Revamped the example Flower Android client to provide the team an SDK in
        the Kotlin programming language for FL.
    - Contributed to Flower by Pull Requests.
- Developed demos to, respectively, use HTTP, MQTT, and gRPC to communicate
    between Android clients and Python servers.
- Investigated and tried potential on-device training options on Android such
    as ONNX, MNN, PyTorch Mobile, FedML, and TensorFlow Lite, and landed on the
    latter.

#### Knowledge and skills gained from FedCampus

Deeply practiced mobile development, back-end development, and FL.

- Gathered Android development experience: handled on-device training,
    HTTP requests, SQLite3 database, and user interface using Kotlin.
- Practiced back-end development: built JSON APIs using Django REST Framework.
- Learn the ideas and practices of FL customizing Flower servers.

### Independent network research project (2023/04 - )

This project aims to provide network administrators a tool to find network
routing anomalies.
Professor Italo Cunha is my supervisor.
[The codebase on GitHub][parse_rpsl_policy] is named `parse_rpsl_policy`.

#### Work summary for `parse_rpsl_policy`

I parse Routing Policy Specification Language (RPSL) into efficient data
structures.
Then, I match actual internet routes against them to find routing anomalies.

- Studied Internet Engineering Task Force (IETF) RFC 4012 and 2622 for RPSL
    syntax and semantics.
- Developed an RPSL parser that produces recursive data structures in the Rust
    programming language.
    - Developed the lexer in Python with [PyParsing][pyparsing] to produce
        abstract syntax tree (AST).
    - Spawn Python lexer workers from Rust.
        Controlled them by piping their Stdin and Stdout.
    - Further parsed the AST into efficient data structures in Rust.
- Developed a comprehensive Rust module to compare Border Gateway Protocol (BGP)
    routes against RPSL policies.
    The comparison checks especially the filters and peerings of each autonomous
    system.
- Cached parsing result efficiently for extremely fast reloading by utilizing
    parallelism.
    Only 1sec to reload parsing result of the whole [RIPE Database][ripe].

#### Knowledge and skills gained from `parse_rpsl_policy`

String processing in Python; programming deeply nested data structures, and
high performance parallel programming in Rust.

- Practiced using Rust in Jupyter Notebook interactively with [Evcxr][evcxr]
    under its lifetime restrictions.
- Experienced string processing in Python using [PyParsing][pyparsing].
    - Used detailed docstrings to make up for the lack of a strong type system
        in Python.
- Designed custom types with clean programming interface to generate
    comparison reports.
    - Applied abstract algebra ideas to persist types across binary
        operations.
    - Utilized the `?` operator in Rust for always correct early return.
- Gained better understanding of StdIO locking when using Stdin and Stdout to
    dynamically pipe data between the Rust parser and the Python lexer.
- Gained hands-on experience on file system operation performance
    characteristics.
    - Split and serialized the parsing result into multiple JSON strings in
        parallel and saved them to disk sequentially for maximum speed.

<!-- TODO: This is where we left off. -->
### RA for search engine research project (2021/12 - 2023/05)

The *SSO* project aims to produce a search engine to search among DKU sites
and intranet.
It is supervised by Professor Jiang Long.

- Developed a web scraper in *Rust*.
    - Sent asynchronous and parallel web requests using Tokio and Reqwest.
    - Developed rich features including saving documents and scraping rings of
        web pages outside of the whitelist.
        <!-- TODO: What is this? -->
    - Made it stable so it ran daily, flawlessly since deployment.
    - Fine-tuned the Regular Expression (regex) filter and blacklist for the
        best set of web pages.
- Helped the team with search engine front end and back end development.
    - Created a modern-looking search interface with Django, HTML, ECMAScript,
        and Tailwindcss.
    - Learned to use Django's Object-Relational Mapping (ORM) to manipulate the
        database.
    - Improved HTML processing code in Python.
        Cleaned up noisy HTML tags using BeautifulSoup.
    - Practiced Git for version control and teamwork.
        - Handled large Git merge conflicts due to parallel development on the
            same files.
- Became inactive in the project after it slowed down dramatically and the
    project goal became vague under the quests for features.
- Learned from the downfall of the project.
    - Learned how a well-defined and well-scoped goal is crucial for any project
        at any time.
    - Experienced the importance of coding best practices for long-term
        maintainability.
    - Witnessed how hype and motivation of the members are essential for any
        project.

### iGEM 2022 DKU team (2021/11 - 2022/10)

Our team won a silver medal in the International Genetically Engineered Machine
(iGEM) Biology competition.

- Developed [the team Wiki][igem_wiki], a static site.
    - Used [mdBook][mdBook] and [mdBook-KaTeX][mdbook-katex] to render Markdown
        and LaTeX math expressions into static HTML.
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
- Learned from working with non-technical Biology team members.
    - Learned how strongly ordinary people resist to exit their software comfort
        zones and learn new software.
    - Realized that Git is too complicated for most non-technical teams.
    - Understood that unicast is the only effective team communication.

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

### Academic Resource Center tutor (2021/05 - 2022/05)

- Obtained a [CRLA certificate][crla] after tutoring for two semesters.
- Tutored MATH 201—Multivariate Calculus, MATH 105—Calculus, and COMPSCI 201.

### Other work at DKU

- Intersections editor and translator (2021/06 - 2021/08)
    - Lead by Professor Austin Woerner.
    - Worked as a Chinese editor and translator.
        Co-translated three articles and reviewed a few.
        These articles are published on Intersections' WeChat public account and
        [its website][intersections].
    - Created a video tutorial: [using OneDrive and Microsoft Word for
        collaboration][onedrive_microsoft].

[crla]: https://github.com/SichangHe/curriculum_vitae/files/11665403/CRLA_certificate.pdf
[cs201_setup]: https://www.youtube.com/watch?v=yiL-ULPBkvE
[evcxr]: https://github.com/evcxr/evcxr
[fedcampus]: https://github.com/FedCampus
[flower]: https://flower.dev/
[igem_wiki]: https://github.com/SichangHe/igem-2022-dku-backup
[intersections]: https://sites.duke.edu/intersections/
[mdBook]: https://github.com/rust-lang/mdBook
[mdbook-katex]: https://github.com/lzanini/mdbook-katex
[onedrive_microsoft]: https://www.youtube.com/watch?v=mYPLp_gtHkM
[parse_rpsl_policy]: https://github.com/SichangHe/parse_rpsl_policy
[pyparsing]: https://github.com/pyparsing/pyparsing/
[ripe]: https://www.ripe.net/manage-ips-and-asns/db
[vscode_git_intro]: https://www.youtube.com/watch?v=C-sAGuWM2JM
