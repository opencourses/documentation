# Documentation

Open Courses is an open education project with the goal of sharing knowledge related to the  Computer Engineering and Electronic Engineering fields through an online platform created, managed and populated by IEEE-HKN students all over the world, following the rules defined in the project manifesto. The target of this platform are computer engineering students and Informatics and Electronic enthusiasts that aim at learning something new in a fast, incremental and well-structured way. The project will be developed using well-known open source solutions to reduce the creation and maintenance costs and exploit collaboration potentialities.

## Implementation Details

The solution has been designed to be sustainable and easy to manage, based on open source solutions and modern concepts that allows reducing developing and maintainability costs. The whole solution will be based on two main tools:

 - Git repositories;
 - Statically generated pages.

Each subject’s content will be stored in a Git repository. GitLab or GitHub can be used to manage a repository for each subject, assigning contributors and repository owners with different access level, as already possible with these platforms. This will allow to use all the tools specific to software engineering also to this specific topic, allowing to report problems in a repository using the concept of "issues", adding new exercises and learning material using the "pull-requests", thus allowing an easy review process able to check the correctness of each new added material. Moreover, the use of specific automation tools (such as git hooks) allows to reduce the review effort, using scripts able to report directly the non conformance to the defined repository structure.

The added material can be accessed by the students directly using the git repository. However, to increase the accessibility even to users not able to work with git and also allow a more personalized user interface to present the material, static web pages will be generated for each repository. This concept is widely used on GitHub and known as GitHub Pages. However, it is possible to use open source solutions such as Jekyll to create static pages and store them on a proprietary web server. Having static pages highly reduces the maintenance costs and effort compared to a dynamic website. It periodically requiring to regenerate them to be conformant with the subject repository, but avoids to deal with security issues or possible malfunctioning of the dynamically generated pages.

All the previously highlighted solutions are open source, free and suitable for working on big projects in a very well-structured way; they are typically used for big software engineering projects and will perfectly fit also in this case, where multiple contributors are required and the added content must pass through a review process.

## How to contribute?

Everyone is free to contribute to the project adding new material, following a new course or just modifying or providing feedback on an already present course. 

The contributions will be managed using GitHub. There are three general cases:
- **Add or modify material on an already present course:** this must be done by means of pull-requests, an easy way to contribute to a GitHub repository. To open a pull-requrest you need first to fork the course repository in your GitHub account, clone it on your local computer to make the modifications, push them to your fork and from them make the pull-request. When you are opening the pull-request please specify exactly the goal of your work, following the contribution template present in the repository.
- **Provide feedback and open a discussion on an already present course:** if you want to discuss an exercise or the content of course you should open an issue in that specific course repository. When writing the issue you should follow the issue template provided in the repository, to make sure you target all the informations needed to make a constructive discussion.
- **Start a new course:** to start a new course you should discuss it with the project mantainers using the dedicated slack channel. You can access the slack channel at opencourses.slack.com, where we will have a channel for each course and a generic channel to make general discussions on the project

## Course structure

Each course should be structured according to the following file list:

 - Readme.md: a file indicating the 
 - Contributors.md
 - Licence.md
 - Requirements.md
 - Exercises.md lista autogenerata
 - open-courses.sh (script di management de progetto)
 - Exercises/exercise.sh
 - Exercises/exercise_01
 - Readme.md generato dal toml o dal json in automatico
 - exercise.toml | json file parsabile contenente key value pair dell’esercizio
 - Various files

## How to manage contributions?
Most of the maintainers’ work is related to periodical verification of the system status, considering the courses material available, the consistency of the exercises, the correct generation of the supporting files and the static web pages.

Whenever a new contribution is submitted, either using pull requests or issues, the system should automatically analyze the related data thus enabling automatic characterization and management of the contribution itself.

Contributions must be reviewed to check:
associated tags are relevant;
format is compliant;
content doesn’t contain vulgarity etc.
it adds something new and valuable to the repository

Some of these tasks can be carried on automatically:
format verification;
content semantic control
but all the others require user intervention.

Even though static web pages are automatically generated, the page layout, the displayed content order, the connecting paragr

