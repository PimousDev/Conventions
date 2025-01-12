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
No plurial: Because we could put it everywhere, so we choosed to not use it.

### Project structure
- `/`: _Project root._

	Project and git files in UpperCase:
	- `project.yaml`: Project definition file<sup>4;6;9;10</sup> (Used by [ProjectUtils](https://www.github.com/PimousDev/ProjectUtils); Any other file from a project/dependency manager would fit).
	- `README.md`
	- `LICENSE.md|COPYING|COPYING.*`: Depends on the licensing authority.
	- `.gitignore`

	Non-programming files (Pimous Dev. specific) in PascalCase:
	- `Content/`
		- `Logo/`: See [#Design/Logo](/conventions/design/logo.md).
			- `<project>_logo.png` : Mandatory file for projects listing.
			- `<project>_Large_logo.png` : Mandatory file for the GitHub README.md and project viewing.
		- `Diagram/`: Static and Dynamic UML.
		- `UI/`: UX (Wireframes), UI and placeholder images.
		- `Screenshot/<number>.png`: Project screenshots.
		- `Font`: Some fonts created for/used in the project.
		- `Image/`: Some raw/edited images created for/used in the project.
		- `Video/`: Some raw/edited videos created for/used in the project.
		- `Archive/`: Raw archives or special packaging (?).
		- `Document/`: Like the "other" option.

	Programming files in CamelCase:
	- `bin/`: Binaries and scripts<sup>7;10</sup>.
	- `lib/`: Libraries that can't be downloaded automatically<sup>6</sup>; may be files or folders.
	- `inc/`: Library headers that can't be downloaded automatically<sup>6</sup>; may be files or folders.
	- `<subproject>/`: _One or more subprojects<sup>2;6;8</sup>._
		- `src/`: Subproject sources<sup>2;8;10</sup>, including headers<sup>5</sup>.
		- `resource/`: Subproject resources<sup>2;8</sup> (Optional).
			- `(style|image|script)/`: Raw web publicly available resources<sup>3</sup> (Only for web subprojects).
			- `public/`: Web resources publicly available<sup>3;10</sup> (Only for web subprojects).
		- `test/`: Subproject tests<sup>2;8</sup>, including headers<sup>5</sup>.
		- `test-resource/`: Subproject test resources<sup>2;8</sup> (Optional).
		- `btest/`: Subproject benchmark test sources<sup>2;8;9</sup>, including headers<sup>5</sup> (Optional).
		- `btest-resource/` Subproject benchmark test resources<sup>2;8;9</sup> (Optional).
		- `itest/`: Subproject integration test sources<sup>2</sup>, including headers<sup>5</sup> (Optional).
		- `itest-resource/` Subproject integration test resources<sup>2</sup> (Optional).
	- `doc/`: Generated or hand-written documentations.
	- `out/`: Project build outputs (Should be ignored by git)<sup>11</sup>.
		- `<subproject>/`: _One or more subproject outputs._
			- `dev/`: Compiled, transpiled and/or rearranged sources and resources.
				- `public/(style|image|script)/`: Compiled, transpiled and/or rearranged web publicly available resources<sup>3;10</sup> (Only for web subprojects).
			- `prod/`: Executable(s) and/or compressed/minimized file(s) ready to be released<sup>11</sup>.
				- `public/(style|image|script)/`: Minimized and/or compressed web publicly available resources<sup>3;10</sup> (Only for web subprojects).
			- `test/`: Compiled, transpiled and/or rearranged tests and test-resources<sup>11</sup>.
			- `itest/`: Compiled, transpiled and/or rearranged integration tests and itest-resources.

### Docker structure
- `/`: _Root filesystem._

## Links
- [Design/Logo](/conventions/design/logo.md)

## References
1. Wikipedia contributors, “Convention over configuration”, Wikipedia, The Free Encyclopedia, 02-Apr-2024. [Online]. Available: https://en.wikipedia.org/w/index.php?title=Convention_over_configuration&oldid=1216958188.
2. J. van Zyl, “Introduction to the standard directory layout - maven”, Apache.org, 09-Mar-2014. [Online]. Available: https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html. [Accessed: 17-Nov-2024].
3. schaermu, “Folder structure for a Node.js project”, Stack Overflow. [Online]. Available: https://stackoverflow.com/a/5193206/23208036. [Accessed: 11-Jan-2025].
4. “Organizing Gradle Projects”, Gradle.org. [Online]. Available: https://docs.gradle.org/current/userguide/organizing_gradle_projects.html. [Accessed: 11-Jan-2025].
5. “Canonical Project Structure”, Open-std.org. [Online]. Available: https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p1204r0.html. [Accessed: 12-Jan-2025].
6. “The optimal CMake project structure”, Github.io, 10-Apr-2019. [Online]. Available: https://palikar.github.io/posts/cmake_structure/. [Accessed: 12-Jan-2025].
7. Olivine Labs, "Lua Style Guide", Github.com, 8-Jan-2013. [Online]. Available: https://github.com/Olivine-Labs/lua-style-guide. [Accessed: 12-Jan-2025].
8. “Project layout - The Java Plugin”, Gradle.org. [Online]. Available: https://docs.gradle.org/current/userguide/java_plugin.html#sec:java_project_layout. [Accessed: 12-Jan-2025].
9. “Package Layout - The Cargo Book”, Rust-lang.org. [Online]. Available: https://doc.rust-lang.org/cargo/guide/project-layout.html. [Accessed: 12-Jan-2025].
10. “How to choose a PHP project directory structure?”, PHP.earth. [Online]. Available: https://docs.php.earth/faq/misc/structure/. [Accessed: 12-Jan-2025].
11. “Compile and build applications with IntelliJ IDEA”, IntelliJ IDEA Help. [Online]. Available: https://www.jetbrains.com/help/idea/compiling-applications.html. [Accessed: 12-Jan-2025].

https://refspecs.linuxfoundation.org/FHS_2.3/fhs-2.3.html