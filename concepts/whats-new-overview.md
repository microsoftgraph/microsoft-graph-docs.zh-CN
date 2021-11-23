---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 37f80e951ea71d5847e0c793053c3a1bc9cd42dc
ms.sourcegitcommit: c6bbba6cb9aaa7ad35374d1b5d4466c49878ab43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2021
ms.locfileid: "61135170"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


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

## <a name="october-2021-new-and-generally-available"></a>2021 年 10 月：新增和正式版本

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
- [传输](/graph/api/call-transfer)活动对等呼叫。
- 将组呼叫传输给指定与会者（传输接收方）。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
支持拨入电话访问和[联机会议](/graph/api/resources/onlinemeeting)（[音频会议](/graph/api/resources/audioConferencing)）使用多个收费和免费号码。

<!-- Hold off until permissions are deployed
As part of [privacy management in Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), subject rights request now debuts in both v1 and beta endpoints of Microsoft Graph. The [subject rights request API](/graph/api/resources/subjectrightsrequest) lets users make requests to review or manage their personal data in their organizations. It also lets organizations automate and scale managing these requests, helping them to meet industry regulations more efficiently.
-->

### <a name="education"></a>教育
支持将 [介质](/graph/api/resources/educationMediaResource) 文件或其他 [外部泛型资源](/graph/api/resources/educationExternalResource) 为 [分配资源](/graph/api/resources/educationassignmentresource)。

### <a name="identity-and-access--applications"></a>标识和访问权限 | 应用程序
- 若要改进[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)的许可体验，请指定[应用程序需要访问的资源](/graph/api/resources/requiredresourceaccess?view=graph-rest-beta&preserve-view=true)，包括应用程序所需的 OAuth 2.0 委派权限和应用程序角色集。
- 将所需 API 的数量限制为 50 个，将每个应用程序所需的权限限制为 400 个。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- 设置[设备](/graph/api/resources/device)的[扩展属性](/graph/api/resources/onpremisesextensionattributes)，并在[创建](/graph/api/device-post-devices)或[更新](/graph/api/device-update)设备时，在 Azure Active Directory 中管理这些属性。
- [代表登录的用户（设备所有者或相应的角色）获取 BitLocker 恢复密钥](/graph/api/bitlockerrecoverykey-get)。 获取恢复密钥会生成与最终用户体验存在奇偶校验的[审核日志](/azure/active-directory/reports-monitoring/concept-audit-logs)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
通过 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) 的 **additionalNotificationRecipients** 属性，将清单中其他用户或组成员指定为接收访问评审进度的通知。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
将[条件访问策略](/graph/api/resources/conditionalaccesspolicy)中的设备指定为应用该策略时，负责管理的一部分[条件](/graph/api/resources/conditionalAccessConditionSet)。

### <a name="personal-contacts"></a>个人联系人
在个人 Microsoft 帐户中，对 [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-beta&preserve-view=true) 资源启用支持委派的权限（`Contacts.Read` 或 `Contacts.ReadWrite`）。

### <a name="teamwork"></a>Teamwork
- [通过[团队](/graph/api/resources/team)中的所有频道获取所有消息](/graph/api/channel-getallmessages)。
- 从用户参与的[所有聊天中获取所有消息](/graph/api/chats-getallmessages)，包括一对一聊天、群组聊天和会议聊天。
- 了解适用于 Microsoft Graph 中的 Microsoft Teams API 的[许可和付款模式](teams-licenses.md)。

### <a name="users"></a>用户
现在，Azure Active Directory (Azure AD) 服务的用户许可证支持使用时间戳来显示最后一次更新 [许可证分配状态](/graph/api/resources/licenseassignmentstate) 的时间。 

## <a name="october-2021-new-in-preview-only"></a>2021 年 10 月：仅限预览版中的新增功能

### <a name="applications"></a>应用程序
使用[联合标识凭据](/graph/api/resources/federatedidentitycredential?view=graph-rest-beta&preserve-view=true)管理应用程序的凭据，并允许组织的云应用程序在不使用机密和证书的情况下访问 Azure AD。

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
使用 [participantInfo](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true) 资源类型的 **participantId** 属性，确定呼叫 [参与者](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true)。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
启用[会议注册](/graph/api/resources/meetingregistration?view=graph-rest-beta&preserve-view=true)，并组织联机会议作为[网络研讨会](/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3)。 将会议与注册页关联，并选择将每个人或仅组织成员注册为[会议注册者](/graph/api/resources/meetingregistrant?view=graph-rest-beta&preserve-view=true)。 

### <a name="customer-booking"></a>客户预订
- 支持[预订服务](/graph/api/resources/bookingService?view=graph-rest-beta&preserve-view=true)的以下属性：
  - 启用向客户发送短信预约通知（**smsNotificationsEnabled** 属性）。
  - 客户可用于访问服务（**webUrl** 属性）的 URL。
- 通过以下其中一个或多个属性进行[预约](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true)：
  - 指定客户的时区（**customerTimeZone** 属性）。
  - 指定在线预约的 URL（**joinWebUrl** 属性）。
  - 启用向客户发送短信预约通知（**smsNotificationsEnabled** 属性）。
- 为[客户](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true)指定一个或多个地址和电话号码。
- 指定[员工成员](/graph/api/resources/bookingStaffMember?view=graph-rest-beta&preserve-view=true)所在的时区。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
[列出](/graph/api/virtualendpoint-list-serviceplans?view=graph-rest-beta&preserve-view=true)组织的云电脑订阅的 [Windows 365 服务计划](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true)。 在每个[服务计划类型](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true#cloudpcserviceplantype-values)（商业版或企业版）下，组织可以选择从按 vCPU、内存和存储等属性划分的多种计划配置中选择要订阅的计划。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
指定可[配置为对应用程序或服务主体的限制](/graph/api/resources/appmanagementconfiguration?view=graph-rest-beta&preserve-view=true)的[密钥凭据配置设置](/graph/api/resources/keycredentialconfiguration?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
启用以下其他[设置](/graph/api/resources/assignmentReviewSettings?view=graph-rest-beta&preserve-view=true)，查看[访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)：
- 未在指定的有效时间内评审请求时的默认行为（**accessReviewTimeoutBehavior** 属性）。
- 向审阅者显示推荐（**isAccessRecommendationEnabled** 属性）。
- 要求审阅者提供审批理由（**isApprovalJustificationRequired** 属性）。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 指定[连续访问评估策略](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true)设置是应该迁移还是已迁移到[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)。
- 作为 Azure Active Directory [条件访问](/azure/active-directory/conditional-access/overview)的一部分，使用新的会议控制 [continuousAccessEvaluationSessionControl](/graph/api/resources/continuousAccessEvaluationSessionControl?view=graph-rest-beta&preserve-view=true) 来持续评估访问权限并制定访问权限决策。

### <a name="search--index"></a>搜索 | 索引
- 指定[外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)中内容的搜索体验的[设置](/graph/api/resources/externalconnectors-searchsettings?view=graph-rest-beta&preserve-view=true)。 例如，搜索结果的[显示模板](/graph/api/resources/externalconnectors-displaytemplate?view=graph-rest-beta&preserve-view=true)和用于选择显示模板的[规则](/graph/api/resources/externalconnectors-propertyRule?view=graph-rest-beta&preserve-view=true)。
- 将一个或多个[外部组](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-beta&preserve-view=true)关联到[外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)。 例如，外部组（如业务部门或工作组）可以确定对外部连接表示的数据源中内容的权限。
- 还可以在 **connectorId** 属性的 [外部连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)中指定 Teams 应用的 ID。

### <a name="users"></a>用户
当用户键入密码时，根据组织的密码验证策略实时 [验证密码](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true)。 根据策略中的规则，[从验证获取详细信息](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true)。



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
