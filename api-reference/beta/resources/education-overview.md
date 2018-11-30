---
title: 在 Microsoft Graph 中使用教育 API
description: 教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。 这使你能够轻松地构建与教育资源集成的解决方案。
ms.openlocfilehash: 610a16af6993397ae9162fb27add97cd6c5af0ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048472"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>在 Microsoft Graph 中使用教育 API

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

教育在 Microsoft Graph 中的 Api 增强 Office 365 资源和数据的教育方案，其中包括学校、 学生、 教师、 类、 注册，和工作分配的相关信息。 这使你能够轻松地构建与教育资源集成的解决方案。

教育 Api 包括 rostering 资源和分配资源可用于与中的 Microsoft 团队的 rostering 和分配服务进行交互。 这些资源可用于管理学校名单和自动化学员。

## <a name="authorization"></a>授权

若要在 Microsoft Graph 中调用教育 API，你的应用需要获取访问令牌。 有关访问令牌的详细信息，请参阅[获取用于调用 Microsoft Graph 的访问令牌](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。 你的应用还需要具有相应的权限。 有关详细信息，请参阅[教育权限](/graph/permissions-reference#education-permissions)。 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>请求学校 IT 管理员许可的应用权限 

若要部署与 Microsoft Graph 中的教育 API 集成的应用，学校 IT 管理员必须首先授权许可应用请求的权限。 仅能授权许可一次，除非权限更改。 管理员同意后，将对租户中的所有用户预配应用。

若要触发许可对话框，请使用以下 REST 调用。

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

您可以使用 Api 中的工作分配相关 education 集成的 Microsoft 团队中具有工作分配。 Office 365 教育版中的 Microsoft 团队基于相同的教育 Api，并提供使用案例使用 Api 可以执行的操作。 您的应用程序可以使用这些 Api 进行交互的整个生命周期工作分配的工作分配。 

工作分配 Api 提供以下关键资源：

- [educationAssignment](educationassignment.md) -分配 API 的核心对象。 表示任务或工作分配给类中的学生或团队成员属于其研究单位。
- [educationSubmission](educationsubmission.md) -表示的资源的个人 （或组） 提交的工作分配关联薪等级和工作分配的反馈。
- [educationResource](educationresource.md) -表示学习对象，它是被分配或提交。 **EducationResource**相关联**educationAssignment**和/或**educationSubmission**。

工作分配 Api 支持以下方案：

- [创建工作分配](../api/educationclass-post-assignments.md)
- [发布工作分配](../api/educationassignment-publish.md)
- [创建工作分配资源](../api/educationassignment-post-resources.md)
- [创建提交资源](../api/educationsubmission-post-resources.md)
- [提交的作业](../api/educationsubmission-submit.md) 
- [Unsubmit 工作分配](../api/educationsubmission-unsubmit.md)   
- [返回学生薪等级和反馈](../api/educationsubmission-return.md) 
- [获取工作分配详细信息](../api/educationuser-list-assignments.md)

以下是一些常见的使用案例工作分配相关教育版 Api。

|用例|说明|另请参阅|
|:-------|:----------|:-------|
|创建工作分配|外部系统可以创建类的工作分配，并附加到工作分配的资源。|[创建工作分配](../api/educationassignment-post-resources.md)|
|读取工作分配信息|分析应用程序可以获取有关分配和学生提交，包括多个日期和薪等级的信息。|[获取工作分配](../api/educationassignment-get.md)|
|跟踪学生提交|您的应用程序可以提供的显示多少拾取学生需要进行评分教师仪表板。|[提交资源](educationsubmission.md)|

## <a name="school-data-sync-management"></a>学校数据同步管理

[学校数据同步](https://sds.microsoft.com/)可帮助自动完成的导入和与 Azure Active Directory (Azure AD) 和 Office 365 同步学生信息系统中的名单数据的过程。 您可以使用在 Microsoft Graph 学校数据同步管理 Api 设置从 CSV 文件或支持的 SI API 连接器的同步。

学校数据同步管理 Api 支持以下方案：

- [列表同步配置文件](../api/educationsynchronizationprofile-list.md)
- [获取同步配置文件](../api/educationsynchronizationprofile-get.md)
- [创建同步配置文件](../api/educationsynchronizationprofile-post.md)
- [删除同步配置文件](../api/educationsynchronizationprofile-delete.md)
- [暂停正在进行同步](../api/educationsynchronizationprofile-pause.md)
- [恢复暂停的同步](../api/educationsynchronizationprofile-resume.md)
- [重置 sync](../api/educationsynchronizationprofile-reset.md)
- [启动同步上载文件](../api/educationsynchronizationprofile-start.md) 
- [获取一个上载 URL](../api/educationsynchronizationprofile-uploadurl.md)
- [要获取同步的状态](../api/educationsynchronizationprofilestatus-get.md)
- [获取同步错误](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>后续步骤
使用 Microsoft Graph 教育 Api 构建访问学员和学校名单的教育解决方案。 了解详细信息：

- 探索对你的方案最有帮助的资源和方法。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。

