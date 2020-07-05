---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d0e462ab93b60796e8cbb4463c19799ba9033cd2
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038644"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的和[六月和六月份](changelog.md#june-2020)[部分。](changelog.md#may-2020) 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="july-2020-new-and-generally-available"></a>2020年7月：新的和普遍可用

### <a name="change-notifications"></a>更改通知
从[changeNotification](/graph/api/resources/changenotification)资源中删除了 erronously 引入的**sequenceNumber**属性。

## <a name="july-2020-new-in-preview-only"></a>2020年7月：仅预览中的新内容

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
使用应用程序权限 `Printer.ReadWrite.All` 和[Internet 打印协议（IPP）编码](https://tools.ietf.org/html/rfc8010)[更新打印机](/graph/api/printer-update?view=graph-rest-beta)。

## <a name="june-2020-new-and-generally-available"></a>2020年6月：新的和普遍可用的

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
- `Accept-Language`[创建联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)时使用 HTTP 标头，以提供基于区域设置的联接信息。
- 使用[createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0)返回具有指定的**externalId**值的联机会议; 或者，如果尚不存在，则创建一个，以便简化在第三方日历中嵌入结果会议。

### <a name="files"></a>文件
- 增强的同步支持：
  - 使用**pendingOperations**属性可标识任何可能更新[driveItem](/graph/api/resources/driveitem)文件的二进制内容的操作，这些[操作](/graph/api/resources/pendingoperations)会挂起完成。
  - [还原](/graph/api/driveitem-restore)已删除且位于 OneDrive 个人版的回收站中的**driveItem** 。
- 获取或设置[照片](/graph/api/resources/photo)的方向。 OneDrive 个人版上支持设置。
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file)数据安全性和完整性。
- 在将 `deferCommit` [文件上载](/graph/api/driveitem-createuploadsession)到 OneDrive for business 时，使用参数推迟最终创建，直到应用程序发出请求来完成上载。
- 使用**fileSize**属性可作为**项目**参数的一部分提供估计，以便在 OneDrive 个人版上上[传文件](/graph/api/driveitem-createuploadsession)之前执行配额检查。
- 通过[drive](/graph/api/resources/drive)资源的**Quota**属性查找[storagePlanInformation](/graph/api/resources/storageplaninformation) ，以查看是否有更高的可用存储配额计划。

### <a name="groups"></a>组
使用应用程序权限 `Group.Read.All` ，并 `Group.ReadWrite.All` 获取组[对话](/graph/api/resources/conversation)和[会话线程](/graph/api/resources/conversationthread)资源。

### <a name="identity-and-access"></a>身份和访问 
- 用于[标识保护](/graph/api/resources/identityprotectionroot)的两组 API GA：[风险检测](/graph/api/resources/riskdetection)和有[风险的用户](/graph/api/resources/riskyuser)api。

### <a name="security"></a>安全性
- 将以下内容作为[警报](/graph/api/resources/alert?view=graph-rest-1.0)的属性进行跟踪：
  - 与警报相关的事件的 Id。
  - 将[资源](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values)标识为 "受攻击" 或 "作为警报中的相关资源"。
  - 指定与警报相关的[网络连接](/graph/api/resources/networkconnection?view=graph-rest-1.0)的源和目标位置。

### <a name="sites-and-lists"></a>网站和列表
在 SharePoint[列表](/graph/api/resources/list)资源的[列定义](/graph/api/resources/columndefinition)中指定地理位置数据。

### <a name="teamwork"></a>团队合作
- 使用委派的权限[AppCatalog](/graph/permissions-reference#appcatalog-resource-permissions)列出 Microsoft 团队应用程序目录中的[应用程序](/graph/api/resources/teamsapp?view=graph-rest-1.0)。
- [获取有关](/graph/api/channel-get-filesfolder)映射到 "团队[频道](/graph/api/resources/channel)的**文件**" 选项卡的文件夹的信息。
- 获取[团队](/graph/api/resources/team)的[默认频道](/graph/api/team-get-primarychannel)（标记为 "**常规**"）。


## <a name="june-2020-new-in-preview-only"></a>2020年6月：仅预览中的新内容

### <a name="calendar"></a>日历
除了跟踪**calendarView**中事件的增量更改（集合或由开始_和_结束日期分隔的事件），可对用户邮箱中的事件或特定用户日历中的事件使用[delta](/graph/api/event-delta?view=graph-rest-beta)函数。

### <a name="cloud-communications--presence"></a>云通信 |Shell
获取组织中的所有用户或 grgr 中的特定用户[的状态](/graph/api/presence-get?view=graph-rest-beta)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 在配置[要打印的文档](/graph/api/resources/printdocument?view=graph-rest-beta)时指定[打印边距](/graph/api/resources/printmargin?view=graph-rest-beta)。
- 支持以下[打印机功能](/graph/api/resources/printercapabilities?view=graph-rest-beta)：
  - 送纸方向
  - 打印页面范围
  - 以 DPI 显示的打印分辨率
  - 最大打印作业队列大小（字节数）
  - 输入纸盒
  - 边距
  - 排序
  - 文档缩放
- 支持打印分辨率（DPI）和文档缩放作为[默认打印机设置](/graph/api/resources/printerdefaults?view=graph-rest-beta)的一部分。
- 对以下[文档配置](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta)设置的支持：
  - 输入纸盒
  - 输出箱
  - 媒体大小
  - 边距
  - 媒体类型
  - finishings，例如装订或绑定
  - 每版打印页数
  - 多页布局，指定在每个工作表中排列页面的方向
  - 排序
  - 能力
- 在[列出 pring 作业](/graph/api/printer-list-jobs?view=graph-rest-beta)时展开文档。
- [注册打印机]()并使用[printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta)资源来跟踪和验证打印机的注册。
- 在当前用户或应用程序的租户内[获取长时间运行的打印机注册操作](/graph/api/printoperation-get?view=graph-rest-beta)。
- 属性和枚举类型的几个重命名-请参阅[六月](changelog.md#june-2020)更改日志 updates for cloud 打印中的详细信息。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
测试版中的 Intune[六月](changelog.md#june-2020)更新。

### <a name="education"></a>教育
- 可以使用委派权限 `EduRoster.ReadBasic` [获取](/graph/api/educationuser-get?view=graph-rest-beta)外部源程序中[教师](/graph/api/resources/educationteacher?view=graph-rest-beta)或[学生](/graph/api/resources/educationstudent?view=graph-rest-beta)的 ID，作为**externalId**属性。
- **externalSource** `lms` 如果教育[组织](/graph/api/resources/educationorganization?view=graph-rest-beta)或[课程](/graph/api/resources/educationclass?view=graph-rest-beta)是从学习管理系统（LMS）创建的，则使用 externalSource 属性来跟踪该值。

### <a name="identity-and-access"></a>身份和访问
- IT 专业人员可以使用轻型代理连接到[AZURE AD 应用程序代理](/azure/active-directory/manage-apps/what-is-application-proxy)的[连接器](/graph/api/resources/connector?view=graph-rest-beta)资源，并[在外部发布本地 web 应用程序应用](/graph/api/resources/onpremisespublishing?view=graph-rest-beta)，以便其组织的远程用户能够以安全的方式访问这些应用程序。
- 在租户级别管理[身份验证策略](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta)，以启用或禁用外部用户的[自助服务注册](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta)。
- [根据需要预配用户帐户](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta)，并能够指定要执行的预配和同步规则的对象。

### <a name="search"></a>搜索
- 对[架构](/graph/api/resources/schema?view=graph-rest-beta)中的[属性](/graph/api/resources/property?view=graph-rest-beta)使用增强功能： **isRefinable**以启用对搜索结果的筛选以及更精确地控制搜索体验，以及**别名**和**标签**以实现更好的相关性。
- 能够在**架构**中指定最大为128的**属性**资源。
- 将[Get externalItem](/graph/api/externalitem-get?view=graph-rest-beta)用于诊断目的。

### <a name="users"></a>用户
- 使用[mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta)的**userPurpose**属性可在 Exchange Online 中识别共享邮箱和设备邮箱中单个用户的邮箱并区分该邮箱。 
- 使用[用户设置](/graph/api/resources/usersettings?view=graph-rest-beta)[获取](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta)或[更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta)[首选 languaes 和区域设置](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta)。
- 用户设置是通过点击 Azure AD 用户配置文件以反映相同的用户首选项的[用户](/graph/api/resources/user?view=graph-rest-beta)可访问的关系，可实现跨应用程序的一致用户体验。 查看[用户设置如何区分邮箱设置](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册[microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，获取免费的 microsoft 365 订阅，然后开始开发！


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

