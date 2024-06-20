# Open-sourcing Tips / Tutorial #2

**Table of Contents**
* [Licensing](#licensing)
* [Adding a README file](#readme)
* [Keep your code clean](#clean-code)

**Licensing** <a name="licensing"></a>

Licensing your code is an important step in open-sourcing,
as well as understanding other repositories licenses. The recommended
resource for getting started with licensing is 
[choosealicense.com](https://choosealicense.com). Here are the main
take aways and my opinon:

* **Be aware of your dependencies' licenses:** This is important because
you need to ensure that you are using their software according to their
expectation. Additionally, this will help guide your decision in your own
licensing. For example, if your project relies on a heavily restricted dependency
you might not be allowed to specify a less restrictive license for your own
project. Or additionally, if you would like to contribut code to a community
such as npm, then you must use a specific license (MIT for npm)

* **No license means no go:** If a creative work (such as code) does not specify a
license agreement then it is exclusive by default. If a dependency in your program
does not have a license then you should ask the maintainer of the dependency to
provide one, or specify the terms of use for their dependency. This will avoid
conflicts and potentially the take-down of your code from public domain.

* **Best license for research (IMO):** In my opinion, the best license for
research related work is the [GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/) 
license. This covers the user from liability and warranty. Additionally, it
requires that software based on your code also discloses source-code and uses
the same license. Therefore, this license is the most permissive while requiring
that advancements on the code are also made open-source. This is the license used 
by Linux, Bash, amongst other popular open-source software.

**Adding a README file** <a name = "readme"></a>

The README.md file is an essential part of any open-source project. It is the intro
document to your project. Here is a common structure that I like to follow for my README
files:

1. **General info:** Title, main contributor, link to related paper/s.
2. **Introduction:** what is this project about?
3. **Installation:** How do I get started? Provide specific commands used to clone, install dependencies, and build project.
4. **Basic usage:** Commands, or basic script to run your project/use the API.

This format is suitable for small projects, however if you are working on a big project with multiple contributors and a lots of functionalities; You may consider a more dynamic structure for your README. For example, only keep the general info in the readme, and then provide links to other files with information about installation, example usage, contribution guidelines, etc.

**Keep your code ✨*clean*✨** <a name="clean-code"></a>

Keeping your code clean is incredibly important whenever you want to publish
code for others to use, modify, or contribute to. However, this is something that
comes with practice, what is more, different programming languages have different
definitions/standards for what constitutes as clean code. Personally, I have found
notable improvements in the way I write code ever since I started worrying about the
"cleanliness" of my code. When it comes to python programming, the best resource I can
recommend is the YouTube channel ["ArjanCodes"](https://www.youtube.com/@ArjanCodes).

Additionally, I would recommed becoming familiar with at least one styling guide for
your language. Google has publicly available [styling guides](https://google.github.io/styleguide/) for different languages in their code bases. In python, the standard 
(most common) styling guide is outlined in the [PEP #8 post](https://peps.python.org/pep-0008/) and it is commonly referred to as PEP8. However, most developers use
auto-formatters such as [black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html). 