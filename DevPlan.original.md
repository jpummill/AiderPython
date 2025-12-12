# title: Create User Information API
### Overview
- Create a user information API

### Mandatory Rules
- Always refer to ./CONVENTION.md and adhere to the rules.
  - Especially, strictly follow the phpdoc specifications for documentation rules.

### Development Goals
- Implementation of userController.php is complete.
- Implementation of userUseCase.php is complete.
- All unit tests pass.

### Context for Generative AI Training
#### UnitTest: userTest
- Develop using TDD, so create tests first.
- The reference file for creating unit tests is `/path/to/userControllerTest.php`.
  - Use DatabaseTransactions.
  - Create test data.

#### Model: Necessary model classes
Refer to model classes under the /path/to/Eloquents directory.
- UserModel.php
- XxxModel.php

#### Screenshot: path/to/file
- /path/to/xxx.png
<!-- Aider can add images as context with the /paste command, so use as needed -->

### Process
#### process1: Create necessary files

When creating files, include phpdoc for classes, methods, class properties, and constants.
For phpdoc conventions, refer to CONVENTION.md#Documentation Rules.

- [ ] Create /path/to/UserController.php
  - [ ] Refer to @ref /path/to/YyyController.php
- [ ] Create /path/to/UserUseCase.php
  - [ ] Create get() method
    - [ ] Use Eloquent's UserModel
    - [ ] Extract only usernames after retrieval

#### process2: Follow-up
##### sub1: Refactor UserController.php
- [ ] Refactor the code.

##### sub2: Code correction
- [ ] Update phpdoc for context target files.
  - [ ] Reflect the latest method arguments in @param.
  - [ ] Reflect the latest method return values in @return.
- [ ] Reflect the latest method exceptions in @throws.
