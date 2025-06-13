|alias|tag|command|description|
|:-|:-|:-|:-|
|ga|selector|git add|用于将工作目录中的更改暂存，以便进行下一个提交。它可以将新文件、修改过的文件或已删除的文件添加到暂存区。一旦更改被暂存，它们将被包括在下一个提交中|
|glo|viewer|git log|显示当前分支的提交历史。它提供了一系列提交记录，以及提交哈希、作者、日期和提交信息等信息|
|gi|generator|.gitignore|一个纯文本文件，用于在 Git 仓库中指定 Git 应该忽略的文件和目录。列在 .gitignore 中的文件和目录将不会被 Git 跟踪，这意味着它们的更改不会被暂存或提交。这对于排除临时文件、构建产物、秘密密钥或任何其他不应纳入版本控制的文件非常有用|
|gd|viewer|git diff|显示工作目录与索引（已暂存文件）之间的差异，或显示提交、分支等之间的差异。它提供对所做更改的逐行查看|
|gso|viewer|git show|显示特定提交的信息，包括提交信息、作者和在该提交中所做的更改。您可以指定提交哈希、分支名或标签以查看不同的版本|
|grh|selector|git reset HEAD <file>|取消暂存指定的文件，将其有效地移回工作目录，而不会丢失更改。它用于重新指定下一个提交中暂存的内容|
|gcf|selector|git checkout <file>|将指定的文件恢复到当前分支的最后提交状态。对此文件在最后提交后所做的任何更改都会丢失|
|gcb|selector|git checkout <branch>|切换当前工作分支到指定的分支，更新工作目录以匹配该分支的最后提交状态|
|gbd|selector|git branch -D <branch>|强制删除指定的分支，即使该分支有未合并的更改。这对于清理不再需要的分支非常有用|
|gct|selector|git checkout <tag>|检出仓库中的特定标签。这将使工作目录进入一个“分离的 HEAD”状态，在历史记录中的该时刻|
|gco|selector|git checkout <commit>|在“分离的 HEAD”状态下检出指定的提交，允许您查看该提交时的项目状态，而不移动分支指针|
|grc|selector|git revert <commit>|创建一个新的提交，用于撤销指定提交中所做的更改。这是一种安全地从您的项目历史中删除更改的方法|
|gss|viewer|git stash|临时保存您在工作目录中尚未准备好提交的修改。您可以稍后取回这些更改|
|gsp|selector|git stash push|暂存您的更改，您可以选择添加信息或命名暂存。这允许您在不提交的情况下保存工作，类似于 `git stash`|
|gclean|selector|git clean|从工作目录中删除未跟踪的文件。可以使用选项来指定是否仅删除目录或仅删除文件|
|gcp|selector|git cherry-pick|将特定提交中的更改应用到您当前的分支。这允许您从另一个分支中包含特定的更改，而无需合并整个分支|
|grb|selector|git rebase -i|开始一次交互式变基，允许您编辑、合并或重新排列当前分支中的提交。这对于清理提交历史非常有用|
|grl|viewer|git reflog|显示影响当前仓库的所有引用（或操作）的日志，允许您恢复丢失的提交或分支|
|gbl|selector|git blame|显示文件中每行的最后修改信息，包括提交哈希和作者。这对于跟踪谁做了特定更改非常有用|
|gfu|selector|git commit --fixup && git rebase -i --autosquash|以“fixup”信息提交更改，指示该提交应在交互式变基期间合并至特定的先前提交。`--autosquash` 选项在变基过程中自动重新排列提交以执行 fixup|
|gsq|selector|git commit --squash && git rebase -i --autosquash|以“squash”信息提交更改，指示该提交应在变基期间与先前的提交合并。与前一个命令一样，`--autosquash` 有助于在变基过程中自动重新排列提交|
|grw|selector|git commit --fixup=reword && git rebase -i --autosquash|创建一个修复提交，同时在交互式变基期间更改指定提交的提交信息。该提交将与指定提交合并，其信息将根据 fixup 更新|
