---
title: 在 Microsoft Graph 中使用教育 API
description: Microsoft Graph 中的教育 api 使用与教育方案相关的信息 (包括学校、学生、教师、课程、注册和工作分配) 增强了 Office 365 的资源和数据。 这使你能够轻松地构建与教育资源集成的解决方案。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534869"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>在 Microsoft Graph 中使用教育 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 中的教育 api 使用与教育方案相关的信息 (包括学校、学生、教师、课程、注册和工作分配) 增强了 Office 365 的资源和数据。 这使你能够轻松地构建与教育资源集成的解决方案。

教育 api 包括名册资源和工作分配资源, 您可以使用这些资源与 Microsoft 团队中的名册和工作分配服务进行交互。 您可以使用这些资源管理学校名单并自动完成学生作业。

## <a name="authorization"></a>授权

若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。 有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。 你的应用还需要具有相应的权限。 有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>请求学校 IT 管理员许可的应用权限 

若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。 仅能授权许可一次，除非权限更改。 在管理员许可后，就会为租户中的所有用户预配应用。

若要触发许可对话框, 请使用以下 REST 调用。

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|参数|说明|
|:--------|:----------|
|Tenant|学校的租户 ID。 使用完整 ID，其中包含 onmicrosoft.com。|
|clientId|应用的客户端 ID。|
|redirectUrl|应用重定向 URL。|


## <a name="rostering"></a>Rostering

借助名册 API，可以从学校的 Office 365 租户（预配了 [Microsoft 学校数据同步](https://sds.microsoft.com/)）中提取数据。这些 API 提供对有关学校、部门、教师、学生和名册的信息的访问权限。 API 既支持仅应用（同步）方案，也支持应用 + 用户（交互）方案。 支持交互式方案的 API 基于调用 API 的用户角色，强制实施相应地区的 RBAC 策略。 这可以提供一致的 API 和最小策略展现，而无需考虑租户中的管理配置。 此外，API 还提供特定于教育的权限，确保相应用户具有访问数据的权限。

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

- [列出所有学校](../api/educationroot-list-schools.md) 
- [列出所教授课程的学校](../api/educationclass-list-schools.md)
- [为用户列出学校](../api/educationuser-list-schools.md)
- [获取所有课程](../api/educationroot_list_classes.md )
- [获取学校的课程](../api/educationschool-list-classes.md)
- [为用户列出课程](../api/educationuser-list-classes.md)
- [将课程添加到学校](../api/educationschool-post-classes.md)
- [获取课程的学生和教师](../api/educationclass-list-members.md)
- [将成员添加到课程](../api/educationclass-post-members.md) 
- [列出课程的教师](../api/educationclass-list-teachers.md)
- [获取学校的用户](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>作业 

您可以使用与工作分配相关的教育 api 与 Microsoft 团队中的工作分配集成。 适用于教育的 Office 365 中的 Microsoft 团队基于相同的教育 api, 并为使用 api 时可以执行的操作提供了一个用例。 您的应用程序可以使用这些 api 与工作分配生命周期中的工作分配进行交互。 

分配 api 提供以下关键资源:

- [educationAssignment](educationassignment.md) -工作分配 API 的核心对象。 表示分配给课程中的学生或团队成员的任务或工作单元, 作为其研究的一部分。
- [educationSubmission](educationsubmission.md) -表示个人 (或组) 提交的工作分配的资源, 以及该工作分配的相关评分和反馈。
- [educationResource](educationresource.md) -表示要分配或提交的学习对象。 **educationResource**与**educationAssignment**和/或**educationSubmission**相关联。

分配 api 支持以下方案:

- [创建作业](../api/educationclass-post-assignments.md)
- [发布作业](../api/educationassignment-publish.md)
- [创建作业资源](../api/educationassignment-post-resources.md)
- [创建提交资源](../api/educationsubmission-post-resources.md)
- [提交分配](../api/educationsubmission-submit.md) 
- [Unsubmit 分配](../api/educationsubmission-unsubmit.md)   
- [将成绩和反馈返回给学生](../api/educationsubmission-return.md) 
- [获取工作分配详细信息](../api/educationuser-list-assignments.md)

以下是与工作分配相关的教育 api 的一些常见用例。

|用例|说明|另请参阅|
|:-------|:----------|:-------|
|创建工作分配|外部系统可以为类创建分配并将资源附加到工作分配。|[创建作业](../api/educationassignment-post-resources.md)|
|读取工作分配信息|分析应用程序可以获取有关工作分配和学生提交的信息, 包括日期和成绩。|[获取作业](../api/educationassignment-get.md)|
|跟踪学生提交|您的应用程序可以提供一个教师仪表板, 以显示学生的提交次数需要进行评分。|[提交资源](educationsubmission.md)|

## <a name="school-data-sync-management"></a>学校数据同步管理

[学校数据同步](https://sds.microsoft.com/)可帮助您自动执行从使用 azure Active Directory (azure AD) 和 Office 365 导入和同步学生信息系统中的名单数据的过程。 您可以使用 Microsoft Graph 中的学校数据同步管理 api 设置 CSV 文件或受支持的 SIS API 连接器的同步。

学校数据同步管理 api 支持以下方案:

- [列出同步配置文件](../api/educationsynchronizationprofile-list.md)
- [获取同步配置文件](../api/educationsynchronizationprofile-get.md)
- [创建同步配置文件](../api/educationsynchronizationprofile-post.md)
- [删除同步配置文件](../api/educationsynchronizationprofile-delete.md)
- [暂停正在进行的同步](../api/educationsynchronizationprofile-pause.md)
- [恢复暂停的同步](../api/educationsynchronizationprofile-resume.md)
- [重置同步](../api/educationsynchronizationprofile-reset.md)
- [开始同步上载的文件](../api/educationsynchronizationprofile-start.md) 
- [获取上载 URL](../api/educationsynchronizationprofile-uploadurl.md)
- [获取同步状态](../api/educationsynchronizationprofilestatus-get.md)
- [获取同步错误](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>后续步骤
使用 Microsoft Graph 教育 api 生成可访问学生工作分配和学校名册的教育解决方案。 了解详细信息：

- 探索对你的方案最有帮助的资源和方法。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
