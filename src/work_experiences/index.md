# Work Experiences

## Work at DKU

### RA for Federated Learning research project (2023/03 - )

The [*FedCampus*][fedcampus] project aims to develop a federated learning
platform for mobile devices and use it to conduct experiments on DKU campus.
For example, one of the applications is to monitor students' health information
without directly collecting it.
It is lead by Professor Bing Luo.

- Investigated and tried potential on-device training options on Android such
    as ONNX, MNN, PyTorch Mobile, FedML, and TensorFlow Lite, and landed on the
    latter.
- Developed separate demos to use HTTP, MQTT, and gRPC to communicate between
    Android clients and Python servers.
- Proposed and lead the use of [Flower][flower], a federated learning framework
    in Python.
    - Contributed to Flower by Pull Requests.
    - Investigated Flower server source code and applied customizations to save
        model parameters into database.
    - Revamped the example Flower Android client to provide the team an SDK in
        *Kotlin* for federated learning.
    - Developed a demo to use Django servers to spawn and manage Flower servers
        in separate background processes on demand.
- Learned and practiced mobile development, federated learning, and back-end
    development.
    - Learned Android development.
    - Learned to use the Kotlin programming language.
    - Learned the ideas and practices of federated learning using FLower.
    - Practiced back-end development using Django REST Framework.

### Independent network research project (2023/04 - )

The [parse_rpsl_policy][parse_rpsl_policy] project aims to find network routing
anomalies.
I am doing with it Professor Italo Cunha.
I parse Routing Policy Specification Language (RPSL) into efficient data
structures in *Rust*.
Then, I match actual internet routes against them to find routing anomalies.

- Studied Internet Engineering Task Force (IETF) RFC 4012 and 2622 for RPSL
    syntax and semantics.
- Developed an RPSL lexer in Python with [PyParsing][pyparsing] to produce
    abstract syntax tree (AST).
- Further parsed the AST into efficient data structures in Rust.
- Used *Rust* in Jupyter Notebook with [Evcxr][evcxr] to compare Border Gateway
    Protocol (BGP) routes against RPSL policies interactively.
- Practiced string processing and programming deeply nested data structures
    efficiently in Python and *Rust*.
    - Practiced using detailed docstrings to make up for the lack of a strong
        type system in Python.
    - Practiced parallel programming in *Rust*.
    - Experimented using Stdin and Stdout to dynamically pipe data between the
        *Rust* parser and the Python lexer.
    - Designed custom *Rust* types using a little category theory to provide
        nice experience to generate match reports.
        <!-- TODO: Explain better. -->

### RA for search engine research project (2021/12 - 2023/05)

The *SSO* project aims to produce a search engine to search among DKU sites
and intranet.
It is supervised by Professor Jiang Long.

- Developed a web scraper in *Rust*.
    - Asynchronous and parallel web requests using Tokio and Reqwest.
    - Rich features including saving documents and scraping rings of web pages
        outside of the whitelist.
        <!-- TODO: What is this? -->
- Helped the team with search engine front end and back end development.
    - Created a modern-looking search interface with Django, HTML, ECMAScript,
        and Tailwindcss.
    - Improved HTML processing code in Python.
        Cleaned up noisy HTML tags using BeautifulSoup.
- Quit the project after it slowed down dramatically and the project goal
    became vague under the quests for features.
- Learned from the failure of the project.
    - Learned how a well-defined and well-scoped goal is crucial for any project
        at any time.
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
    - [VS Code & Git introduction video for the team][vscode_git_intro].
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

### Other work at DKU

<!-- TODO -->
- Academic Resource Center tutor (2021/05 - 2022/05)
- Intersections editor and translator (2021/06 - 2021/08)

[cs201_setup]: https://www.youtube.com/watch?v=yiL-ULPBkvE
[evcxr]: https://github.com/evcxr/evcxr
[fedcampus]: https://github.com/FedCampus
[flower]: https://flower.dev/
[igem_wiki]: https://github.com/SichangHe/igem-2022-dku-backup
[mdBook]: https://github.com/rust-lang/mdBook
[mdbook-katex]: https://github.com/lzanini/mdbook-katex
[parse_rpsl_policy]: https://github.com/SichangHe/parse_rpsl_policy
[pyparsing]: https://github.com/pyparsing/pyparsing/
[vscode_git_intro]: https://www.youtube.com/watch?v=C-sAGuWM2JM
