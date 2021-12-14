---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 499fb9829c0f5b5eddc6f8b124fbf3d6375b5c12
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424573"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="december-2021-new-and-generally-available"></a>2021 年 12 月：新增功能并正式发布

### <a name="cloud-communications--presence"></a>云通信 | 预览版
对指定用户的[状态](/graph/api/resources/presence)[订阅更改通知](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&preserve-view=true)。 始终在订阅请求中指定加密证书，因为这些是[包含加密资源数据的丰富通知](webhooks-with-resource-data.md)。

## <a name="december-2021-new-in-preview-only"></a>2021 年 12 月：仅预览版新增功能

### <a name="cloud-communications--presence"></a>云通信 | 预览版
- 使用 [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 操作可设置用户的首选空闲状态和活动状态。 用户状态将成为首选状态。
- 使用 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 操作可清除用户的任何首选空闲状态和活动状态。
- 将 `Presence.ReadWrite` 用作 [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true)、 [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true)、[setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 或 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true)的委派权限。
- 将 `Presence.ReadWrite.All` 用作 [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true)、 [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true)、[setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 或 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true)的应用程序权限。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- 通过 **认证** 属性 [获取](/graph/api/application-get?view=graph-rest-beta&preserve-view=true)[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)的认证详细信息。 仅当应用程序是通过 [Microsoft 365 应用符合性计划](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)认证的时，才设置该属性。  
- 通过 [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) 的 **certifiedClientApplicationsOnly** 属性，将认证 [包含](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true)或 [排除](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true)为 [权限授予策略](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true)中的一个 [条件](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true)。

### <a name="search--index"></a>搜索 | 索引
使用[更新](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true)操作更新[连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)架构中项目的属性，包含其别名和标签。


## <a name="november-2021-new-and-generally-available"></a>2021 年 11 月：新增和正式发布

### <a name="files"></a>文件
通过指定相应的 URL 编码时间戳，获取特定时间的驱动器状态。 请参阅[示例](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp)。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
- 运行[活动](/graph/api/resources/authenticationMethodsRegistrationCampaign)，[强制用户在登录时注册](/graph/api/resources/registrationEnforcement)以设置目标身份验证方法。
-  在 Azure AD B2C 租户中配置 [Apple 标识提供者](/graph/api/resources/applemanagedidentityprovider)。

## <a name="november-2021-new-in-preview-only"></a>2021 年 11 月：仅预览版新增功能

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
在联机会议中自动允许新类型的参与者，并绕过会议大厅：
- 仅组织者邀请的人员。
- 仅来自同一公司的参与者。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 定义一个[配置](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true)预配的云电脑设备如何联接Azure Active Directory（Azure AD）：仅限云并仅加入Azure AD，或者混合和加入本地 Active Directory和Azure AD。
- 获取可用于预配云电脑的当前组织的 [库映像资源](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true)。

### <a name="devices-and-apps--device-updates"></a>设备和应用|设备更新
- 使用 [保护设置](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true) 选择退出针对部署中可能出现的问题的保护措施。
- 支持 [部署状态](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) 由于内容不再可部署而导致部署出错，例如服务结束时。

### <a name="identity-and-access--directory-management"></a>标识和访问权限 | 目录管理
- 定义[自定义安全属性](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true)并将其分配给Azure AD对象。 使用这些属性存储信息、对对象进行分类，或对特定 Azure 资源强制实施精细的访问控制。 将这些属性与[Azure 基于属性的访问控制](/azure/role-based-access-control/conditions-overview) （Azure ABAC） 配合使用。
- [在管理单元中创建组](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
[Microsoft 365 JSON 输出类型中](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) 的使用情况报告不再强类型化，并且属于类型 `Edm.Stream`。 有关详细信息，请参阅 [Microsoft Graph中Microsoft 365使用情况报告 API 的OData 属性更改](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/)。

### <a name="teamwork"></a>Teamwork
将聊天标记为 [阅读](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true)，或 [用户的未读](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true)。



## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的初次发布。任何相关的 REST API 更新都在 Beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
