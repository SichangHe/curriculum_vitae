# Side Projects

## Happy projects

### Maintain & develop [mdBook-KaTeX][mdbook-katex] (2022/11 - )

mdBook-KaTeX is a preprocessor for [mdBook][mdBook] in *Rust*.
It pre-renders LaTeX math expressions to HTML using KaTeX.

[![mdBook-KaTeX version][mdbook-katex_version]
![mdBook-KaTeX downloads][mdbook-katex_downloads]][crates_mdbook-katex]

- Took over [maintainership by publishing a fork][mdbook-katex2]
    when the project was unmaintained.
- Resolved more than 18 GitHub issues opened by others by fixing the bugs.
    For example:
    - Fixed persisting Markdown rendering bugs.
        For example, KaTeX outputs newline characters, [which broke Markdown
        rendering in tables and headers][katex-break-table].
        Fixed by replacing newline characters.
    - Fixed several error handling bugs.
        For example, fixed crashing on placeholder chapters.
    - Worked around Windows platform support from upstream.
        Discovered an alternative, working, but slightly compromised dependency
        by communicating with upstream `katex_rs` developers.
    - Fixed the GitHub CIs for MUSL Linux and Windows builds.
        Use cross compilation to provide full-feature builds.
- Improved speed by 10 times (on an M1 MacBook) by adopting parallelism and
    avoiding repeated rendering.
- Developed new features up to the point that mdBook-KaTeX is considered
    feature-complete. For example:
    - Adopted feature to preserve fenced code blocks according to CommonMark
        specification.
        Accomplished by hand-writing a finite-state machine to scan through
        Markdown code.
    - Added other features such as options to include math expressions source,
        enable MathML for accessibility, and use custom delimiters.
- Deprecated the problematic `static-css` feature gradually and provided an
    alternative.

### Author & maintain [recursive_scraper][recursive_scraper] (2022/06 - )

A web scraper in *Rust* that scrapes recursively, at constant frequency
(requests per time), asynchronously.

[![recursive_scraper version][scraper_version]
![recursive_scraper downloads][scraper_downloads]][crates_scraper]

- Learned from the design mistakes in [the SSO scraper][ra_search_engine] and
    chose elegant and maximally simple designs.
- Implemented without using mutexes or channels.
    Instead, used [`FuturesUnordered`][futures_unordered] to queue
    self-contained tasks.

### Other happy projects

- [Maintains and contributed to Open Source projects on
    GitHub][contribution_activity].
- [Configuration files][config].
    - Over 1000 lines of Lua for my modal editor Neovim and my tiling window
        manager Yabai.
    - Configuration for Fish shell, Starship, and Alacritty.
    - Support my smooth terminal and keyboard workflow.
- Learned new programming languages on [Exercism][exercism].
- Explored various operating systems.
    - Installed Windows 10 & 11,
        several Linux distributions such as Arch Linux, and FreeBSD,
        on hardware, on Parallels Desktop, and on QEMU/KVM.
    - Built a Hackintosh on a ThinkPad, but did not have Wi-Fi.
        Switched to QEMU/KVM instead.
- Explored various text editors such as IntelliJ and Doom Emacs.
    Daily drove Visual Studio Code before switching to Neovim.

## Failed projects

### Academic forum

<!-- TODO -->

### Forum using Ruby on Rails (2022/06 - 2022/08)

[Forum][forum] using Ruby on Rails and Hotwire.

- Deployed it on Heroku.
- Developed features such as infinitely nested comments and MathJax support.

[config]: https://github.com/SichangHe/.config
[contribution_activity]: https://github.com/SichangHe#js-contribution-activity
[crates_mdbook-katex]: https://crates.io/crates/mdbook-katex
[crates_scraper]: https://crates.io/crates/recursive_scraper
[exercism]: https://exercism.org/profiles/SichangHe
[forum]: https://github.com/SichangHe/forum
[futures_unordered]: https://docs.rs/futures/latest/futures/stream/struct.FuturesUnordered.html
[katex-break-table]: https://github.com/lzanini/mdbook-katex/issues/3
[mdBook]: https://github.com/rust-lang/mdBook
[mdbook-katex]: https://github.com/lzanini/mdbook-katex
[mdbook-katex_downloads]: https://img.shields.io/crates/d/mdbook-katex
[mdbook-katex_version]: https://img.shields.io/crates/v/mdbook-katex
[mdbook-katex2]: https://github.com/lzanini/mdbook-katex/issues/37
[ra_search_engine]: https://sichanghe.github.io/curriculum_vitae/work_experiences/index.html#ra-for-search-engine-research-project-202112---202305
[recursive_scraper]: https://github.com/SichangHe/scraper
[scraper_downloads]: https://img.shields.io/crates/d/recursive_scraper
[scraper_version]: https://img.shields.io/crates/v/recursive_scraper
