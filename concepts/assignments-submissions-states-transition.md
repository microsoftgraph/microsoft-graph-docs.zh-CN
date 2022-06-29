---
title: 分配和提交的状态、转换和限制
description: 了解流程流程期间分配和提交状态的更改，以及涉及 Microsoft Graph 中的教育 API。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 479acbfa696c17d63e31c3298f10bedcfae906d9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437056"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Microsoft Graph 中分配和提交的状态、转换和限制

作业和提交是教师与学生行动互动的重要组成部分。 本文介绍流程流程期间分配和提交状态的更改，以及涉及 Microsoft Graph 中的教育 API。

## <a name="assignment-states-and-transitions"></a>分配状态和转换

作业表示分配给课堂中学生或团队成员的任务或工作单位，作为学习的一部分。 只有教师或团队所有者才能创建、复制或计划作业。 这些操作会影响分配状态。 下表列出了可用于更改状态的分配状态和 API。 

| 状态 | 说明 | REST API 调用 | 可用于编辑的功能 |
|:--|:--|:--|:--|
| Draft | 从现有分配创建或复制新分配时的初始状态。 | `POST /education/classes/{id}/assignments` | 资源、类别、红宝石 |
| Published | 分配给分配给每个分配的学生时，后台处理状态。 | `POST /education/classes/{id}/assignments/{id}/publish` | |
| Scheduled | 教师计划在将来发布作业时的状态。 | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` | 资源、类别、红宝石 |
| 已分配 | 完成发布后，作业将移到“分配”状态，可供学生使用。 | `POST /education/classes/{id}/assignments/{id}/publish` | 提交 |
| Pending | 从现有分配复制新分配时的后台处理状态。 | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` | |

下图显示了分配可能发生的状态转换。

![分配状态转换关系图](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>如何验证分配是否已发布

调用方必须使用 [GET 分配](/graph/api/educationassignment-get.md) 操作来检查当前分配状态并验证发布过程是否成功。

### <a name="assignment-state-transitions-based-on-the-allowed-actions"></a>基于允许的操作的分配状态转换

| 当前分配状态 | 新操作 | 新状态 |
|:--|:--|:--|
| Draft | 教师安排作业 | Scheduled |
| Draft | 发布 | Published |
| Draft | 编辑 | Draft |
| Draft | 丢弃 | |
| Published | 发布完成 | 已分配 |
| Published | 发布失败 | Draft |
| Published | 丢弃 | |
| Scheduled | 达到截止日期 | Published |
| Scheduled | 取消计划 | Draft |
| Scheduled | 安排 | Scheduled |
| 已分配 | 丢弃 | |
| Pending | 复制已完成 | Draft |
| Pending | 丢弃 | |

> [!NOTE]
> 不允许表中未列出的任何操作和状态转换。

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>通过分配 API 调用同步与异步操作

下表提到影响分配状态和操作类型的 API 调用。

同步操作一次执行一次，只有完成一个操作后，才能启动以下操作，并返回结果，直到最后一个操作完成。 使用异步操作时，操作将启动，另一个操作可以在上一个操作完成之前运行。 异步操作执行一些后台活动，调用方必须轮询才能获得结果。

| API | 同步或异步 | 获取最新状态的机制 |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | 投票 |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | 投票 |
| `POST /education/classes/{id}/assignments` | Async | 投票 |

## <a name="submission-states-and-transitions"></a>提交状态和转换

提交表示单个 (或组) 用于分配的资源。 提交由分配拥有，并在发布分配时自动创建。

状态是提交中的只读属性，根据学生和教师的操作进行更改。

| 状态 | 说明 | REST API 调用 |
|:--|:--|:--|
| Working | 创建提交后的初始状态。 | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | 这发生在学生上交作业之后。 | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| 返回 | 教师将作业返回给学生后。 | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |
| 分配 | 教师将作业返回给学生进行修订后。 | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` |

下图显示了状态转换流。

![提交状态转换关系图](images/states-transitions/diagram-submissions.PNG)

### <a name="submission-state-transitions-based-on-allowed-actions"></a>基于允许的操作的提交状态转换

| 当前提交状态 | 新操作 | 新状态 |
|:--|:--|:--|
| Working | 交入 | Submitted |
| Working | 用于修订的返回 | 分配 |
| Working | Return | 返回 |
| Submitted | 撤消入门 | Working |
| Submitted | Return | 返回 |
| Submitted | 用于修订的返回 | 分配 |
| 返回 | 交入 | Submitted |
| 返回 | Return | 返回 |
| 返回 | 用于修订的返回 | 分配 |
| 分配 | 交入 | Submitted |
| 分配 | Return | 返回 |
| 分配 | 用于修订的返回 | 分配 |

> [!NOTE]
> 不允许表中未列出的任何操作和状态转换。

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>通过提交 API 调用同步与异步操作

下表列出了影响提交状态和操作类型的 API 调用。

在这种情况下，所有调用都是异步调用，这意味着操作开始，另一个操作可以在第一个操作完成之前启动。 异步操作执行一些后台活动，调用方必须轮询才能获得结果。  

| API | 同步或异步 | 获取最新状态的机制 |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` | Async | 投票 |

### <a name="limits"></a>限制

以下限制适用于所有 API 调用：

* 教师的最大作业和提交资源数为 10，学生为 10。
* 资源允许的最大大小为 50 MB 或 10 个资源。
* 限制适用;有关详细信息，请参阅 [Microsoft Graph 限制指南](/graph/throttling)。
