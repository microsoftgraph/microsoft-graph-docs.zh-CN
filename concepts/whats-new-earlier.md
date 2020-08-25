---
title: Microsoft Graph 早期版本的亮点
description: Microsoft Graph 早期版本中的新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: de4aec69c62c611532143d2dfee2340b485d3a0f
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873074"
---
# <a name="highlights-of-earlier-releases"></a>早期版本的亮点

## <a name="june-2020-new-and-generally-available"></a>2020 年 6 月：新版本和正式版

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
- [创建联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) 以提供基于区域的加入信息时，请使用 `Accept-Language` HTTP 标头。
- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) 返回具有指定 **externalId** 值的在线会议，或者创建一个外部值（如果不存在），以简化将结果会议嵌入到第三方日历中。

### <a name="files"></a>文件
- 增强的同步支持：
  - 使用 **pendingOperations** 属性标识可能会更新挂起的 [driveItem](/graph/api/resources/driveitem) 文件的二进制内容的任何 [操作](/graph/api/resources/pendingoperations)。
  - [还原](/graph/api/driveitem-restore) 已删除且位于 OneDrive 个人版回收站中的 **driveItem**。
- 获取或设置[照片](/graph/api/resources/photo)的方向。 OneDrive 个人版上支持设置。
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file)数据安全性和完整性。
- 在向 OneDrive for Business [上传一个大文件](/graph/api/driveitem-createuploadsession)时，使用 `deferCommit`这个参数来延迟最终的创建，直到应用程序请求完成上传。
- 使用 **fileSize** 属性作为 **项目**参数的一部分提供估算，以便在在将文件 [上载](/graph/api/driveitem-createuploadsession)到 OneDrive 个人版中之前执行配额检查。
- 通过 [驱动器的 **quota** 属性找到 [storagePlanInformation](/graph/api/resources/storageplaninformation)](/graph/api/resources/drive) 资源，查看是否有更高的存储配额计划可用。

### <a name="groups"></a>组
使用应用程序权限`Group.Read.All`和`Group.ReadWrite.All`，以便获得[组对话](/graph/api/resources/conversation)和[对话线程](/graph/api/resources/conversationthread)的资源。

### <a name="identity-and-access"></a>身份和访问 
- GA 两组 API，用于 [标识保护](/graph/api/resources/identityprotectionroot)： [的风险检测](/graph/api/resources/riskdetection) 和 [有风险的用户](/graph/api/resources/riskyuser) API。

### <a name="security"></a>安全性
- 在 [警报](/graph/api/resources/alert?view=graph-rest-1.0)的属性中跟踪以下内容：
  - 与警报相关的事件的ID。
  - 将 [资源标识](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) 为受攻击或警报中的相关资源。
  - 指定与警报相关的 [网络连接](/graph/api/resources/networkconnection?view=graph-rest-1.0) 的源和目标位置。

### <a name="sites-and-lists"></a>网站和列表
指定 SharePoint [列表](/graph/api/resources/list) 资源的 [列定义](/graph/api/resources/columndefinition) 中的地理位置数据。

### <a name="teamwork"></a>团队合作
- 使用委派的权限[AppCatalog.Read.All](/graph/permissions-reference#appcatalog-resource-permissions)列出来自 Microsoft Teams 应用程序目录的[应用](/graph/api/resources/teamsapp?view=graph-rest-1.0)。
- [获取有关映射到 Teams [频道](/graph/api/resources/channel)中的**文件** 选项卡的文件夹](/graph/api/channel-get-filesfolder) 的信息。
- [获取[团队](/graph/api/resources/team)的默认频道](/graph/api/team-get-primarychannel)，标记为**常规**"。


## <a name="june-2020-new-in-preview-only"></a>2020 年 6 月：预览版新增功能

### <a name="calendar"></a>日历
除了跟踪**calendarView**中事件的增量更改（集合或由 start _和_结束日期分隔的事件），请对用户邮箱中的事件或特定用户日历中的事件使用[delta](/graph/api/event-delta?view=graph-rest-beta)功能。

### <a name="cloud-communications--presence"></a>云通信 | 预览版
[获取组织中所有用户的状态](/graph/api/presence-get?view=graph-rest-beta) 或组织中特定用户的状态。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 在配置 [文档进行打印](/graph/api/resources/printdocument?view=graph-rest-beta)时指定[打印页边距](/graph/api/resources/printmargin?view=graph-rest-beta)。
- 支持以下 [打印机功能](/graph/api/resources/printercapabilities?view=graph-rest-beta)：
  - 源方向
  - 打印页面范围
  - 在DPI上的打印分辨率
  - 最大打印作业队列大小（以字节为单位）
  - 输入纸盒
  - 边距
  - collation
  - 文档缩放
- 支持打印分辨率（DPI）和文档缩放作为 [默认打印机设置](/graph/api/resources/printerdefaults?view=graph-rest-beta)中的一部分。
- 支持以下 [文档配置](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta) 设置：
  - 输入纸盒
  - 输出纸盒
  - 媒体大小
  - 边距
  - 媒体类型
  - finishings （例如装订）
  - 每版打印页数
  - 多页版式指定每版打印页面的布局方向
  - collation
  - scaling
- 在[列出pring作业](/graph/api/printer-list-jobs?view=graph-rest-beta)时展开文档。
- [注册打印机]()并使用[printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta)资源跟踪和验证打印机的注册。
- 在当前用户或应用程序的租户内[获取长期运行的打印机注册操作](/graph/api/printoperation-get?view=graph-rest-beta)。
- 一些属性和枚举类型的重命名 - 详见[六月](changelog.md#june-2020)更新的云打印更新。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[6月](changelog.md#june-2020)试用版中更新

### <a name="education"></a>教育
- 可以使用委托权限`EduRoster.ReadBasic`来[获取](/graph/api/educationuser-get?view=graph-rest-beta)外部源程序中的[教师](/graph/api/resources/educationteacher?view=graph-rest-beta)或[学生](/graph/api/resources/educationstudent?view=graph-rest-beta)的ID，作为**externalId**属性。
- 如果从学习管理系统(LMS)创建了教育[组织](/graph/api/resources/educationorganization?view=graph-rest-beta)或[班别](/graph/api/resources/educationclass?view=graph-rest-beta)，那么使用**externalSource**属性来跟踪值`lms`。

### <a name="identity-and-access"></a>身份和访问
- IT专业人员可以使用作为轻量级代理的[连接器](/graph/api/resources/connector?view=graph-rest-beta)资源连接到[Azure AD 应用程序代理](/azure/active-directory/manage-apps/what-is-application-proxy)，并[在外部发布本地web应用程序应用程序](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)，以便其组织的远程用户可以以安全的方式访问这些应用程序。
- 在租户级别[管理身份验证策略](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta)，以启用或禁用外部用户的[自服务注册](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta)。
- [按需提供用户帐户](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta)，并能够指定要提供的对象和要执行的同步规则。

### <a name="search"></a>搜索
- 利用[模式](/graph/api/resources/schema?view=graph-rest-beta)中[属性](/graph/api/resources/property?view=graph-rest-beta)上的增强功能：**isRefinable** 支持搜索结果的过滤和更精细的搜索体验控制，**别名**和**标签** 支持更好的相关性。
- 在 **架构**中，最多可以指定 128 **属性** 资源。
- 使用 [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta) 用于诊断目的。

### <a name="users"></a>用户
- 使用 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) 的 **userPurpose** 属性，可在 Exchange Online 中识别共享邮箱和设备邮箱中的单个用户的邮箱并从中区分。 
- 使用 [用户设置](/graph/api/resources/usersettings?view=graph-rest-beta)去 [获取](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta)或[更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta)[首选语言和区域设置](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta)。
- 用户设置是通过点击 Azure AD 用户配置文件以反映相同的用户首选项，可通过 [用户](/graph/api/resources/user?view=graph-rest-beta) 实现跨应用的一致用户体验的关系。 请参阅 [用户设置与邮箱设置](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats)的区别。


## <a name="may-2020-new-and-generally-available"></a>2020 年 5 月：新版本和正式版

### <a name="calendar--place"></a>日历 | 位置
v1.0 中的[位置 API](/graph/api/resources/place) 的正式版 - 在生产应用中使用此 API 可以获取、更新或删除租户中的[房间](/graph/api/resources/room)或[房间列表](/graph/api/resources/roomlist)。 [了解有关位置 API 的详细信息](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context)。

### <a name="change-notifications"></a>更改通知
- 订阅 Microsoft Cloud for US Government 中的更改通知。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- [通话记录 API](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0) 的正式版 - 使用 [callRecord ](/graph/api/resources/callrecord?view=graph-rest-1.0) 资源获取 Microsoft Teams 和 Skype 上的通话和在线会议的元数据。
- 订阅[更改通知](/graph/webhooks)，了解组织中所有** callRecord** 资源的更改。
- 在 **callRecord** 中[列出会话](/graph/api/callrecords-session-list?view=graph-rest-1.0)，并根据需要[扩展每个会话以列出呼叫记录中的段](/graph/api/callrecords-session-list?view=graph-rest-1.0#example-2-get-session-list-with-segments)。
- 支持段中媒体端点的 60 GHz (`frequency60GHz`) 和 `unknownFutureValue`WiFi 波段值。
- 支持将语音邮件作为通信[段](/graph/api/resources/callrecords-segment)中服务端端点的一种可能类型。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
v1.0 中的 Intune [5 月](changelog.md#may-2020)更新。

### <a name="graph-explorer"></a>Graph 浏览器
[Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)中的许多新功能可用于增强沙箱中的学习和原型制作。 例如：
- 在 C#、Java、JavaScript 和 Objective C 中查看与你输入的 REST API 查询相对应的代码段。
- 登录租户、查看访问令牌并将其复制到你喜欢的 REST 客户端应用程序。

有关详细信息，请参阅[新 Graph 浏览器现已上市](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/)。

### <a name="groups"></a>组
- 通过 Azure AD Connect 将本地目录同步到 Azure Active Directory 时现在会返回 **onPremisesDomainName **、**onPremisesNetBiosName** 和 **onPremisesSamAccountName** 属性，作为[组](/graph/api/resources/group?view=graph-rest-1.0)资源的一部分。
- 订阅由 21Vianet 运营的 Microsoft Cloud 中国的 [group](/graph/api/resources/group) 资源的更改通知。

### <a name="identity-and-access"></a>身份和访问
- v1.0 中的服务主体 API 的正式版 - 使用生产应用程序中的 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) 资源，以编程方式管理应用程序实例并控制应用程序可以在租户中执行的操作。 你可以控制谁可以使用应用程序、应用程序可以访问哪些资源，例如添加密码凭据、滚动过期证书以及管理委派的权限授予和应用程序角色分配。
- [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) API 的正式版，该 API 记录了 向[用户](/graph/api/resources/user?view=graph-rest-1.0)、[组](/graph/api/resources/group?view=graph-rest-1.0)或 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)的 [appRole](/graph/api/resources/approle?view=graph-rest-1.0) 分配情况（代表 ID 令牌和访问令牌中的 `roles` 声明）。
- 在 Azure Active Directory 上使用 Facebook 作为标识提供程序。
- 使用 `AppRoleAssignment.ReadWrite.All` 的委派权限或应用程序权限以允许应用管理任何 API（包括 Microsoft Graph）的应用程序权限授予和任何应用（已登录或未登录用户）的应用程序分配。


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
有关如下内容，请参阅新的 SDK 指南：
- [分页](/graph/sdks/paging)
- [批处理](/graph/sdks/batch-requests)
- [将大文件上传到 OneDrive](/graph/sdks/large-file-upload)
- [通过 HTTP 中间件组件自定义 SDK 服务客户端](/graph/sdks/customize-client)。

### <a name="teamwork"></a>团队合作
- 如果你的方案涉及 Teams 在线会议，请参阅有关[如何在[日历 API ](outlook-calendar-online-meetings.md)和[云通信 API](cloud-communications-online-meetings.md)之间进行选择](choose-online-meeting-api.md)的新指南，以创建和加入在线会议。
- [在[频道](/graph/api/resources/channel?view=graph-rest-1.0)中发送](/graph/api/channel-post-messages?view=graph-rest-1.0)和[回复](/graph/api/channel-post-messagereply?view=graph-rest-1.0)邮件。
- 通过使用 **fileFolder** 导航属性，获取[频道](/graph/api/resources/channel?view=graph-rest-1.0)文件的 OneDrive for Business 位置。

### <a name="teamwork--shifts"></a>团队合作 | Shifts
v1.0 中 [ shifts API](/graph/api/resources/shift?view=graph-rest-1.0) 的正式版 - 在生产应用程序中使用此 API 创建、更新和管理一线员工的日程安排，以使他们保持联系并有效进行协作。

### <a name="users"></a>用户
- 订阅由 21Vianet 运营的 Microsoft Cloud 中国的 [user](/graph/api/resources/user) 资源的更改通知。
- 通过使用 **user** 资源的 **externalUserState** 和 **externalUserStateChangeDateTime** 跟踪[已受邀](/graph/api/invitation-post?view=graph-rest-1.0)加入组织的外部用户的最新状态更改的状态和日期/时间。

## <a name="may-2020-new-in-preview-only"></a>2020 年 5 月：仅限预览版新增功能

### <a name="change-notifications"></a>更改通知
- 使用正式架构化的类型 [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) 和 [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) 处理资源更改通知。 
- 通过使用 **changeNotification** 资源上的 **sequenceNumber** 属性跟踪通知是否按顺序或是否缺少通知。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [printer](/graph/api/resources/printer?view=graph-rest-beta) 和 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta) 资源现在是奇偶校验的，并且彼此具有相同的属性。
- 围绕打印机共享的一些属性和类型名称清理：
  - 使用 [print](/graph/api/resources/print?view=graph-rest-beta) 的 **shared** 导航属性来获取在租户中注册的打印机共享列表。 
  - 有关详细信息，请参阅 [5 月](changelog.md#may-2020)更改日志。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
测试版中的 Intune [5 月](changelog.md#may-2020)更新。

### <a name="groups"></a>组
- 使用[组](/graph/api/resources/group?view=graph-rest-beta)的现有规则或指定规则[评估](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta)用户或设备是否是动态组的成员。 [基于规则的动态成员资格](/azure/active-directory/users-groups-roles/groups-dynamic-membership)减少了添加和删除成员的管理开销。
- 创建 Microsoft 365 [组](/graph/api/resources/group?view=graph-rest-beta)时，通过在 **resourceBehaviorOptions** 属性中指定组的行为来仅限配置。 例如，允许成员发布、为新成员订阅对话、禁用欢迎电子邮件以及在 Outlook 体验中隐藏组。
- 在 **resourceProvisioningOptions** 属性中指定要提供的资源，这些资源通常不属于默认[组](/graph/api/resources/group?view=graph-rest-beta)创建的一部分。 当前支持使用 Microsoft Teams 功能将组作为[团队](/graph/api/resources/team?view=graph-rest-beta)进行配置。

### <a name="identity-and-access"></a>身份和访问
- 获取从 [directoryObject]() 派生的实体集合时，请应用 OData 系统查询选项（`$count`、`$filter`、`$search`）。 你可以[在这些实体的 **displayName** 和 **description** 属性中搜索特定标记](/graph/query-parameters?#using-search-on-directory-object-collections)，并使用 OData 强制转换将 **directoryObject** 的结果修剪为特定的派生类型。 有关详细信息，请参阅[使用 $count、$filter、$search 和 $orderby 在 Microsoft Graph 中生成高级查询](https://developer.microsoft.com/zh-CN/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/)。
- 作为[身份保护 API](/graph/api/resources/identityprotection-root?view=graph-rest-beta) 的一部分，请使用 **riskEventType** 属性来[获取检测到的风险类型](/graph/api/riskdetection-get?view=graph-rest-beta)或[获取用户历史记录中的风险类型](/graph/api/riskyuser-list-history?view=graph-rest-beta)。 不要使用 **riskType** 属性，因为它已被弃用。
- 在[条件集](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta)的 **clientAppTypes** 属性中为[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)指定客户端应用程序类型。
- 使用 `EntitlementManagement.Read.All` 的委派权限允许应用代表已登录的用户请求读取访问包及相关权利管理资源。
- 使用 `Application.Read.All` 和 `Application.ReadWrite.All` 的委派或应用程序权限来[列出组织中的应用程序](/graph/api/application-list?view=graph-rest-beta)。
- 使用 [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta) 资源类型控制 Azure AD 中的授权设置。

### <a name="teamwork"></a>团队合作
- [支持单点登录 (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) 的 Teams 应用可以在 [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta) 的 **azureADAppId** 属性中从 Teams 应用清单中指定 `WebApplicationInfo.id`。
- 使用[细粒度权限](/graph/permissions-reference#teams-resource-specific-consent-permissions)访问[团队](/graph/api/resources/team?view=graph-rest-beta)和[频道](/graph/api/resources/channel?view=graph-rest-beta)资源。


## <a name="april-2020-new-and-generally-available"></a>2020 年 4 月：新版本和正式版

### <a name="calendar"></a>日历
- 采用编程方式[共享或委派日历](outlook-share-or-delegate-calendar.md)，与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-1.0)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-1.0)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- [创建事件并作为联机会议更新](outlook-calendar-online-meetings.md)：
  - 对于每个**日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-1.0)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用**事件**的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的[已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。
- 将[高达 150MB 的文件附件](outlook-large-attachments.md)添加到[event](/graph/api/resources/event?view=graph-rest-1.0)。

### <a name="files"></a>文件
- [签出](/graph/api/driveitem-checkout?view=graph-rest-1.0)或[签入](/graph/api/driveitem-checkin?view=graph-rest-1.0)文件到 OneDrive，以管理更新文件并在更新就绪后向其他人提供更新。
- 应用可选的密码和到期日/时间作为[邀请](/graph/api/driveitem-invite?view=graph-rest-1.0)和[创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-1.0)操作的参数，以共享 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)。
- 获取或设置[权限](/graph/api/resources/permission?view=graph-rest-1.0)的密码和到期日/时间，并跟踪被授予共享 **driveItem** 权限的用户的 [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0)。
- 使用 **permission** 导航属性，获取[共享驱动器项](/graph/api/resources/shareddriveitem?view=graph-rest-1.0)的[权限](/graph/api/resources/permission?view=graph-rest-1.0)。
- 使用[共享链接](/graph/api/resources/sharinglink?view=graph-rest-1.0)将用户限制为只能在 OneDrive for Business 或 SharePoint 上查看共享 **driveItem** 的内容并且不能下载。

### <a name="identity-and-access"></a>身份和访问
- 若要在基于角色的访问控制（RBAC）提供程序中管理角色并分配资源访问权限，请使用 [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0)。 **unifiedRoleAssignmentMultiple** 资源支持在一系列作用域中定义单个角色，并将该角色分配给多个主体（例如用户）。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-1.0)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0)。 

### <a name="mail"></a>邮件
向 [message](/graph/api/resources/message?view=graph-rest-1.0) 添加了[高达 150MB 的文件附件](outlook-large-attachments.md)。

### <a name="sites-and-lists"></a>站点和列表
- [列出站点](/graph/api/sites-list-followed?view=graph-rest-1.0)，这些站点时已登录用户关注的。
- 通过使用 **dataLocationCode** 属性来确定[网站集](/graph/api/resources/sitecollection?view=graph-rest-1.0)的地理区域。
- 通过访问属于 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) 的 **sharepointIds** 的 **tenantId** 属性，在 SharePoint 上标识文件、文件夹或其他项目的租户。

## <a name="april-2020-new-in-preview-only"></a>2020 年 4 月：仅限预览版中的新增功能

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

将允许的用户和组指定为在通用打印（Microsoft 365 基于云的打印基础结构）上使用特定的[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta)。 若要体验可靠且集中的打印管理功能，并为打印用户提供简单而丰富安全的打印体验，请参阅[通用打印公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775)并加入其预览计划。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [4 月](changelog.md#april-2020)更新。

### <a name="groups"></a>组
通过组的应用 ID 识别创建[组](/graph/api/resources/group?view=graph-rest-beta)的应用。

### <a name="identity-and-access"></a>身份和访问
- [管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)[跟踪更改](/graph/api/administrativeunit-delta?view=graph-rest-beta)。
- [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta)[跟踪更改](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta)。
- [管理](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)用户的[身份验证方法](/graph/api/resources/authenticationmethod?view=graph-rest-beta)，其中包括[密码](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta)或[电话](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta)。 例如，[重置用户密码](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta)并[获取重置状态](/graph/api/authenticationoperation-get?view=graph-rest-beta)，或者为用户[添加电话号码](/graph/api/authentication-post-phonemethods?view=graph-rest-beta)以进行短信或语音通话身份验证（如果策略为用户启用）。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
[列出](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) Active Directory 联合身份验证服务中配置的[依赖方](https://docs.microsoft.com/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
查看 CSV 报告中的**会议创建**和**会议互动**数据，以查看[电子邮件活动计数](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)、[电子邮件活动用户计数](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)和[电子邮件活动用户详细信息](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)。


## <a name="march-2020-new-and-generally-available"></a>2020 年 3 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
- 获取呼叫路由和[呼叫](/graph/api/resources/call?view=graph-rest-1.0)的传入上下文。
- 对呼叫进行[录制状态更新](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0)。
- 可为[参与者](/graph/api/resources/participant?view=graph-rest-1.0)指定录制信息，包括录制的发起人和状态。
- 使用 **callChainId** 属性唯一标识会议或参与者到参与者[呼叫](/graph/api/resources/call?view=graph-rest-1.0)中的参与者。
- 可将参与者的国家/地区代码和终结点类型（例如 Skype for Business 或 Skype for Business VOIP）标识为 [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) 的组成部分。
- 第三方视频电话会议 (VTC) 设备合作伙伴可以通过云视频互操作 (CVI) 机器人和 [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0) 函数，记录并提供视频电话会议设备的媒体质量数据。 媒体质量数据包括，[音频](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0)、[视频](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0)和[屏幕共享](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0)的开放类型数据。

### <a name="files"></a>文件
- 与用户共享、添加至用户 OneDrive、或作为搜索结果返回的[远程项](/graph/api/resources/remoteitem?view=graph-rest-1.0)，包含图像或视频的元数据。
- [关注](/graph/api/driveitem-follow?view=graph-rest-1.0) [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-1.0)可停止关注驱动器项。
- 向用户[授予](/graph/api/permission-grant?view=graph-rest-1.0)访问共享链接的权限，以便共享相应的驱动器项。

### <a name="identity-and-access"></a>身份和访问
- [组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0)[跟踪更改](/graph/api/orgcontact-delta?view=graph-rest-1.0)。
- 使用 **riskEventTypes_v2** 属性可获取与[登录](/graph/api/resources/signin?view=graph-rest-1.0)相关的风险事件类型。
- 使用 `User.ManageIdentities.All` 委托的权限，可允许应用读取、更新或删除与登录用户有权访问的用户帐户关联的标识。 在没有登录用户的情况下，在应用程序级别使用此权限。 这样，应用可以[管理](/graph/api/user-update?view=graph-rest-1.0)用户能够使用哪些标识来登录。

### <a name="reports"></a>报告
将 Teams 服务管理员和 Teams 通信管理员用作接受的用户角色，允许应用代表用户以[用户委派的授权的形式](reportroot-authorization.md)读取 Microsoft 365 服务使用情况报告。 

### <a name="sites"></a>网站
- 让用户[关注](/graph/api/site-follow?view=graph-rest-1.0)或[取消关注](/graph/api/site-unfollow?view=graph-rest-1.0) SharePoint 网站。
- 针对 SharePoint [列表](/graph/api/resources/list?view=graph-rest-1.0)[订阅更改通知](/graph/api/resources/subscription?view=graph-rest-1.0)。 

## <a name="march-2020-new-in-preview-only"></a>2020 年 3 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
- 使用 **calendarGroupId** 属性可获取创建[日历](/graph/api/resources/calendar?view=graph-rest-beta)的[日历组](/graph/api/resources/calendargroup?view=graph-rest-beta)。
- 使用 **isDraft** 属性可将[事件](/graph/api/resources/event?view=graph-rest-beta)标识为用户已在 Outlook 中更新但尚未发送给更新与会者的会议。

### <a name="cloud-communications"></a>云通信
- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta) 按自定义外部 ID 获取[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)实例，并在不存在此实例时创建一个实例。
- 可选择使用 **externalId** 属性来标识具有自定义外部 ID 的联机会议。
- 使用可选的 `Accept-Language`HTTP 请求标头[创建](/graph/api/application-post-onlinemeetings?view=graph-rest-beta)或[获取](/graph/api/onlinemeeting-get?view=graph-rest-beta)联机会议实例，以在成功操作时，采用指定语言和区域设置显示 **joinInformation** 属性的内容。

### <a name="devices-and-apps"></a>设备和应用
Intune [3 月](changelog.md#march-2020)更新。

### <a name="identity-and-access"></a>标识和访问
- 使用 `Auditlogs.Read.All` 权限可列出[用户](/graph/api/resources/user?view=graph-rest-beta)的[登录活动](/graph/api/resources/signinactivity?view=graph-rest-beta)。
- 使用 [Azure 资源的 Privileged Identity Management (PIM)](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) 的 `PrivilegedAccess.Read.AzureResources` 应用程序级别权限为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。
- 使用 [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta) 实体可[获取](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta)或[更新](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta)预配置的默认安全设置，以保护组织免受常见攻击。
- 调用条件访问 API 时，请使用 `identity` 段。 例如，要[获取](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta)[条件性访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)：`GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`。
- 使用 **authenticationRequirement** 属性可获取通过所有登录步骤所需的最高级别的身份验证，以便[登录](/graph/api/resources/signin?view=graph-rest-beta)成功。
- 在[列出租户中发生的预配事件](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta)时，请使用分页。

### <a name="search"></a>搜索
- 若要将文件中的数据添加到搜索结果中，只需将数据作为 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 编制索引即可。 **externalFile** 类型已遭弃用。
- [更新](/graph/api/externalitem-update?view=graph-rest-beta)[索引中的项](/graph/api/resources/externalitem?view=graph-rest-beta)，具体方法为专门更新纯文本表示的项（用 **content** 属性表示），或项的属性包（用 **properties** 属性表示）。 由于更新属性包中的任何属性都会覆盖整个属性包，因此请务必在更新中显式添加项的所有属性。
- 在调用 **externalItem** 的 [create](/graph/api/externalconnection-put-items?view=graph-rest-beta)、[update](/graph/api/externalitem-update?view=graph-rest-beta) 或 [delete](/graph/api/externalitem-delete?view=graph-rest-beta) 操作后，检查 `HTTP 429` 和 `Retry-After` 响应头。 使用 `Retry-After` 延迟来回退请求是从[限制](throttling.md#best-practices-to-handle-throttling)中恢复的最快方法。

### <a name="teamwork"></a>团队合作
使用 `ChannelMessage.Read.All` 应用程序级别权限，在没有登录用户的情况下读取频道中的 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 实例。

### <a name="universal-print"></a>通用打印
调试允许用户在 web 上或从应用程序上打印的[通用打印 API](universal-print-concept-overview.md)。 借助 API，IT 管理员能够在 Microsoft 365 云远程打印机中管理用户和组对打印机的访问权限，以保持可用性、监视打印机状态，报告存档的打印作业和使用情况。 

注意：自 2020 年 3 月起，通用打印_服务_仅在个人预览版中提供。 参见[宣布推出通用打印：基于云的打印解决方案](https://aka.ms/announcinguniversalprint)，了解有关参与的详细信息。


## <a name="february-2020-new-and-generally-available"></a>2020 年 2 月：新版本和正式版

### <a name="calendar"></a>日历
浏览“[在共享或委派日历中创建事件](outlook-create-event-in-shared-delegated-calendar.md)”示例，或浏览可用于此流程期间的代理人、受邀者和日历所有者的操作与属性。

### <a name="identity-and-access"></a>身份和访问
- 为了提升在订阅“[更改用户通知](webhooks.md)”的安全性，强制在通知流程中使用的客户端和网站服务器上[强制执行传输层安全性（TLS）1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2)或更高。 新要求自 2020 年 2 月 15 日起分阶段推出。 到 2020 年 5 月 15 日，所有通知端点必须符合新的 TLS 要求。 [找出推出阶段](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/)，如有必要，请使用新的 **latestSupportedTlsVersion** 属性作为临时解决方法，以避免订阅失败，然后再完成 TLS 升级。
- 使用相应类型的[威胁评估请求](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0)跟踪[邮件](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0)、[电子邮件文件](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0)（.EML 文件）、[电子邮件附件文件](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0)（文本、Word 或二进制文件）或 [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0) 中的威胁。

### <a name="users"></a>用户
[重新处理](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0)[用户](/graph/api/resources/user?view=graph-rest-1.0)的所有基于组的许可证分配。


## <a name="february-2020-new-in-preview-only"></a>2020 年 2 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
参看“[管理日历共享和委派的预览版 API 所支持的任务](outlook-share-or-delegate-calendar.md)”。

### <a name="cloud-communications"></a>云通信

- 使用新的[通话记录](/graph/api/resources/callrecord?view=graph-rest-beta)资源，在 Microsoft Teams 和 Skype for Business 上为组织获取通话和联机会议的元数据。
- 对于会议中的参与者，请使用 **initiator** 属性获取[记录](/graph/api/resources/recordinginfo?view=graph-rest-beta)（如果有）的发起人的标识信息。

### <a name="devices-and-apps"></a>设备和应用
Intune [2 月](changelog.md#february-2020)更新。

### <a name="groups"></a>组
使用 [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta) 方法将产品（如 Microsoft 365 或企业移动性 + 安全性）的许可证分配给组。 由于 Azure AD 可确保将许可证分配给组的成员，因此加入或离开组的成员不再需要单独级别的许可证管理。

### <a name="identity-and-access"></a>身份和访问
- 创建[访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)时设置请求程序、审批和审阅设置。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-beta)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta)。 
- 使用应用程序级和委派的 `Policy.ReadWrite.ApplicationConfiguration` 权限，以读取和写入有关前一项中所述的应用程序配置[策略](/graph/api/resources/policy-overview?view=graph-rest-beta)的操作。

### <a name="teamwork"></a>团队合作
- 在组织中的所有频道消息或所有聊天消息中使用[更改通知](/graph/api/resources/webhooks?view=graph-rest-beta)。
- [拒绝](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta)与[团队](/graph/api/resources/team?view=graph-rest-beta)中的其他用户[换班的请求](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta)。

## <a name="january-2020-new-and-generally-available"></a>2020 年 1 月：新版本和正式版

### <a name="security"></a>安全性
作为客户警报管理的一部分，请使用 [update alert](/graph/api/alert-update?view=graph-rest-1.0) 方法并将“**注释**”字段更新为 `Closed in IPC` 或 `Closed in MCAS`。

### <a name="teamwork"></a>团队合作
使用“[团队](/graph/api/resources/team?view=graph-rest-1.0)”的 **primaryChannel** 导航属性来访问默认频道，“**常规**”。

### <a name="users"></a>用户
使用“**标识**”属性访问[用户](/graph/api/resources/user?view=graph-rest-1.0)可用于登录至 Azure AD 用户账户的一个或多个标识。 这些标识可由 Microsoft，组织或 Facebook、Google 或 Microsoft 等社交标识提供商提供。 此属性允许用户使用任一这些身份登录至用户账户。

## <a name="january-2020-new-in-preview"></a>2020 年 1 月：预览版新增功能

### <a name="devices-and-apps"></a>设备和应用
Intune [1 月](changelog.md#january-2020)更新。


## <a name="december-2019-new-and-generally-available"></a>2019 年 12 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
云通信 API 已正式发布，适用于[呼叫](/graph/api/resources/call?view=graph-rest-1.0)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-1.0)的 API [在 v1.0 中可用](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)。

### <a name="education"></a>教育
使用 **classSettings** 属性管理课程专属设置，例如启用发送每周作业摘要的操作。 当团队表示[教育课程](/graph/api/resources/educationclass?view=graph-rest-1.0)时，此属性可在[团队](/graph/api/resources/team?view=graph-rest-1.0)资源中使用。

### <a name="identity-and-access"></a>标识和访问 
[尝试使用有限权限获取容器对象会返回部分数据](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects)。 例如，与[用户](/graph/api/resources/user?view=graph-rest-1.0)、另一个**组**和[设备](/graph/api/resources/device?view=graph-rest-1.0)关联的[组](/graph/api/resources/group?view=graph-rest-1.0)实例。 只有 User.Read.All 和 Group.Read.All 权限且正在尝试访问此**组**实例的应用将获取**用户**和**组**实例，但获得的**设备**对象数据有限（仅限数据类型和对象 ID，不包括属性值）。

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
见解 API 已正式发布。 在生产应用中使用此 API 确定具有以下特征的相关文档：

- 用户的[常用文档](/graph/api/insights-list-trending?view=graph-rest-1.0)
- 用户[使用的](/graph/api/insights-list-used?view=graph-rest-1.0)文档
- [与用户共享由用户共享的](/graph/api/insights-list-shared?view=graph-rest-1.0)文档

### <a name="reports"></a>报告
要使用用户委派的权限获取 Microsoft 365 使用情况报告，管理员必须向该用户分配 Azure AD 受限管理员角色。 可以是以下角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、全局读取者或报告读取者。 有关详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](reportroot-authorization.md)。

### <a name="toolkit"></a>工具包
Microsoft Graph 工具包 v1.1 已发布。 有关增强功能和 bug 修复的列表，请参阅更改日历的[“2019 年 12 月”部分](changelog.md#december-2019)。

## <a name="december-2019-new-in-preview"></a>2019年12月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用新的[状态](/graph/api/resources/presence?view=graph-rest-beta)资源了解一名或多名用户的忙闲状态和当前活动。
- [删除](/graph/api/onlinemeeting-delete?view=graph-rest-beta)[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的实例。
- 要重命名和删除[呼叫](/graph/api/resources/call?view=graph-rest-beta)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的几个成员以便与这些资源的 v1 版本一致，请参阅更改日志的[“2019 年 12 月”部分](changelog.md#december-2019)。

### <a name="devices-and-apps"></a>设备和应用
Intune [12 月](changelog.md#december-2019)更新

### <a name="identity-and-access"></a>标识和访问 
- 修复了 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) 上 **appRoleAssignments** 和 **appRoleAssignedTo** 关系的行为。
- 使用 [Azure AD 权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)中的 [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) 来请求将资源添加到 [目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)中，以便可在[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta)中使用该资源的角色。
- 使用[威胁评估 API](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta) 帮助管理员报告可疑电子邮件、网络钓鱼 URL、电子邮件附件或其他文件。 然后，线程扫描判定会通知他们相应地调整组织策略。

### <a name="teamwork"></a>团队合作
- 针对[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)资源在 Microsoft 团队频道和聊天中[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。
- 针对新的或已更改的[频道消息或聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta)[订阅通知](/graph/api/resources/subscription?view=graph-rest-beta)。
- 借助 [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) 资源，可在[日程安排](/graph/api/resources/schedule?view=graph-rest-beta)中将用户的忙线状态指定为“已分配排班”。 作为用户的[设置](/graph/api/resources/usersettings?view=graph-rest-beta)的一部分获取或设置此信息。


## <a name="november-2019-new-and-generally-available"></a>2019 年 11 月：新版本和正式版

### <a name="groups"></a>组
- 使用委派或应用程序权限GroupMember.Read.All和GroupMember.ReadWrite.Al，来列出组、读取基本组属性，读取（并更新，如有读写权限）能够访问应用程序组的成员身份。
- 使用应用程序权限Group.Create，创建不含已登录用户的组。
- 对于指定的 [组](/graph/api/resources/group?view=graph-rest-1.0)，在其它组或目录角色中[检查成员身份](/graph/api/group-checkmemberobjects?view=graph-rest-1.0)。

### <a name="identity-and-access"></a>身份和访问
- 注册通过 Azure Active Directory (Azure AD) 进行身份验证的[应用程序](/graph/api/resources/application?view=graph-rest-1.0)。 根据需要使用委派的[权限](/graph/permissions-reference#application-resource-permissions)（即 Application.Read.All 和 Application.ReadWrite.All）或应用程序权限（即 Application.Read.All）。
- 对于指定的 [设备](/graph/api/resources/device?view=graph-rest-1.0)，在其它组或目录角色中[检查成员身份](/graph/api/device-checkmemberobjects?view=graph-rest-1.0)。

### <a name="mail"></a>邮件
- 使用 **conversationIndex** 属性可获取邮件在 Outlook 电子邮件对话中的位置。
- 使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来获取[邮件](/graph/api/resources/message?view=graph-rest-1.0)或[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0)资源，跟踪更改，并针对邮件的更改通知管理[订阅](/graph/api/resources/subscription?view=graph-rest-1.0)。

### <a name="users"></a>用户
- 针对指定的[用户](/graph/api/resources/user?view=graph-rest-1.0)，[检查组成员身份](/graph/api/user-checkmemberobjects?view=graph-rest-1.0)。
- 使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。

## <a name="november-2019-new-in-preview"></a>2019 年 11 月：预览版中的新增功能

### <a name="calendar"></a>日历
- [使用 Outlook 组织或参加联机会议](outlook-calendar-online-meetings.md)。
- [为](/graph/api/place-update?view=graph-rest-beta)[会议室](/graph/api/resources/room?view=graph-rest-beta)和[会议室列表](/graph/api/resources/roomlist?view=graph-rest-beta)的丰富位置类型设置属性。

### <a name="cloud-communication"></a>云通信
[呼叫](/graph/api/resources/call?view=graph-rest-beta) 资源类型支持以下附加功能：

- [传入呼叫上下文](/graph/api/resources/incomingcontext?view=graph-rest-beta)
- 参与者的终结点类型，例如语音邮件或Skype for Business
- [更新](/graph/api/call-updaterecordingstatus?view=graph-rest-beta)[参与者](/graph/api/resources/participant?view=graph-rest-beta)[录制](/graph/api/resources/recordinginfo?view=graph-rest-beta)信息的能力

### <a name="devices-and-apps"></a>设备和应用
Intune [11 月](changelog.md#november-2019)更新

### <a name="education"></a>教育
管理员能够通过与[类](/graph/api/resources/educationclass?view=graph-rest-beta)相关的[团队](/graph/api/resources/team?view=graph-rest-beta)  **classSettings** 属性启用全类设置。 .当前没有关于向监护人通知每周分配的设置。

### <a name="identity-and-access"></a>身份和访问
- 使用应用程序权限Policy.Read.All 读取组织的条件访问策略和命名位置，无需登录用户存在。
- 允许 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) 处于仅报告状态，`enabledForReportingButNotEnforced`。
- 使用委派权限ThreatAssessment.ReadWrite.All 或应用程序权限ThreatAssessment.Read.All，来读取（或创建，如果有读写权限）组织威胁存取请求。

### <a name="mail"></a>邮件
使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来管理更改[消息](/graph/api/resources/message?view=graph-rest-beta)资源更改通知的[订阅](/graph/api/resources/subscription?view=graph-rest-beta) 。

### <a name="notifications"></a>通知
使用新的轻量级通知 [Web SDK](https://aka.ms/GNSDK) 代替 [Project Rome SDK](https://github.com/Microsoft/project-rome)，以利用改进的身份验证模型和对使用 Web 推送的 Web 应用的支持。 

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
首次推出的[配置文件](/graph/api/resources/profile?view=graph-rest-beta)资源，这是 Microsoft 服务中下一代人脉实体的丰富表示形式。 此资源与常见和切实可行的人脉属性有关，包括任何有意义的日期（如[周年纪念日](/graph/api/resources/personanniversary?view=graph-rest-beta)）的信息、[教育](/graph/api/resources/educationalactivity?view=graph-rest-beta)、[就业岗位](/graph/api/resources/workposition?view=graph-rest-beta)、[兴趣](/graph/api/resources/personinterest?view=graph-rest-beta)、[语言](/graph/api/resources/languageproficiency?view=graph-rest-beta)和[技能](/graph/api/resources/skillproficiency?view=graph-rest-beta)熟练程度、[项目参与](/graph/api/resources/projectparticipation?view=graph-rest-beta)、[网站关联](/graph/api/resources/personwebsite?view=graph-rest-beta)以及其他[帐户](/graph/api/resources/useraccountinformation?view=graph-rest-beta)和联系人信息。

### <a name="search"></a>搜索
首次推出的 [Microsoft 搜索 API](search-concept-overview.md)，它使应用用户可以获得由 Microsoft Graph 支持的更多最新、个性化和相关的搜索结果。 使用[查询](/graph/api/search-query?view=graph-rest-beta)功能，该功能默认情况下在 Microsoft 云中搜索 Outlook 邮件和事件以及 OneDrive 和 SharePoint 文件。 使用 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)中的[连接器](/microsoftsearch/connectors-overview)，将搜索数据包括在 Microsoft 云外部。 或者，[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。

### <a name="teamwork"></a>团队合作
使用以下 HTTP 请求语法获取与[团队](/graph/api/resources/team?view=graph-rest-beta)和[频道](/graph/api/resources/channel?view=graph-rest-beta)相关的[文件](/graph/api/resources/driveitem?view=graph-rest-beta)资源：

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>用户
使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。


## <a name="october-2019-new-and-generally-available"></a>2019 年 10 月：新版本和正式版

### <a name="identity-and-access"></a>身份和访问
- 在生产应用中使用[组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0)。 组织联系人由组织管理员管理，可以从本地 Active Directory 或 Exchange Online 同步。
- 在[组织](/graph/api/resources/organization?view=graph-rest-1.0)中配置[基于证书的身份验证](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-1.0)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-1.0)。

### <a name="mail"></a>邮件
使用新的 **message** 参数更新[回复](/graph/api/message-reply?view=graph-rest-1.0)邮件时任何可写的 [message](/graph/api/resources/message?view=graph-rest-1.0) 属性，例如，[将收件人添加到回复](/graph/api/message-reply#example?view=graph-rest-1.0)。

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph 数据连接
开发人员和数据科学家现在可以使用[工具将 Office 365 数据转换为通用数据模型格式](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md)，从而使其与其他支持开放数据倡议 (ODI) 的数据集大致保持一致。 


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
- 使用 JavaScript SDK 中的混乱处理程序来验证应用程序是否可以应对棘手的服务器故障。
- 了解有关[使用 SDK 进行 API 调用](/graph/sdks/create-requests)的信息。

### <a name="users"></a>用户
- [获取](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0)或[设置](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0)[用户邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)的用户首选日期和时间格式设置。 
- 跟踪[用户](/graph/api/resources/user?view=graph-rest-1.0)上一次密码更改的日期/时间。

## <a name="october-2019-new-in-preview"></a>2019 年 10 月：预览版中的新增功能

### <a name="calendar"></a>日历
- 会议组织者可以[允许被邀请者提议备选会议时间](outlook-calendar-meeting-proposals.md)。 当收到包含建议的备选时间的会议响应时，组织者可以决定接受该建议并[更新](/graph/api/event-update?view=graph-rest-beta)会议时间。
- 编程日历共享与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-beta)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-beta)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-beta)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- 其他在线会议支持：
  - 对于每个**日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-beta)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用**事件**的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的[已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。

### <a name="devices-and-apps"></a>设备和应用
Intune [10 月](changelog.md#october-2019)更新

### <a name="graph-explorer"></a>Graph 浏览器
尝试使用[下一版本的 Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/preview)，并在新的“权限”****、“身份验证”**** 和“代码片段”**** 选项卡中查看权限、访问令牌和 SDK 代码片段等便捷的上下文信息。 使用“预览”**** 滑块在[生产](https://developer.microsoft.com/graph/graph-explorer)和 Graph Explorer 的新预览版本之间切换。

### <a name="groups"></a>组
- 使用 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性在 Outlook 用户界面的某些部分或 Outlook 客户端中控制[组](/graph/api/resources/group?view=graph-rest-beta)的可见性。
- [分配](/graph/api/group-assignlicense?view=graph-rest-beta)或删除[组](/graph/api/resources/group?view=graph-rest-beta)中用户的许可证。

### <a name="identity-and-access"></a>标识和访问
- 使用[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)自定义组织的访问规则。 这些规则会考虑有关用户或设备标识（如用户或组成员身份、IP 位置）的信号，以及尝试访问特定应用程序等行为和有风险的登录行为。
- 使用[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)来管理组织内外的用户对组、应用程序和 SharePoint Online 网站的访问。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-beta)和[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-beta)。
- 管理 Azure AD B2C [信任框架策略密钥](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta)。
- 定义 Azure AD B2C [用户流](/graph/api/resources/identityuserflow?view=graph-rest-beta)策略，用于登录、注册、合并注册和登录、密码重置和配置文件更新。
- 配置[信息保护标签](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)以对用户或租户的敏感度进行分类。
- 将 API 用于[标识风险事件](/graph/api/resources/identityriskevent?view=graph-rest-beta)的现有应用应转换为适用于 Azure AD Identity Protection 中[风险检测](/graph/api/resources/riskdetection?view=graph-rest-beta)的应用。 有关更多详细信息和弃用时间线，请参阅相关的[博客文章](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/)。


### <a name="mail"></a>邮件
通过创建[上载会话](/graph/api/resources/uploadsession?view=graph-rest-beta)，[将高达 150MB 的大文件附加到](outlook-large-attachments.md) [message](/graph/api/resources/message?view=graph-rest-beta) 实例，并迭代上载文件的范围，直至文件的所有字节都已上载。 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph 安全性 API
- 预览版与 RSA NetWitness、ServiceNow 和 Splunk 集成，以关联和同步[警报](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts)，并改善威胁防护和响应。
- 已将新触发器添加到适用于逻辑应用和流的 [Microsoft Graph 安全连接器](https://docs.microsoft.com/connectors/microsoftgraphsecurity/)和 [playbook](https://docs.microsoft.com/azure/security-center/security-center-playbooks) 中。 请参阅 [playbook 示例](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks)。
- 支持向 Microsoft Defender ATP 发送[威胁指示器](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview)，以使用其自己的智能源阻止威胁或发出威胁警报。 通过与 ThreatConnect 等合作伙伴集成，客户能够直接从威胁智能和自动化解决方案发送指示器。 

### <a name="notifications"></a>通知
- [创建通知并将其发送给用户登录的所有设备终结点上的所有应用程序客户端](/graph/api/user-post-notifications?view=graph-rest-beta)，而无需管理用户委派的权限。
- 在用户[通知](/graph/api/resources/notification?view=graph-rest-beta)上使用[目标策略终结点](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta)，以便专门针对 Windows、iOS、Android 或 WebPush 平台投放通知。
- 在 iOS 终结点的通知上指定[回退策略](/graph/api/resources/fallbackpolicy?view=graph-rest-beta)，以便发送由于平台特定的限制（如节电模式）而可能无法传递到设备的高优先级原始通知。

 
### <a name="powershell-sdk"></a>PowerShell SDK 
开发人员和 IT 专业人员会注意到推出了 [Microsoft Graph Powershell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell)，该 SDK 将生成包含用于发出 Microsoft Graph REST API 请求的 cmdlet 的模块。

## <a name="september-2019-new-and-generally-available"></a>2019 年 9 月：新版本和正式版

### <a name="calendar-mail-and-group"></a>日历、邮件和组
[获取文件的原始内容或项目的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)，该项目已作为[附件](/graph/api/resources/attachment?view=graph-rest-1.0)添加到[事件](/graph/api/resources/event?view=graph-rest-1.0)、[邮件](/graph/api/resources/message?view=graph-rest-1.0)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0)。

### <a name="calendar-mail-outlook-task-personal-contact"></a>日历、邮件、Outlook 任务、个人联系人
使用 [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0) 函数在受支持的[格式](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)之间转换 Outlook 项目 ID，包括 Microsoft Graph 默认 ID 格式和不可变的 ID 格式。 

以下资源支持 ID 格式转换：

- [附件](/graph/api/resources/attachment?view=graph-rest-1.0)
- [联系人](/graph/api/resources/contact?view=graph-rest-1.0)
- [事件](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [邮件](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>邮件
[获取邮件的 MIME 内容](outlook-get-mime-message.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
使用 [Microsoft Graph 工具包](toolkit/overview.md)开发生产应用，该应用提供一致的 Microsoft 365 外观，可以节省从 Microsoft Graph 进行身份验证和访问数据的时间。

## <a name="september-2019-new-in-preview"></a>2019 年 9 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [9 月](changelog.md#september-2019)更新

### <a name="files"></a>文件
- 增强的同步支持：

  - 使用新的 **pendingOperations** 属性标识可能影响 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 的二进制内容的操作。
  - [还原](/graph/api/driveitem-restore?view=graph-rest-beta)已删除的 **driveItem**。 
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file?view=graph-rest-beta)数据安全性和完整性。
- 获取或设置[照片](/graph/api/resources/photo?view=graph-rest-beta)的方向。 OneDrive 个人版上支持设置。

### <a name="identity-and-access"></a>标识和访问
- 使用新的 **identities** 属性并获取[用户](/graph/api/resources/user?view=graph-rest-beta)可用于登录帐户的标识。 这些标识可由组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 用于在租户的云应用程序中[同步标识](/graph/api/resources/synchronization-overview?view=graph-rest-beta)的增强功能：

  - 存储[同步作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)的设置
  - 指定对同步作业施加[隔离](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta)的原因

### <a name="teamwork"></a>团队合作
使用[团队](/graph/api/resources/team?view=graph-rest-beta)的**常规**频道或自定义[成员设置](/graph/api/resources/teammembersettings?view=graph-rest-beta)，让团队成员在**团队**中创建专用频道。

### <a name="users"></a>用户
- 获取或更新[用户](/graph/api/resources/user?view=graph-rest-beta)用于登录帐户的标识。 这些标识可由商业组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta)。


## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月：新版本和正式版 

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)。
- 在[获取组活动详细信息](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)时，跟踪 Microsoft 365 组 ID。
- 在获取 [OneDrive 使用帐户详细信息](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)和 [SharePoint 网站使用情况详细信息](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)时，跟踪所有者主体名称。
- 在[获取每 Microsoft 365 服务的用户计数报告](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)时，获取 Microsoft 365 上的活动和非活动用户数。

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
最终用户可以使用 Microsoft 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) 应用获取与管理时间、工作协作和工作生活平衡有关的见解。 现在，你可以使用[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) 整合与工作活动（如呼叫、聊天和电子邮件）所花时间相关的数据、以帮助提高用户的工作效率和幸福感。 


## <a name="july-2019-new-and-generally-available"></a>2019 年 7 月：新版本和正式版 

### <a name="example-code-snippets"></a>代码片段示例
现在 v1.0 和 beta 参考中的所有 API 主题中提供了 Objective-C 代码片段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)的 Objective-C 示例。

### <a name="group"></a>Group
- 使用 [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) 函数确保现有 Microsoft 365 组的显示名称和邮件昵称符合命名策略。
- 或者，在创建组之前，可以为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 使用 [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) 函数来首先验证名称。

### <a name="identity-and-access"></a>身份和访问
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-1.0)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0)。
- 使用[新的委派和应用程序权限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_，对于公司目录中的与角色的访问控制 (RBAC)：

  - 使用读取/写入权限来首先[激活](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0)目录角色。 
  - 激活角色之后，可以使用读取权限来[读取目录角色](/graph/api/directoryrole-list?view=graph-rest-1.0)、[列出角色成员](/graph/api/directoryrole-list-members?view=graph-rest-1.0)和[列出目录角色模板](/graph/api/directoryroletemplate-list?view=graph-rest-1.0)。 
  - 还可以使用读取/写入权限来[添加](/graph/api/directoryrole-post-members?view=graph-rest-1.0)和[删除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0)角色成员。


## <a name="july-2019-new-in-preview"></a>2019 年 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="calendar"></a>日历 
按照 Exchange Online 管理员的设置，使用新的[位置 API](/graph/api/resources/place?view=graph-rest-beta) 来使用诸如 [room](/graph/api/resources/room?view=graph-rest-beta) 和 [room list](/graph/api/resources/roomlist?view=graph-rest-beta) 之类的富位置类型。

### <a name="devices-and-apps"></a>设备和应用
Intune [7 月](changelog.md#july-2019)更新

### <a name="files"></a>文件 
在为文件、文件夹或其他 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) [创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-beta)时，应用到期日期/时间或密码。

### <a name="identity-and-access"></a>标识和访问
- 使用[新的应用程序权限](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ 对[访问权限审阅](/graph/api/resources/accessreviews-root?view=graph-rest-beta)执行 CRUD 操作。 
- 使用[新的委派和应用程序权限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以分别读取或写入（包括创建、更新、删除或管理成员身份）[管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)资源。
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-beta)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta)。
- 使用新的 [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta) 函数查找最新的目录[同步架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)，以便将目录对象、属性及类型同步到应用。
- 使用[功能推出策略](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta)帮助租户管理员在为整个组织启用一些功能之前，针对特定组试用这些功能。

### <a name="mail"></a>邮件
使用更精确的应用程序权限 _Mail.ReadBasic.All_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 现适用于 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 以及针对[邮件](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的[更改跟踪](delta-query-overview.md)

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)。

### <a name="teamwork"></a>团队合作
- 为用户[安装](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)、[卸载](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta)、[升级](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)和[列出已安装的 Microsoft Teams 应用](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta)。
- 使用仅应用访问权限来读取频道消息、频道消息回复以及聊天中的消息。 [请求和批准](teams-protected-apis.md)此类访问。

## <a name="may---june-2019-new-and-generally-available"></a>2019 年 5 月 - 7 月：新版本和正式版

### <a name="calendar-mail-and-personal-contacts"></a>日历、邮件和个人联系人
Exchange 管理员可以向应用程序授予应用程序权限, 并[限制该应用仅访问邮箱 ](auth-limit-mailbox-access.md) 的子集, 而不是默认的访问组织中的所有邮箱。 此类受限访问适用于授予[日历](permissions-reference.md#calendars-permissions)、 [联系人](permissions-reference.md#contacts-permissions)及[邮件和邮箱设置](permissions-reference.md#mail-permissions)的应用的任何应用程序权限。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)。

### <a name="mail"></a>邮件
使用[邮件搜索文件夹](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API 来搜索邮件, 并访问 Outlook 电子邮件搜索结果。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)。

### <a name="postman"></a>Postman
除 Graph 资源管理器外, 请在[Microsoft Graph Postman 集合](use-postman.md)中试用 Microsoft Graph API, 了解 API 行为并加速应用程序开发。

### <a name="tutorials"></a>教程
尝试使用新[教程构建 Java 控制台应用](/graph/tutorials/java) , 以获取有关用户日历的信息。

### <a name="user"></a>用户
管理员或用户可以[吊销](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)用户的所有已颁发的刷新令牌。 通常用于防止已丢失或被盗设备上的应用访问组织的数据。


## <a name="may---june-2019-new-in-preview"></a>2019 年 5 月 - 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
- Intune [5月](changelog.md#may-2019)更新 
- Intune [6月](changelog.md#june-2019)更新

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta)的增量查询。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta)的增量查询和属性添加。 

### <a name="group"></a>Group
获取[敏感度标签](/graph/api/resources/assignedlabel?view=graph-rest-beta)，帮助保护 Microsoft 365 组的敏感数据并满足合规性策略。 这些标签是[assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta)对象，由 Microsoft 365 安全与合规性中心的管理员发布，作为 Microsoft 信息保护功能的一部分。 

### <a name="identity-and-access"></a>身份和访问控制
- 获取[应用程序](/graph/api/resources/applicationtemplate?view=graph-rest-beta)的实例，或将 Azure AD 应用程序库中的实例作为模板添加到目录中。
- 获取租户中所有[预配事件](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)目录的列表。
- 获取有关 Azure AD 环境中[检测到的用户或登录风险](/graph/api/resources/riskdetection?view=graph-rest-beta)的信息。 此风险检测功能是 Azure AD 标识保护的一部分。

### <a name="mail"></a>邮件
使用更精确的代理权限 _Mail.ReadBasic_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 可用于读取 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 方法和更改 [message](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的 [跟踪](delta-query-overview.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
[Microsoft Graph 工具包](/graph/toolkit/overview)是一组框架不可知的 web 组件和帮助器, 提供对 Microsoft Graph 中的数据进行身份验证和访问的便利。  由于 Microsoft Graph 工具包处于预览状态，请仅在非生产应用中使用工具包提供程序和组件。

### <a name="reports"></a>报告
- 获取组织中用户采用的[身份验证方法的报告](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta)，例如自助服务密码重置和多因素身份验证 (MFA).。

### <a name="sites"></a>网站
让用户[关注](/graph/api/site-follow?view=graph-rest-beta)或[取消关注](/graph/api/site-unfollow?view=graph-rest-beta) SharePoint 网站。

### <a name="teamwork"></a>团队合作
- 在 Microsoft 团队[聊天消息](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)中存储[图像](/graph/api/resources/chatmessage?view=graph-rest-beta)。 
- 支持[配置](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)私人团队的发现方式。


## <a name="january---april-2019-new-and-generally-available"></a>2019 年 1 月 - 4 月：新版本和正式版

[Microsoft Graph 数据连接](data-connect-concept-overview.md)

### <a name="calendar"></a>日历
[获取忙/闲日程安排](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>身份和访问控制
[身份提供程序](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[改进的身份验证指南](/graph/auth)
[将应用从 Azure AD Graph 迁移到 Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>SDK
[SDK 指南](/sdks/sdks-overview.md) API 片段（[示例](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code)）

### <a name="security"></a>安全性
[租户安全功能分数](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>2019 年 1 月 - 4 月：预览版中的新功能

### <a name="calendar-group-mail-to-do-tasks"></a>日历、群组、邮件、待办任务
[获取事件、消息、Outlook 任务或组帖子中文件或项目附件的原始/MIME 内容](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)

### <a name="change-notifications"></a>更改通知
[减少 Outlook 资源的缺失更改通知](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>设备和应用
- Intune [1 月](changelog.md#january-2019)更新 
- Intune [2 月](changelog.md#february-2019)更新
- Intune [3 月](changelog.md#march-2019)更新
- Intune [4 月](changelog.md#april-2019)更新

### <a name="files"></a>文件
[共享邀请](/graph/api/driveitem-invite?view=graph-rest-beta)包含过期时间和密码

### <a name="financials"></a>财务
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>身份和访问控制
[访问评审](/graph/api/resources/accessreviews-root?view=graph-rest-beta)支持应用程序权限[审核和登录日志](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Azure AD B2C 中的自定义注册和登录](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[存在风险的用户](/graph/api/resources/riskyuser?view=graph-rest-beta)和[历史记录](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>邮件
[获取消息的 MIME 内容](outlook-get-mime-message.md)

### <a name="reports"></a>报表
[应用程序登录报表](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>安全性
[安全操作](/graph/api/resources/securityaction?view=graph-rest-beta)
[威胁指示器](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>团队合作
[一对一聊天](/graph/api/resources/chat?view=graph-rest-beta)
[排班管理](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>另请参阅
- 请参阅 Microsoft Graph 中的[新增功能](whats-new-overview.md)。
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。