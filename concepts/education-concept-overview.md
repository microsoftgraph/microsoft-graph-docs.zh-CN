---
title: 教育版 API 概述
description: Microsoft Graph 中的教育版 API 可增强 Office 365 资源和与教育情景相关的信息，其中包括有关学校、课程、用户（学生和教师）、作业以及订阅信息。 这使你能够轻松构建与各种学校和课堂情景的教育资源集成的解决方案。
author: mmast-msft
ms.openlocfilehash: 2085c9be619e3de5eb4df457579461445423113a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344987"
---
# <a name="education-api-overview"></a>教育版 API 概述

Microsoft Graph 中的教育版 API 可增强 Office 365 资源和与教育情景相关的信息，其中包括有关学校、课程、用户（学生和教师）、作业以及订阅信息。 这使你能够轻松构建与各种学校和课堂情景的教育资源集成的解决方案。

Microsoft Graph 中的教育版 API 提供对课程、学校、用户、作业、提交等的访问。

![EDU Graph 概述](images/edugraph.png)

## <a name="why-integrate-with-education-scenarios"></a>为什么与教育情景集成？

### <a name="build-applications-that-are-aware-of-class-roster"></a>构建了解班级名册的应用程序

大多数教育软件开发人员在早期便了解到，此班级名册是运行其应用程序所需的关键信息之一，而且它通常被锁定在学校的学生信息系统 (SIS) 中。 只要教师将新应用程序引入其课堂，他们就需要花时间手动将名单数据导入到该应用。 许多 ISV 通过连接 SIS 导入名单数据来解决此问题。 在具备专有格式的数百个学生信息系统中，这将成为一个挑战。 将 [Microsoft 学校数据同步](https://sds.microsoft.com/)与名单 API 结合使用，可为应用程序开发人员以及学校解决这一难题。

以下是名单 API 启用的一些情况：

- [获取学校的所有课程](/graph/api/educationschool-list-classes?view=graph-rest-1.0)
- [获取课程的所有用户](/graph/api/educationclass-list-members?view=graph-rest-1.0)
- [获取我讲授的所有课程](/graph/api/educationuser-list-classes?view=graph-rest-1.0)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a>使用 Microsoft Teams 在“作业”选项卡中创建课程作业


可使用作业 API 创建 Web 应用来管理课程作业，然后在新自定义选项卡上将应用集成到 Microsoft Teams。  

Office 365 中的 Microsoft Teams 是一个数字中心，它可将对话、内容和应用整合到教室这一个位置中。 Microsoft Teams 提供了[一组丰富的扩展点](https://docs.microsoft.com/zh-CN/microsoftteams/platform/concepts/apps/apps-overview)，包括创建选项卡、连接器和自动程序。 这些扩展点可以在 Microsoft Graph 中调用教育版 API 以处理作业和提交。 通过启用具备任何其他 Microsoft Graph API 以及作业和提交 API 的扩展点来构建更全面的体验。

对于教育版，Microsoft Teams 自定义选项卡应用在教育课堂（团队）上下文中打开，在此环境中，管理端到端作业流（从创建和分发到评分和反馈）别具意义。 这只是有关 Microsoft Teams 如何节省时间和简化日常后勤的一个示例，以便教育工作者可以更多地将重心放在他们的学生身上。

下图显示了**科学-生物学科 1**课程“作业”自定义选项卡中用于管理作业的 Web 应用。

![Microsoft Teams 中面向“科学-生物学科”课程的“作业”选项卡屏幕截图](images/assignmentsinteams.png)


通过作业 API，你的应用可以与 Microsoft Teams 之外的作业服务进行交互。 Microsoft Teams 将处理分发、截止日期和评分，而系统可以为学生提供丰富的学习体验。
以下是由作业 API 启用的几个方案示例：

- [添加到应用程序的作业链接](/graph/api/educationclass-post-assignments?view=graph-rest-beta) 
- [对于链接到应用程序的作业，将成绩分配给各个学生](/graph/api/educationsubmission-update?view=graph-rest-beta)
- [创建学生仪表板以显示哪些作业何时截止](/graph/api/educationclass-list-assignments?view=graph-rest-beta)


### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a>使学校管理员能够使用学校数据同步管理（预览版）管理标识和名单同步

[学校数据同步](https://sds.microsoft.com/)可帮助自动执行从使用 Azure Active Directory (Azure AD) 和 Office 365 的学生信息系统中导入和同步学生标识及名单数据的过程。 当同步信息时，可以使用名单 API 将名单信息读入应用程序。 如果你是建立学校学生信息系统和学校数据同步整合关系的系统集成者，则可以使用 Microsoft Graph 中的 [SDS 管理 API](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) 从 CSV 文件或受支持的 SIS API 连接器设置同步。

学校数据同步管理 API 支持用于管理同步的端到端方案；例如：

- [创建自动启动同步的同步配置文件](/graph/api/educationsynchronizationprofile-post?view=graph-rest-beta)
- 通过[暂停](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta)、[继续](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta)和[重置](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta)操作管理同步生命周期

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的教育版 API](/graph/api/resources/education-overview?view=graph-rest-1.0)
- [Microsoft Graph beta 中的教育版 API](/graph/api/resources/education-overview?view=graph-rest-beta)


## <a name="next-steps"></a>后续步骤

- 若要开始使用教育版 API，请参阅：
    - [使用名单 API](/graph/api/resources/education-overview?view=graph-rest-1.0)
    - [使用作业 API](/graph/api/resources/educationassignment?view=graph-rest-beta)
    - [使用 SDS 管理 API](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta)
- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中试用教育版 API。
- 浏览下面的教育相关示例：
    - [SSO 和排班 .NET 示例](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
    - [SSO 和排班 Angular Node 示例](https://github.com/OfficeDev/O365-EDU-AngularNodeJS-Samples)   
    - [SSO 和排班 Python 示例](https://github.com/OfficeDev/O365-EDU-Python-Samples)
    - [SSO 和排班 PHP 示例](https://github.com/OfficeDev/O365-EDU-PHP-Samples)
    - [配置文件管理 API 示例](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples) 



 

