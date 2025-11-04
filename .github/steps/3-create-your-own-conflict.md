<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 3: 动手创建一个合并冲突

_太棒了！你已经成功解决了一次合并冲突！ :tada:_

不过在 GitHub 上，**解决冲突后并不会自动完成合并**。 GitHub 会把你的修改保存成一次 **合并提交（merge commit）**。

当我们解决冲突时，GitHub 实际上执行的是一种叫 **反向合并（reverse merge）** 的操作。
也就是说，它会把 `main` 分支的改动合并进你的 `my-resume` 分支，而不是反过来。
这样只有 `my-resume` 分支会更新，你可以先在自己的分支上测试修改，确认没问题后再合并回 `main`。

现在，让我们来点 “挑战性的” 练习吧。

### :keyboard: 实操环节

为了方便练习，我们将人为的制造一次合并冲突。我们已经在 `main` 分支中新增了一个文件 **`references.md`**，并推送到了远程仓库，但还没有同步到你的 `my-resume` 分支。

1. 切换到 `my-resume` 分支。
2. 点击 **Add file** 下拉菜单，选择 **Create new file**。
3. 创建一个名为 `references.md` 的文件。
4. 在 `references.md` 文件中输入一些与 `main` 分支中不同的内容（这样才能产生冲突）。
5. 滚动到页面底部，为本次修改输入提交信息（commit message）。
6. 点击 **Commit new file** 按钮，确保选中 “**Commit directly to the `my-resume` branch**”。
7. 等待大约 20 秒后，刷新当前页面。[GitHub Actions](https://docs.github.com/en/actions) 会自动检测进度并跳转到下一步。