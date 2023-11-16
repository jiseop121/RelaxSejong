# Git Commit Convention

## Commit Messages

### Message Structure

A commit messages consists of three distinct parts separated by a blank line: the title, an optional body and an optional footer. The layout looks like this:
```
type: Subject

body

footer
```
### The Type
|태그 이름| 설명                    |
|--|---------------------------|
|Feat | 새로운 기능을 추가할 경우          |
| Fix | 버그를 고친 경우               |
| Design | CSS 등 사용자 UI 디자인 변경 |
|!BREAKING CHANGE|커다란 API 변경의 경우|
|!HOTFIX|급하게 치명적인 버그를 고쳐야하는 경우|
|Style|코드 포맷 변경, 세미 콜론 누락, 코드 수정이 없는 경우|
|Refactor|프로덕션 코드 리팩토링|
|Comment|필요한 주석 추가 및 변경|
|Docs|문서를 수정한 경우|
|Test|테스트 추가, 테스트 리팩토링(프로덕션 코드 변경 X)|
|Rename|파일 혹은 폴더명을 수정하거나 옮기는 작업만인 경우|
|Remove|파일을 삭제하는 작업만 수행한 경우|

### The Subject
Subjects should be no greater than 50 characters, should begin with a capital letter and do not end with a period.<br>

Use an imperative tone to describe what a commit does, rather than what it did. For example, use **change**; not changed or changes.
### The Body
Not all commits are complex enough to warrant a body, therefore it is optional and only used when a commit requires a bit of explanation and context. Use the body to explain the **what** and **why** of a commit, not the how.<br>

When writing a body, the blank line between the title and the body is required and you should limit the length of each line to no more than 72 characters.
### The Footer
The footer is optional and is used to reference issue tracker IDs.

### Example Commit Message

```
Feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```

## Resources
[**Udacity Git Commit Message Style Guide**](https://udacity.github.io/git-styleguide/)

