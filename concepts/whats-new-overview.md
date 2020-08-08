---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 85c3a540c6aa2f0c7f3b00bf86a3e727997743b3
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589142"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="july-2020-new-and-generally-available"></a>2020 年 7 月：新版本和正式版

### <a name="calendar"></a>日历
正式发布一项功能，它允许组织者接受备选会议时间提案，并允许受邀者在[暂时接受](/graph/api/event-tentativelyaccept?view=graph-rest-1.0)或[拒绝](/graph/api/event-decline?view=graph-rest-1.0)事件时[为会议建议新时间](outlook-calendar-meeting-proposals.md)。

### <a name="change-notifications"></a>更改通知
已删除从 [changeNotification](/graph/api/resources/changenotification) 类型中错误引入的 **sequenceNumber** 资源。

### <a name="groups"></a>组
[group](/graph/api/resources/group?view=graph-rest-v1.0) 实体下列属性的通用版本：**assignedLabels**、**expirationDateTime**、**membershipRule**、**membershipRuleProcessingState**、**preferredLanguage** 和 **theme**。

### <a name="identity-and-access"></a>身份和访问
- 删除作为[设备](/graph/api/resources/device)的注册所有者或用户的用户。
- 跟踪对新创建、更新或删除的应用程序本地表示形式（由 [servicePrincipals](/graph/api/resources/serviceprincipal) 资源表示）和委派权限授予（由 [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant) 资源表示）的更改，而无需对整个资源集合执行完全读取操作。
- 正式发布[用于强制安全性默认设置的策略](/graph/api/resources/identitysecuritydefaultsenforcementpolicy)，可以保护组织免受常见攻击。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 正式发布[条件访问策略](/graph/api/resources/conditionalAccessPolicy)，它们是用于定义访问方案的自定义规则。
- 正式发布表示自定义规则的[命名位置](/graph/api/resources/namedLocation)，用于定义在条件访问策略中使用的网络位置。

### <a name="schema-extensions"></a>架构扩展
[架构扩展](/graph/api/resources/schemaextension)功能现在可在[Microsoft Cloud for US Government](/graph/deployments)使用。

### <a name="teamwork"></a>团队合作
使用 `TeamsAppInstallation.ReadForTeam` 或 `TeamsAppInstallation.ReadWriteForTeam` 的委派权限，或者使用 `TeamsAppInstallation.ReadForTeam.All` 或 `TeamsAppInstallation.ReadWriteForTeam.All` 的应用程序权限来[列出已在团队中安装的应用](/graph/api/teamsappinstallation-list)。

## <a name="july-2020-new-in-preview-only"></a>2020 年 7 月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用[更新](/graph/api/onlinemeeting-update?view=graph-rest-beta)操作来更新[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)的 **startDateTime**、**endDateTime**、**participants** 或 **subject** 属性。
- 订阅有关 Microsoft Teams 上用户可用性更改的通知，如[状态](/graph/api/resources/presence?view=graph-rest-beta)资源所示。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- [获取](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta)公用电话交换网 (PSTN) 通话的记录。
- [获取](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta)直接路由通话的记录。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
首次推出的[电子数据展示事例](/graph/api/resources/ediscoverycase?view=graph-rest-beta)包含可在法律案件中作为证据的保管人、保留、集合、管理审阅集和导出。
应用现在可以对收集用于诉讼、调查或法规请求的[审阅集数据](/graph/api/resources/reviewset?view=graph-rest-beta)进行[查询](/graph/api/resources/reviewsetquery?view=graph-rest-beta)和挑选。 这一首次推出的内容是 Microsoft 365 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide)的一部分。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 使用应用程序权限 `Printer.ReadWrite.All` 和 [Internet 打印协议（IPP）编码](https://tools.ietf.org/html/rfc8010)至[更新打印机](/graph/api/printer-update?view=graph-rest-beta)。
- 使用以下应用权限之一、`PrintJob.ReadBasic.All`、`PrintJob.Read.All`、`PrintJob.ReadWriteBasic.All` 或 `PrintJob.ReadWrite.All`，来[获取打印作业](/graph/api/printjob-get?view=graph-rest-beta)或[列出打印机打印作业](/graph/api/printer-list-jobs?view=graph-rest-beta)。
- [获取打印作业](/graph/api/printjob-get?view=graph-rest-beta)时，请使用 `$expand` 获取对作业正在执行或已执行的[打印作业](/graph/api/resources/printtask?view=graph-rest-beta)。 [截取打印](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing)中使用打印任务、[任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta)、和[任务触发器](/graph/api/resources/printtasktrigger?view=graph-rest-beta)。
- [重定向打印作业](/graph/api/printjob-redirect?view=graph-rest-beta)至其他打印机，作为截取打印的组成部分。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [7 月](changelog.md#july-2020)试用版更新。

### <a name="groups"></a>组
使用 Microsoft 365 [组](/graph/api/resources/group?view=graph-rest-beta)的 **isAssignableToRole** 属性，并在创建组的过程中对其进行设置，以指示该组是否可以分配给 Azure AD 角色。 这[有助于在 Azure AD 中管理角色分配](/azure/active-directory/users-groups-roles/roles-groups-concept)，例如特权角色管理员或全局管理员可以创建 Microsoft 365 组并向该组分配 Azure AD 角色，而不是向单个用户分配这一角色，这样一来，用户加入该_组_后，他们会被间接分配既定角色。

### <a name="identity-and-access"></a>身份和访问
- [获取访问令牌](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta)，以授权 Azure AD 预配服务将用户预配到应用程序。
- [获取](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta)或[更新](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta)权限管理设置，这些设置控制对组织内部和外部用户的组、应用程序和 SharePoint Online 网站的访问权限。 

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 将用户风险级别（`low`、`medium`、`high`、`none`）包含为应用 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)的注意事项。
- [使用密码更改作为授予控制](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control)，以便传递条件访问策略。
- 在 Azure AD 租户和 Azure AD B2C 租户中，将 [OpenID Connect 提供程序](/graph/api/resources/openidconnectprovider?view=graph-rest-beta) (OIDC) 用作标识提供程序。 其 **claimsMapping** 属性允许 Azure AD 将 OIDC 提供程序的[声明映射](/graph/api/resources/claimsmapping?view=graph-rest-beta)到 Azure AD 可识别和使用的声明。

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能|见解
在 Microsoft 365 中，对[项见解](/graph/api/resources/iteminsights?view=graph-rest-beta)的可用性和显示进行更[精细的隐私控制](insights-customize-item-insights-privacy.md)。 这些见解表示 OneDrive for Business 中的用户和文档之间的关系，并使用高级分析和机器学习技术进行计算。 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>人脉和工作区智能 | 个人资料卡片自定义
管理员可以使用[个人资料卡属性](/graph/api/resources/profilecardproperty?view=graph-rest-beta) API，[自定义显示在组织个人资料卡上的属性](add-properties-profilecard.md)。

### <a name="sites-and-lists"></a>网站和列表
访问 SharePoint [术语库](/graph/api/resources/termstore-store?view=graph-rest-beta)分类系统，该系统的层次结构包括 [group](/graph/api/resources/termstore-group?view=graph-rest-beta)、[set](/graph/api/resources/termstore-set?view=graph-rest-beta) 和 [term](/graph/api/resources/termstore-term?view=graph-rest-beta) 资源，以及术语之间的 [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta) 资源。

### <a name="workbooks-and-charts"></a>工作簿和图表
[获取[工作簿](/graph/api/resources/workbook?view=graph-rest-beta)中长时间运行[操作](/graph/api/resources/workbookoperation?view=graph-rest-beta)的状态和任何结果](/graph/api/workbookoperation-get?view=graph-rest-beta)。

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


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

