# NEXT RFC

## 什么是 RFC ?

“RFC”（征求意见）流程旨在为新功能进入 NEXT 提供一致且受控的方法。

许多更改，包括错误修复和文档改进，都可以通过正常的 GitHub 拉取请求工作流程实施和审查。

虽然有些更改是“重大的”，但我们要求这些更改经过一些设计过程，并在 NEXT 核心团队和社区之间产生共识。

## RFC 生命周期

一个 RFC 经历以下阶段：

- **Pending：**当 RFC 作为 PR 提交时。
- **Active：**当 RFC PR 被合并并正在实施时。
- **Landed：**当 RFC 提议的更改在实际版本中发布时。
- **Rejected：**当一个 RFC PR 被关闭而不被合并时。

[待处理的 RFC 列表](https://github.com/nx-space/rfcs/pulls)

## 何时遵循此流程

如果您打算对下面列出的项目之一进行“重大”更改，则需要遵循此过程：

- [NEXT Core](https://github.com/nx-space/core)

我们正在限制这些 repos 的 RFC 流程，以便以更易于管理的方式测试该流程，并可能 `NEXT` 在未来将其扩展到组织下的更多项目。目前，如果您希望对其他项目提出更改建议，请使用它们各自的 issues 功能进行操作。

构成“重大”变化的内容正在根据社区规范不断发展，但可能包括以下内容：

- 创建新的 API
- 更改现有 API 的功能或行为
- 删除已作为发布渠道的一部分提供的功能
- 引入新的惯用用法或约定，即使它们不包括对 NEXT 本身的代码更改。

有些更改不需要 RFC：

- 严格改进客观、数字质量标准的添加（加速，更好的浏览器支持）
- 修正客观上不正确的行为
- 改写、重组或重构
- 添加或删除警告
- 只有其他 NEXT 实现者才可能*注意到*添加，而 NEXT 用户不可见。

如果您在未通过 RFC 流程的情况下提交拉取请求以实现新功能，则可能会先让您提交 RFC 。

## 为什么你需要这样做

很高兴您正在考虑对 NEXT 提出新功能或更改建议，感谢你的贡献！然而，随着 NEXT 的慢慢发展，我认为我们需要更加重视稳定性，因此必须仔细考虑我们所做的每一个可能影响最终用户的更改的影响。另一方面，NEXT 目前已经进入了一个 API 相对稳定的阶段，我们希望开始有意识地防止新 API 的进一步复杂性。

对于提出更改只是为了解决他们刚刚遇到的特定问题的用户来说，这些限制和权衡可能不会立即显而易见。RFC 流程作为一种方式来指导您在对 NEXT 进行更改时完成我们的思考过程，以便我们在讨论为什么或为什么不应该进行这些更改时可以在同一页面上。

## 提交前收集反馈

在深入了解 RFC 所需的 API 设计细节级别之前，通常获得有关你的概念的反馈会很有帮助。**你可以在这个 repo 上打开一个 issue 来开始一个高层次的讨论**，目标是最终制定一个具有特定实现设计的 RFC pull request

## 如何贡献 RFC

1. 根据此 repo 中的模板 （`0000-template.md`）撰写新的功能提案，然后对此仓库发起 PR
   - 注意细节信息：**没有提供令人信服的动机、展示对设计影响的理解或对缺点或替代方案不现实的 RFC 通常不受欢迎**。
   - 记得总结好你的提案内容，凝聚成为讨论 与 PR 的标题
2. 在[ Issues ](https://github.com/nx-space/rfcs/issues)中打开一个新的议题，并且将 Label 设置为 “rfc”，其他 Label 交给核心团队操作

## 实施 RFC

RFC 的作者没有义务实施它。当然，欢迎 RFC 作者（与任何其他开发人员一样）在 RFC 被接受后发布实现以供审查。

如果有的话，一个活跃的 RFC 应该列出实现 PR 的链接。对实际实现的反馈应该在实现 PR 而不是原始的 RFC PR 中进行。

如果您有兴趣为“活动”RFC 的实现工作，但不能确定其他人是否已经在工作，请随时询问（例如，通过对相关问题发表评论）。

**NEXT 的 RFC 流程大量来自于 [Vue RFC 流程](https://github.com/vuejs/rfcs/blob/master/README.md)**
