---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 7a6ab3c50fe14986744ccfd64fdddadd9aa67a6e
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822772"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

你是否知道 Microsoft Graph 中的一些新功能来源于开发人员社区的热门请求？ 

Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 

在下面查看 Microsoft Graph 中新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 如需了解 API 更新的更多详情，请参阅 API 更改日志的 [9 月](changelog.md#september-2019)和 [8 月](changelog.md#august-2019)部分。 


## <a name="september-2019-new-in-preview"></a>2019 年 9 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="users"></a>用户
- 获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta)。

## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月：新版本和正式版 

### <a name="reports"></a>报告
- 获取与已删除项计数和大小相关的更多[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)。
- 在[获取组活动详细信息](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)时，跟踪 Office 365 组 ID。
- 在获取 [OneDrive 使用帐户详细信息](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)和 [SharePoint 网站使用情况详细信息](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)时，跟踪所有者主体名称。
- 在[获取每 Office 365 服务的用户计数报告](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)时，获取 Office 365 上的活动和非活动用户数。

### <a name="security"></a>安全性
- 使用新的[适用于 Splunk 的 Microsoft Graph 安全性 API 加载项](https://aka.ms/graphsecuritysplunkaddon)将多个合作伙伴产品的安全警报和看法传输至 Splunk，从而更轻松地实时关联其安全性数据。 有关详细信息，请参阅[公告](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972)。 
- [查看由 Microsoft 或者与安全性 API 相关的 Microsoft 合作伙伴构建的其他解决方案和连接器列表](security-integration.md)，使你以统一的格式使用数据。


## <a name="august-2019-new-in-preview"></a>2019 年 8 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生变更，恕不另行通知；一些功能可能永远不会升级为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [8 月](changelog.md#august-2019)更新

### <a name="education"></a>教育版
- 将[教师](/graph/api/resources/educationuser?view=graph-rest-beta)或[作业](/graph/api/resources/educationassignment?view=graph-rest-beta)与[评分标准](/graph/api/resources/educationrubric?view=graph-rest-beta)相关联，以解释特定作业质量和等级。 质量示例为拼写和语法，等级示例为“良好”和“不良”。 可以进一步将点数和权重与评分标准相关联。 有关详细信息，请参阅[教育版评分标准概述](education-rubric-overview.md)。
- 评估作业并从[反馈](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta)、[数字等级](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta)或[评分标准](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta)方面展示结果。

### <a name="files"></a>文件
到目前为止，你已可以[关注](/graph/api/driveitem-follow?view=graph-rest-beta) [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 现在可以使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-beta)操作来停止关注此类驱动器项。

### <a name="identity-and-access"></a>身份和访问
- 基于角色的访问控制 (RBAC) 提供商可以在 Azure Active Director 中[管理角色](/graph/api/resources/rolemanagement?view=graph-rest-beta)，方法是[定义可以在特定资源上执行的角色操作](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta)，基于这些角色定义为用户[分配角色](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta)，为他们授权相应的资源访问权限。
- 管理员可以[列出访问审查](/graph/api/accessreview-list?view=graph-rest-beta)，以高效地审核组成员身份、企业应用程序访问权限和角色分配。 定期访问审查可确保只有相应的人员才能继续以特定方式访问资源。

### <a name="social-and-workplace-intelligence"></a>社交和工作场所智能
最终用户可以使用 Office 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) 应用获取与管理时间、工作协作和工作生活平衡有关的见解。 现在，你可以使用[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) 整合与工作活动（如呼叫、聊天和电子邮件）所花时间相关的数据、以帮助提高用户的工作效率和幸福感。 


## <a name="want-to-stay-in-the-loop"></a>保持循环
- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/zh-CN/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/en-us/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

