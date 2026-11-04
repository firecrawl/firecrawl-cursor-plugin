# Research code and APIs

Use this route when the question requires repository code, issue discussions
or pull requests, rather than an answer from official documentation alone. Use
`read-docs` for documented setup, usage, migrations and compatibility. A supplied
issue or repository can be investigated directly; a documentation search is not
a prerequisite.

Use `firecrawl_developer_search` for library behavior, API contracts, error
messages, known bugs, and implementation examples in indexed public repositories
and documentation. Include the library, version, and exact error or symbol when
known. Read the returned matched passages and their source URLs.

Distinguish official documentation from issues, proposals, and merged pull
requests. A merged fix does not establish that it shipped in the user's version.
Use `firecrawl_scrape` on a source URL when the passage lacks the needed context.
Use `firecrawl_search` when the relevant source is outside the index or the index
does not resolve the question.

Answer from the retrieved evidence, cite the relevant sources, and state any
unverified version or release boundary.
