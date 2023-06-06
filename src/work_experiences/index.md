# Work Experiences

## Works at DKU

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
    Android clients and Django servers.
- Proposed and lead the use of [Flower][flower], a federated learning framework
    in Python.
    - Contributed to Flower by Pull Requests.
    - Investigated Flower server source code and applied customizations to save
        model parameters into database.
    - Revamped the example Flower Android client to provide the team an SDK in
        *Kotlin* for federated learning.
    - Developed a demo to use Django servers to spawn and manage Flower servers
        in separate background processes on demand.

### RA for search engine research project (2021/12 - 2023/05)

The *SSO* project aims to produce a search engine to search among DKU sites
and intranet.
It is lead by Professor Jiang Long,

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

### Other works at DKU

<!-- TODO -->
- Independent research on finding network routing anomalies (2023/04 - )
- iGEM 2022 DKU team (2021/11 - 2022/10)
- TA for COMPSCI 201 (2021/11 - 2022/03)
- Academic Resource Center tutor (2021/05 - 2022/05)
- Intersections editor and translator (2021/06 - 2021/08)

[fedcampus]: https://github.com/FedCampus
[flower]: https://flower.dev/
