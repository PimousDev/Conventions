# Folder Structure
<table>
	<thead>
		<tr>
			<th>Status</th>
			<th>Verification</th>
			<th>Authors</th>
			<th>Created date</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Under study</td>
			<td>-</td>
			<td><a href="https://www.github.com/Xibitol">Xibitol</a></td>
			<td>Feb 26, 2024</td>
		<tr>
	</tbody>
</table>

### Roadmap

## Convention
No plurial: Because we could put them any where, so we choosed to not use them.
Files and folders are always in camelCase.

Repository and git files in UpperCase:
- `/README.md`
- `/LICENSE.md|COPYING|COPYING.*` depending on the licensing authority.
- `.gitignore`

Non-programming files (Pimous Dev. specific) under `/Content/` in PascalCase:
- `Logo/`: See #design/logo.
- `Diagram/`: UML.
- `UI/`: UX (Wireframes) and UI.
- `Screenshot/<number>.png`: Project screenshots.
- `Font`: Some fonts used in the project (?).
- `Image/`: Some raw/edited images used in the project.
- `Video/`: Some raw/edited videos used in the project.
- `Archive/`: Raw archives or special packaging (?).
- `Document/`: Like the "other" option.

Programming files:
- `lib/`
- `output/`
- `tmp/`
	One project style:
	- `src/`: Includes header files from some systems.
	- `resource/`
	- `test/`
	- `test-resource/`
	- `integration/`
	- `integration-resource/`
	- `output/dev/`: For compiled, transpiled or minimized programs.
	- `output/prod/`
	- `output/test/`
	- `output/integration/`


- `/README.md`
- `/LICENSE.md|COPYING|COPYING.LESSER`
- `/Content/` : Additional project’s files used in the creation process but unnecessary to make it working.
    - `Documents/`
    - `Logos/` : Created logo used in the project following [Logo](https://www.notion.so/Logo-f45bb860006d4fb1bb5cfd24b083680f?pvs=21) conventions.
        - `<project>_logo.png` : Mandatory file for the GitHub README.md or the projects listing on the website (Replaced by the blank one if wasn’t found ?).
        - `<project>_Large_logo.png` : Mandatory file for the GitHub README.md or the projects listing on the website (Replaced by the blank one if wasn’t found ?).
    - `UI/` : UI files and images used as placeholders.
    - `Fonts/` : Created/Downloaded fonts used in the project.
    - `Images/` : Edited/Downloaded images used in the project.
    - `Screenshots/<number>.png` : Project screenshots.
- `/bin/` : Binaries and scripts.
    - `lib/` : Libraries used by binaries, scripts or other libraries.
- `/<project>|src|src-<subproject>/` : Project sources.
- `/resource/` : Project resources.
    - `config/` : Configuration files.
    - `public/` : Web resources publicly shown (Only for web projects).
- `/test/` : Sub-project that test project sources.
    - `src/` : Test sources.
    - `resource/` : Test resources.
- `/out/` : Project build outputs (Should be ignored by git).
    - `<project>|(src|src-<subproject>)/` : Compiled project sources.
        - `prod/` : Builds ready for publish them into production; Usually a bundle/compressed file of (compiled) sources.
        - `dev/` : Compiled sources used in development process or to bundling them into a production ready build.
        - `public/` : Project web server entry point composed of copied/compiled/compressed sources (Only for web projects).
            - `resource/` : Copied web resources.
    - `test/` : Compiled test sources.
- `/doc/` : Generated or hand-written documentations.
- `/tmp/` : Temporary files (Should be ignored by git).
    - `project/` : Project’s temporary files.
    - `test/` : Test’s temporary files.

## Links

## References
1. J. van Zyl, “Introduction to the standard directory layout – maven”, Apache.org, 09-Mar-2014. [Online]. Available: https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html. [Accessed: 17-Nov-2024].

https://stackoverflow.com/questions/5178334/folder-structure-for-a-node-js-project
https://docs.gradle.org/current/userguide/organizing_gradle_projects.html
https://stackoverflow.com/questions/2360734/whats-a-good-directory-structure-for-larger-c-projects-using-makefile
https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p1204r0.html
https://palikar.github.io/posts/cmake_structure/
https://cliutils.gitlab.io/modern-cmake/chapters/basics/structure.html
https://github.com/luarocks/lua-style-guide
https://doc.rust-lang.org/cargo/guide/project-layout.html
https://docs.php.earth/faq/misc/structure/