# Code Review Developer Guide

# 开发者代码审查手册

## Introduction {#intro}

## 简介

A code review is a process where someone other than the author(s) of a piece of
code examines that code.

代码审查是除了代码作者外的其他人检查代码的过程。

At Google, we use code review to maintain the quality of our code and products.

在Google，我们使用代码审查来保持我们代码和产品的质量。

This documentation is the canonical description of Google's code review
processes and policies.

这个文档是对Google代码审查流程和政策的解读。



This page is an overview of our code review process. There are two other large
documents that are a part of this guide:

本页是代码审查的一个overview页面，代码审查规范还包含下面两个文档：

-   **[How To Do A Code Review](reviewer/index.md)**: A detailed guide for code
    reviewers.
-   **[The CL Author's Guide](developer/index.md)**: A detailed guide for
    developers whose CLs are going through review.

-   **[代码审查者手册](reviewer/index.md)**
-   **[代码作者手册](developer/index.md)**

## What Do Code Reviewers Look For? {#look_for}

## 代码审查用什么内容

Code reviews should look at:

-   **Design**: Is the code well-designed and appropriate for your system?
-   **Functionality**: Does the code behave as the author likely intended? Is
    the way the code behaves good for its users?
-   **Complexity**: Could the code be made simpler? Would another developer be
    able to easily understand and use this code when they come across it in the
    future?
-   **Tests**: Does the code have correct and well-designed automated tests?
-   **Naming**: Did the developer choose clear names for variables, classes,
    methods, etc.?
-   **Comments**: Are the comments clear and useful?
-   **Style**: Does the code follow our
    [style guides](http://google.github.io/styleguide/)?
-   **Documentation**: Did the developer also update relevant documentation?

代码审查是用来审查以下内容：

-   **设计**: 代码是否经过良好设计，是否符合你的系统
-   **功能性**: 代码是否满足作者的意图，代码的行为对的使用者是否友好
-   **复杂性**: 代码可以更简化么，其他的代码开发者将来可以轻易的理解代码么
-   **测试**: 代码是否是正确的，是否有经过良好设计的自动化测试
-   **命名**: 是否为变量、类、方法等选择了合适的名字
-   **注释**: 注释是不是清晰有用的
-   **风格**: 是否符合代码风格的约束
-   **文档**: 是否开发者更新了对应的文档

See **[How To Do A Code Review](reviewer/index.md)** for more information.

阅读，**[如何做代码审查](reviewer/index.md)** 获取更多内容。

### Picking the Best Reviewers {#best_reviewers}

### 选择最好的代码审查者

In general, you want to find the *best* reviewers you can who are capable of
responding to your review within a reasonable period of time.

通常，您希望找到能够在合理的时间内回复您的评论的最佳评论者。

The best reviewer is the person who will be able to give you the most thorough
and correct review for the piece of code you are writing. This usually means the
owner(s) of the code, who may or may not be the people in the OWNERS file.
Sometimes this means asking different people to review different parts of the
CL.

最好的审查者是能够为您编写的代码片段提供最彻底、最正确的审查的人。

If you find an ideal reviewer but they are not available, you should at least CC
them on your change.

如果找到理想的审查者，但没有可用的审查者，则至少应在更改时使用抄送。

### In-Person Reviews {#in_person}

### 一对一审查

If you pair-programmed a piece of code with somebody who was qualified to do a
good code review on it, then that code is considered reviewed.

You can also do in-person code reviews where the reviewer asks questions and the
developer of the change speaks only when spoken to.

## See Also {#seealso}

-   [How To Do A Code Review](reviewer/index.md): A detailed guide for code
    reviewers.
-   [The CL Author's Guide](developer/index.md): A detailed guide for developers
    whose CLs are going through review.
