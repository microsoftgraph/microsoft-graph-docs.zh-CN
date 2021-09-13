---
title: Microsoft Graph 中作业和提交状态、转换和Graph
description: 本文介绍了进程流期间作业和提交状态的变化，以及涉及 Microsoft Graph API。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 83589986cd0c490f4947744896665244a8de3633
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117667"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Microsoft Graph 中作业和提交状态、转换和Graph

作业和提交是教师和学生操作之间交互的重要部分。 本文介绍了进程流期间作业和提交状态的变化，以及涉及 Microsoft Graph API。

## <a name="assignment-states-and-transitions"></a>工作分配状态和转换

作业表示作为学习的一部分分配给课堂中的学生或团队成员的任务或工作单位。 只有教师或团队所有者才能创建、复制或安排作业。 这些操作会影响工作分配状态。 下表列出了可用于更改状态的工作分配状态和 API。 

| 状态 | 说明 | REST API 调用 |
|:--|:--|:--|
| Draft | 从现有工作分配创建或复制新工作分配时的初始状态。 | `POST /education/classes/{id}/assignments` |
| 已发布 | 将作业分发给每个分配的学生时的背景处理状态。 | `POST /education/classes/{id}/assignments/{id}/publish` |
| Scheduled | 教师计划将来发布作业时的状态。 | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` |
| 已分配 | 完成发布后，作业将移动到"已分配"状态，并且可供学生使用。 | `POST /education/classes/{id}/assignments/{id}/publish` |
| 挂起 | 从现有工作分配复制新工作分配时的背景处理状态。 | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` |

下图显示了工作分配可发生的状态转换。

![工作分配状态转换图](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>如何验证工作分配是否发布
调用方必须使用 GET 分配操作来检查当前分配状态，并验证发布过程是否成功。

### <a name="assignments-states-transitions-based-on-the-allowed-actions"></a>工作分配根据允许的操作状态转换
| 当前工作分配状态 | Action | 新状态 |
|:--|:--|:--|
| Draft | 教师设置截止日期。 | Scheduled |
| Draft | 发布 | 已发布 |
| Draft | 已编辑 | Draft |
| Draft | 已放弃 | | 
| 已发布 | 发布完成 | 已分配 |
| 已发布 | 已放弃 | |
| Scheduled | 到达截止日期 | 已发布 |
| Scheduled | 取消计划 | Draft |
| Scheduled | 重新计划 | Scheduled |
| 已分配 | 已放弃 | |
| 挂起 | 复制已完成 | Draft |
| 挂起 | 已放弃 | |   

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>通过分配 API 调用同步与异步操作
下表提及了影响分配状态和操作类型的 API 调用。

同步操作一次执行一个，并且只有在完成一个操作后，才能开始以下操作，并返回结果，直到最后一个操作完成。 使用异步操作，该操作将启动，并且另一个操作可以在前一个操作完成之前运行。 异步操作执行一些后台活动，调用方必须轮询才能获得结果。

| API | 同步或异步 | 获取最新状态的机制 |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | 投票 |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | 投票 |
| `POST /education/classes/{id}/assignments` | Async | 投票 |

## <a name="submission-states-and-transitions"></a>提交状态和转换

提交表示单个用户或组 (为) 启用的资源。 提交归工作分配所有，在发布工作分配时自动创建。

状态是提交中的只读属性，并且根据学生和教师的操作进行更改。
 

| 状态 | 说明 | REST API 调用 |
|:--|:--|:--|
| Working | 创建提交后的初始状态。 | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | 在学生打开作业后，会发生此情况。 | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| 已返回 | 教师将作业返回给学生后。 | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |

下图显示了状态转换流。

![提交状态转换图](images/states-transitions/diagram-submissions.PNG)

### <a name="submissions-states-transitions-based-on-allowed-actions"></a>提交状态基于允许的操作进行转换
| 当前提交状态 | Action | 新状态 |
|:--|:--|:--|
| Working | 启用 | Submitted |
| Working | Return | 已返回 |
| Submitted | 撤消启用 | Working |
| Submitted | Return | 已返回 |
| 已返回 | 启用 | Submitted |

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>通过提交 API 调用同步与异步操作
下表列出了影响提交状态和操作类型的 API 调用。

在这种情况下，所有调用都是异步的，这意味着该操作将启动，并且另一个操作可以在第一个操作完成之前启动。 异步操作执行一些后台活动，调用方必须轮询才能获得结果。  

| API | 同步或异步 | 获取最新状态的机制 |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | 投票 |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | 投票 |

### <a name="limits"></a>限制
以下限制适用于所有 API 调用：

* 教师的最大作业数和提交资源数为 10，学生为 10。
* 资源允许的最大大小为整体 50 MB 或 10 个资源。
* 限制适用;有关详细信息，请参阅[Microsoft Graph限制指南](https://docs.microsoft.com/graph/throttling)。
