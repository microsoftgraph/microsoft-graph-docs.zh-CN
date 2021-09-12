---
title: 在 Microsoft Graph 中使用教育 API
description: Microsoft Graph 中的教育 API 可增强 Microsoft 365 资源和与教育情景（包括学校、学生、教师、课程和注册）相关的信息的数据。 这使你能够轻松地构建与教育资源集成的解决方案。
ms.localizationpriority: high
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 29d50f4628bbca80e7c40e032cc5d9010155f3b7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007241"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>在 Microsoft Graph 中使用教育 API

Microsoft Graph 中的教育 API 可增强 Microsoft 365 资源和与教育情景（包括学校、学生、教师、课程和注册）相关的信息的数据。 这使你能够轻松地构建与教育资源集成的解决方案。

教育 API 包含名单资源和作业资源，可用于与 Microsoft Teams 中的名单服务进行交互。可以使用这些资源管理学校名单。

## <a name="authorization"></a>授权

若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。 有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](/graph/auth/)。 你的应用还需要具有相应的权限。 有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>请求学校 IT 管理员许可的应用权限

若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。 仅能授权许可一次，除非权限更改。 在管理员许可后，就会为租户中的所有用户预配应用。

若要显示许可对话框，请执行以下 REST 调用。

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| 参数   | 说明                                                               |
| :---------- | :------------------------------------------------------------------------ |
| Tenant      | 学校的租户 ID。 使用完整 ID，其中包含 onmicrosoft.com。 |
| clientId    | 应用的客户端 ID。                                                     |
| redirectUrl | 应用重定向 URL。                                                         |

## <a name="rostering"></a>Rostering

借助名册 API，可以从学校的 Microsoft 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。 API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。 支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。 这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。 此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。

可以使用名册 API 让应用用户了解：

- 我是谁
- 我参加或教学的课程
- 我需要做什么以及完成时间

名册 API 提供以下关键资源：

- [educationSchool](educationschool.md) - 表示学校。
- [educationClass](educationclass.md) - 表示学校的课程。
- [educationTerm](educationterm.md) - 表示学年的指定部分。
- [educationTeacher](educationteacher.md) - 表示主要角色为“教师”的用户。
- [educationStudent](educationstudent.md) - 表示主要角色为“学生”的用户。

名册 API 支持以下方案：

- [列出所有学校](../api/educationschool-list.md)
- [列出所教授课程的学校](../api/educationclass-list-schools.md)
- [为用户列出学校](../api/educationuser-list-schools.md)
- [获取所有课程](../api/educationclass-list.md)
- [获取学校的课程](../api/educationschool-list-classes.md)
- [为用户列出课程](../api/educationuser-list-classes.md)
- [将课程添加到学校](../api/educationschool-post-classes.md)
- [获取课程的学生和教师](../api/educationclass-list-members.md)
- [将成员添加到课程](../api/educationclass-post-members.md)
- [列出课程的教师](../api/educationclass-list-teachers.md)
- [获取学校的用户](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>作业

可以使用与作业相关的教育 API 与 Microsoft Teams 中的作业集成。 Microsoft 365 教育版中的 Microsoft Teams 基于同一教育 API，并提供了使用 API 执行哪些操作的用例。 应用可以使用这些 API 在整个作业生命周期内与作业进行交互。 

作业 API 提供以下关键资源：

- [educationAssignment](educationassignment.md) - 作业 API 的核心对象。 是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。
- [educationSubmission](educationsubmission.md) - 是指个人（或组）提交作业的资源以及该作业的相关成绩和反馈。
- [educationResource](educationresource.md) - 是指正在分配或提交的学习对象。 **educationResource** 与 **educationAssignment** 和/或 **educationSubmission** 相关联。

作业 API 支持以下方案：

- [创建作业](../api/educationclass-post-assignment.md)
- [发布作业](../api/educationassignment-publish.md)
- [创建作业资源](../api/educationassignment-post-resource.md)
- [创建提交资源](../api/educationsubmission-post-resources.md)
- [提交作业](../api/educationsubmission-submit.md)
- [取消提交作业](../api/educationsubmission-unsubmit.md)
- [将成绩和反馈返回给学生](../api/educationsubmission-return.md)
- [获取作业详细信息](../api/educationuser-list-assignments.md)

以下是与作业相关的教育 API 的一些常见用例。

| 用例                    | 说明                                                                                                         | 另请参阅                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| 创建作业          | 外部系统可以创建课堂作业并将资源附加到作业。                   | [创建作业](../api/educationassignment-post-resource.md) |
| 阅读作业信息 | 分析应用可以获取有关作业和学生提交（包括日期和成绩）的信息。 | [获取作业](../api/educationassignment-get.md)               |
| 跟踪学生作业提交   | 应用可为教师提供仪表板，显示有多少学生提交的作业需要评分。           | [提交资源](educationsubmission.md)                     |

## <a name="whats-new"></a>最近更新

了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

使用 Microsoft Graph 教育 API 构建访问学校名单的教育解决方案。若要了解详细信息，请：

- 探索对你的方案最有帮助的资源和方法。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。
