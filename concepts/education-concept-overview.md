---
title: 教育版 API 概述
description: 使用 Microsoft Graph 中的教育 API 构建与课堂方案（如名单和作业）的教育资源集成的解决方案。
author: mmast-msft
ms.localizationpriority: high
ms.prod: education
ms.custom: scenarios:getting-started
ms.openlocfilehash: cddc7efd0d5242f68224c3909d0d93e2b55616d2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440892"
---
# <a name="education-api-overview"></a>教育版 API 概述

Microsoft Graph 中的教育版 API 可增强 Microsoft 365 资源和与教育情景相关的信息，其中包括有关学校、课程、用户（学生和教师）、作业以及订阅信息。 这使你能够轻松构建与各种学校和课堂情景的教育资源集成的解决方案。

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a>为什么与教育情景集成？

### <a name="build-applications-that-are-aware-of-class-roster"></a>构建了解班级名册的应用程序

大多数教育软件开发人员在早期便了解到，此班级名册是运行其应用程序所需的关键信息之一，而且它通常被锁定在学校的学生信息系统 (SIS) 中。 只要教师将新应用程序引入其课堂，他们就需要花时间手动将名单数据导入到该应用。 许多独立软件供应商 (ISV) 通过连接 SIS 导入名单数据来解决此问题。 在具备专有格式的数百个学生信息系统中，这将成为一个挑战。

将 [Microsoft 学校数据同步](https://sds.microsoft.com/)与名单 API 结合使用，可为应用程序开发人员以及学校解决这一难题。 以下是名单 API 启用的一些情况：

- [获取学校的所有课程](/graph/api/educationschool-list-classes)
- [获取课程的所有用户](/graph/api/educationclass-list-members)
- [获取我讲授的所有课程](/graph/api/educationuser-list-classes)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a>使用 Microsoft Teams 在“作业”选项卡中创建课程作业

可以使用与作业相关的教育 API 与 Microsoft Teams 中的作业集成。 Microsoft 365 教育版中的 Microsoft Teams 基于同一教育 API，并提供了使用 API 执行哪些操作的用例。 应用可以使用这些 API 在整个作业生命周期内与作业进行交互。

作业 API 提供以下关键资源：

- [educationAssignment](/graph/api/resources/educationassignment)：作业 API 的核心对象。 是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。
- [educationSubmission](/graph/api/resources/educationsubmission)：是指个人（或组）提交作业的资源以及该作业的相关成绩和反馈。
- [educationResource](/graph/api/resources/educationresource)：是指正在分配或提交的学习对象。 **educationResource** 与 **educationAssignment** 和/或 **educationSubmission** 相关联。

通过作业 API，你的应用可以与 Microsoft Teams 之外的作业服务进行交互。 Microsoft Teams 将处理分发、截止日期和评分，而系统可以为学生提供丰富的学习体验。

以下是由作业 API 启用的几个方案示例：

- [添加到应用程序的作业链接](/graph/api/educationclass-post-assignments) 
- [对于链接到应用程序的作业，将成绩等结果分配给各个学生](/graph/api/educationoutcome-update)
- [创建学生仪表板以显示哪些作业何时截止](/graph/api/educationclass-list-assignments)

### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a>使学校管理员能够使用学校数据同步管理（预览版）管理标识和名单同步

[学校数据同步](https://sds.microsoft.com/)可帮助自动执行从使用 Azure Active Directory (Azure AD) 和 Microsoft 365 的学生信息系统中导入和同步学生标识及名单数据的过程。 当同步信息时，可以使用名单 API 将名单信息读入应用程序。 

如果你是建立学校学生信息系统和学校数据同步整合关系的系统集成者，则可以使用 Microsoft Graph 中的 [SDS 管理 API](/graph/api/resources/educationsynchronizationprofile) 从 CSV 文件或受支持的 SIS API 连接器设置同步。

学校数据同步管理 API 支持用于管理同步的端到端方案；例如：

- [创建自动启动同步的同步配置文件](/graph/api/educationsynchronizationprofile-post)。
- 通过[暂停](/graph/api/educationsynchronizationprofile-pause)、[继续](/graph/api/educationsynchronizationprofile-resume)、[重置](/graph/api/educationsynchronizationprofile-reset)操作管理同步生命周期。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的教育版 API](/graph/api/resources/education-overview?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的教育版 API](/graph/api/resources/education-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

若要开始使用教育版 API，请参阅：
- [使用名单 API](/graph/api/resources/education-overview)
- [使用作业 API](/graph/api/resources/educationassignment)
- [使用 SDS 管理 API](/graph/api/resources/educationsynchronizationprofile)

在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中试用教育版 API

浏览下面的教育相关示例：
- [SSO 和排班 .NET 示例](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
- [配置文件管理 API 示例](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples)