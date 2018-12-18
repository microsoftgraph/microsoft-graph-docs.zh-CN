---
title: 用户资源类型
description: 表示 Azure AD 用户帐户。继承自 directoryObject。
author: dkershaw10
ms.openlocfilehash: c9d776091bba18a9459505b7d35d7ff15479cffe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348200"
---
# <a name="user-resource-type"></a>用户资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 将您自己的数据添加到自定义属性，作为[扩展](/graph/extensibility-overview)。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
|[List users](../api/user-list.md) |[user](user.md) 集合| 获取用户对象列表。|
|[Create user](../api/user-post-users.md) |[user](user.md)| 新建用户对象。|
|[Get user](../api/user-get.md) | [user](user.md) |读取 user 对象的属性和关系。|
|[Update user](../api/user-update.md) | [user](user.md) |更新 user 对象。 |
|[Delete user](../api/user-delete.md) | 无 |删除 user 对象。 |
|[List messages](../api/user-list-messages.md) |[Message](message.md) collection| 获取已登录用户的邮箱中的所有邮件。|
|[Create Message](../api/user-post-messages.md) |[Message](message.md)| 通过发布到邮件集合中创建一条消息。|
|[List mailFolders](../api/user-list-mailfolders.md) |[MailFolder](mailfolder.md) collection| 在已登录用户的根文件夹下获取邮件文件夹集合。 |
|[Create mailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 mailFolders 集合创建新 MailFolder。|
|[sendMail](../api/user-sendmail.md)|None|发送请求正文中指定的邮件。|
|[List events](../api/user-list-events.md) |[Event](event.md) collection| 获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/user-post-events.md) |[Event](event.md)| 通过发布到事件集合创建新事件。|
|[List calendars](../api/user-list-calendars.md) |[Calendar](calendar.md) collection| 获取 Calendar 对象集合。|
|[Create calendar](../api/user-post-calendars.md) |[Calendar](calendar.md)| 通过发布到日历集合创建新日历。|
|[List calendarGroups](../api/user-list-calendargroups.md) |[CalendarGroup](calendargroup.md) collection| 获取 CalendarGroup 对象集合。|
|[Create calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| 通过发布到 calendarGroups 集合新建 CalendarGroup。|
|[List calendarView](../api/user-list-calendarview.md) |[Event](event.md) collection| 获取一个事件对象集合。|
|[List contacts](../api/user-list-contacts.md) |[Contact](contact.md) collection| 从已登录用户的默认联系人文件夹中获取联系人集合。|
|[Create Contact](../api/user-post-contacts.md) |[Contact](contact.md)| 通过发布到联系人集合新建联系人。|
|[List contactFolders](../api/user-list-contactfolders.md) |[ContactFolder](contactfolder.md) collection| 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。|
|[Create ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| 通过发布到 contactFolders 集合创建新 ContactFolder。|
|[List directReports](../api/user-list-directreports.md) |[directoryObject](directoryobject.md) collection| 从 directReports 导航属性中获取向此用户报告的用户和联系人。|
|[List manager](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | 从 manager 导航属性中获取是此用户的经理的用户或联系人。|
|[List memberOf](../api/user-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 获取组、 目录角色和管理用户属于其直接成员的 memberOf 导航属性中的单位。|
|[列表可传递 memberOf](../api/user-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 列出了组、 目录角色和管理单元的用户的成员。 此操作可传递，包括用户的嵌套的成员的组。 |
|[列出 joinedTeams](../api/user-list-joinedteams.md) |[groups](group.md)集合| 获取用户从 joinedTeams 导航属性直接成员的 Microsoft 团队。|
|[List ownedDevices](../api/user-list-owneddevices.md) |[directoryObject](directoryobject.md) collection| 从 ownedDevices 导航属性中获取此用户所拥有的设备。|
|[List ownedObjects](../api/user-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。|
|[List plannerTasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) collection| 获取 plannerTasks 分配给用户。|
|[List registeredDevices](../api/user-list-registereddevices.md) |[directoryObject](directoryobject.md) collection| 获取注册的设备的用户的 registeredDevices 导航属性。|
|[列表范围内的角色成员身份](../api/user-list-scopedrolememberof.md) |[scopedRoleMembership](scopedrolemembership.md)| Get 范围角色管理单位为此用户的成员身份。|
|[List createdObjects](../api/user-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| 从 createdObjects 导航属性中获取此用户创建的目录对象。|
|[列表 agreementAcceptances](../api/user-list-agreementacceptances.md) | [agreementAcceptance](agreementacceptance.md)集合 | 获取列表的使用条款接受状态的用户。|
|[assignLicense](../api/user-assignlicense.md)|[用户](user.md)|为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。|
|[List licenseDetails](../api/user-list-licensedetails.md) |[licenseDetails](licensedetails.md) 集合| 获取 licenseDetails 对象集合。|
|[checkMemberGroups](../api/user-checkmembergroups.md)|String collection|检查组列表中的成员身份。检查是可传递的。|
|[findmeetingtimes](../api/user-findmeetingtimes.md)|[meetingTimeCandidate](meetingtimecandidate.md)|查找时间和位置，以满足基于与会者可用性、 位置或时间限制。|
|[findRoomLists](../api/user-findroomlists.md)|[emailaddress.md](emailaddress.md)集合 | 获取在租户中定义的会议室列表。|
|[findRooms](../api/user-findrooms.md)|[emailaddress.md](emailaddress.md)集合 | 获取所有会议房间或特定的会议室列表中用户的租户。 |
|[getMailTips](../api/user-getmailtips.md)|[邮件提醒](mailtips.md)集合|返回向已登录用户提供的一个或多个收件人的邮件提醒。 |
|[getMemberGroups](../api/user-getmembergroups.md)|String collection|返回用户是其成员的所有组。检查是可传递的。|
|[getMemberObjects](../api/user-getmemberobjects.md)|String collection| 返回所有组、 目录角色和管理单元的用户的成员。 检查是传递的。 |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| 无 |使用户的所有刷新和会话令牌颁发给应用程序，通过为当前日期时间重置**refreshTokensValidFromDateTime**用户属性无效。 这样会强制用户再次登录到这些应用程序。|
|[reminderView](../api/user-reminderview.md)|[Reminder](reminder.md) collection|返回指定开始时间和结束时间范围内的日历提醒列表。|
|[delta](../api/user-delta.md)|用户集合| 获取用户的增量更改。 |
|[翻译 Outlook 标识符](../api/user-translateexchangeids.md) |[convertIdResult 资源类型](convertidresult.md)集合| 翻译格式之间的 Outlook 相关的资源的标识符。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性

| 属性       | 类型    | 说明 |
|:---------------|:--------|:------------|
|aboutMe|String|任意形式的文本输入字段，用于介绍用户自身。|
|accountEnabled|Boolean| 启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。    |
|ageGroup|字符串|设置用户的年龄组。 允许值： `null`， `minor`，`notAdult`和`adult`。 请参阅[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|分配给该用户的许可证。不可为 null。            |
|assignedPlans|[assignedPlan](assignedplan.md) 集合|分配给该用户的计划。只读。不可为 null。 |
|birthday|DateTimeOffset|用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|city|字符串|用户所在的城市。支持 $filter。|
|companyName| String | 与用户关联的公司名称。 只读。
|consentProvidedForMinor|字符串|设置是否已为未成年人获得许可。 允许值： `null`， `granted`，`denied`和`notRequired`。 请参阅[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。|
|country|字符串|在用户所处; 国家/地区例如，"美国"或"英国"。 支持 $filter。|
|deletedDateTime|DateTimeOffset| 日期和时间已删除用户。 |
|department|字符串|用户工作部门的名称。支持 $filter。|
|displayName|String|用户通讯簿中显示的名称。 通常，此值是名字的用户，中间的初始，和最后一个名称的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 $filter 和 $orderby。|
|雇员 id|字符串|分配给用户组织的员工标识符。 支持 $filter。|
|externalUserState|字符串|邀请到租户使用[API 邀请](../api/invitation-post.md)外部用户，此属性表示受邀的用户的邀请状态。 受邀用户的状态可以 PendingAcceptance 或接受或`null`为所有其他用户。 支持 $filter 的受支持的值。 例如：`$filter=externalUserState eq 'PendingAcceptance'`。|
|externalUserStateChangeDateTime|字符串|显示 externalUserState 属性的最新更改的时间戳。|
|传真号码|字符串|用户的传真号码。|
|givenName|字符串|用户的名。支持 $filter。|
|hireDate|DateTimeOffset|用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String|用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。|
|interests|String collection|用户介绍自身兴趣的列表。|
|jobTitle|字符串|用户的职务。支持 $filter。|
|legalAgeGroupClassification|字符串| 企业应用程序用于确定的用户的法律年龄组。 此属性是只读的计算基于`ageGroup`和`consentProvidedForMinor`属性。 允许值： `null`， `minorWithOutParentalConsent`， `minorWithParentalConsent`， `minorNoParentalConsentRequired`，`notAdult`和`adult`。 引用[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。）|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md)集合|为此用户的许可证分配状态。 只读。|
|mail|字符串|用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。只读。支持 $filter。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|已登录用户的主邮箱的设置。 您可以[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)设置发送自动答复传入邮件、 区域设置、 和时区。|
|mailNickname|字符串|用户的邮件别名。创建用户时必须指定此属性。支持 $filter。|
|mobilePhone|String|用户的主要移动电话号码。|
|mySite|String|用户个人网站的 URL。|
|officeLocation|String|用户公司地点的办公室位置。|
|onPremisesDistinguishedName|字符串| 包含在本地 Active Directory`distinguished name`或`DN`。 正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。 只读。 |
|onPremisesDomainName|字符串| 包含本地`domainFQDN`，也称为 dnsDomainName 从内部部署目录同步。 正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。 只读。 |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|包含用户的 extensionAttributes 1-15。 请注意，单个扩展属性既不可选，也不可筛选。 为`onPremisesSyncEnabled`用户，此组属性是主要的内部部署和是只读的。 仅限云用户 (其中`onPremisesSyncEnabled`为 false)，这些属性的创建过程中可以设置或更新。 |
|onPremisesImmutableId|字符串|此属性用于将内部部署 Active Directory 用户帐户对其 Azure AD 用户对象相关联。 必须指定此属性，当在图表中创建新的用户帐户，如果您将联盟的域用户的`userPrincipalName`(UPN) 属性。 **重要：****$** 和指定此属性时，不能使用 **_** 字符。 支持 $filter。 |
|onPremisesLastSyncDateTime|DateTimeOffset|表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)集合| 设置过程中使用 Microsoft 同步产品时错误。 |
|onPremisesSamAccountName|字符串| 包含本地`sAMAccountName`从内部部署目录同步。 正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。 只读。 |
|onPremisesSecurityIdentifier|字符串|包含从本地同步到云的用户的本地安全标识符 (SID)。只读。|
|onPremisesSyncEnabled|Boolean| 如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。只读 |
|onPremisesUserPrincipalName|字符串| 包含本地`userPrincipalName`从内部部署目录同步。 正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。 只读。 |
|otherMails|字符串| 用户; 其他电子邮件地址列表例如： `["bob@contoso.com", "Robert@fabrikam.com"]`。 支持 $filter。|
|passwordPolicies|字符串|指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。|
|passwordProfile|[PasswordProfile](passwordprofile.md)|指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|
|pastProjects|String collection|供用户枚举其过去项目的列表。|
|postalCode|字符串|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。|
|preferredDataLocation|字符串|用户首选的数据位置。 有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。|
|preferredLanguage|字符串|用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。|
|preferredName|String|用户的首选名称。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) 集合|为用户设置的计划。只读。不可为 null。 |
|proxyAddresses|String collection|例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 需要多值属性筛选器表达式的 **any** 运算符。只读，不可为 Null。支持 $filter。          |
|refreshTokensValidFromDateTime|DateTimeOffset| 这次均无效，和应用程序会发生错误时使用无效刷新或会话令牌获取委派的访问令牌 （用于访问 Microsoft Graph 如 Api） 之前，发出任何刷新令牌或会话令牌 (会话 cookie)。  如果发生这种情况，应用程序需要获取新刷新令牌的授权终结点向发出请求。 只读。 使用[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)重置。|
|responsibilities|String collection|供用户枚举其职责的列表。|
|schools|String collection|供用户枚举其学习过的学校列表。|
|showInAddressList|Boolean|**true**如果 Outlook 全局地址列表应包含此用户，否则为**false**。 如果未设置，这将被视为**true**。 对于用户通过邀请管理器邀请，此属性将设置为**false**。|
|skills|String collection|供用户枚举其技能的列表。|
|state|字符串|用户地址中的省/市/自治区或省。支持 $filter。|
|streetAddress|String|用户公司地点的街道地址。|
|surname|字符串|用户的姓氏。支持 $filter。|
|usageLocation|字符串|两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。
|userType|字符串|用于分类用户在您的目录，如"成员"和"来宾"中键入一个字符串值。 支持 $filter。          |

### <a name="legal-age-group-property-definitions"></a>法律期限组属性定义

本节介绍如何三个 age 组属性 (`legalAgeGroupClassification`，`ageGroup`和`consentProvidedForMinor`) 的 Azure AD 管理员和企业应用程序开发人员用于满足期限相关法规。

例如： Cameron 是管理员在英国 Holyport 小学的目录。 学校本年度开头他使用许可书面工作征得次要的父级基于 United Kingdom 的年龄相关法规。 从父获得许可允许 Holyport 学校和 Microsoft 应用程序使用次要的帐户。 Cameron 然后创建所有帐户，并设置为"次要"ageGroup 和 consentProvidedForMinor 到"授予"。 使用学生的应用程序就可以禁止不合适进行评级的功能。

#### <a name="legal-age-group-classification"></a>法律期限组分类

企业应用程序开发人员使用此只读属性以确保正确处理根据其法律年龄组的用户。 计算基于用户的`ageGroup`和`consentProvidedForMinor`属性。

| 值   | # |说明|
|:---------------|:--------|:----------|
|null|0|默认值，不`ageGroup`已经为用户设置。|
|minorWithoutParentalConsent |1|（留作将来使用）|
|minorWithParentalConsent|2| 用户被视为基于其所在国家/地区的年龄相关规章次要或区域和管理员的帐户已从父或监护人获取适当许可。|
|成人|3|用户视为成人基于其国家或地区的年龄相关法规。|
|notAdult|4|是用户距离的国家或地区具有其他期限相关法规 （如美国、 英国、 欧盟或韩国），并且用户的年龄之间次要和成人期限 （作为规定根据的国家或地区）。 通常，这意味着青少年都会被视为`notAdult`监管国家/地区。|
|minorNoParentalConsentRequired|5|用户是次要，但从的国家或地区已没有与时间有关的法规。|

#### <a name="age-group-and-minor-consent"></a>年龄组和次要同意

年龄组和次要同意属性是 Azure AD 管理员用来帮助确保正确基于调控用户的国家或地区的年龄相关的管理法规规则处理帐户使用的可选属性。

#### <a name="agegroup-property"></a>ageGroup 属性

| 值    | # |说明|
|:---------------|:--------|:----------|
|null|0|默认值，不`ageGroup`已经为用户设置。|
|次要|1|用户是考虑次要。|
|notAdult|2|用户是从具有法定法规美国、 英国、 欧盟或韩国的国家/地区） 并且用户的年龄孩子期限 （根据国家/地区） 的上限超过和成人年龄小于下限 （作为规定根据的国家或地区）. 基本上，因此视为青少年`notAdult`监管国家/地区。|
|成人|3|用户应该为成人内容处理。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor 属性

| 值    | # |说明|
|:---------------|:--------|:----------|
|null|0|默认值，不`consentProvidedForMinor`已经为用户设置。|
|授予|1|已为用户都具有帐户获得许可。|
|denied|2|用户具有帐户未获得许可。|
|notRequired|3|用户从不需要同意位置。|

## <a name="relationships"></a>Relationships

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md)集合| 使用验收状态的用户的词。 只读。 可为 Null。|
|日历|[日历](calendar.md)|用户的主日历。只读。|
|calendarGroups|[calendarGroup](calendargroup.md)集合|用户的日历组。只读。可为 Null。|
|calendarView|[事件](event.md) 集合|日历的日历视图。只读。可为 Null。|
|calendars|[日历](calendar.md) 集合|用户的日历。只读。可为 Null。|
|contactFolders|[contactFolder](contactfolder.md)集合|用户的联系人文件夹。只读。可为 Null。|
|contacts|[联系人](contact.md)集合|用户的联系人。只读。可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) 集合|由用户创建的 directory 对象。只读。可为 Null。|
|directReports|[directoryObject](directoryobject.md) collection|向此用户报告的用户和联系人。（其 manager 属性已设置为此用户的用户和联系人。）只读。可为 Null。 |
|drive|[驱动器](drive.md)|用户的 OneDrive。只读。|
|events|[事件](event.md) 集合|用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。|
|extensions|[扩展](extension.md)集合|打开扩展名为用户定义的集合。 可为 Null。|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|见解|[见解](insights.md)集合| 只读。可为 NULL。|
|joinedGroups|[组](group.md) 集合| 只读。可为 Null。|
|mailFolders|[mailFolder](mailfolder.md) 集合| 用户的邮件文件夹。只读。可为 Null。|
|manager|[directoryObject](directoryobject.md)|是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）|
|memberOf|[directoryObject](directoryobject.md) 集合|用户所属的所有组、目录角色和管理单元。只读。可为 Null。|
|joinedTeams|[组](group.md) 集合|Microsoft 小组成员的用户。 只读。 可为 Null。|
|messages|[邮件](message.md)集合|邮箱或文件夹中的邮件。只读。可为 Null。|
|onenote|[OneNote](onenote.md)| 只读。|
|outlook|[outlookUser](outlookuser.md)| 选择性 Outlook 服务对用户可用。 只读。 可为 Null。|
|ownedDevices|[directoryObject](directoryobject.md) 集合|用户拥有的设备。只读。可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|用户拥有的 directory 对象。只读。可为 Null。|
|人脉|[人员](person.md)集合| 只读。与用户最相关的人员。该集合按其与用户的相关性排序，相关性由用户的通信、协作和业务关系决定。人脉是邮件、联系人和社交网络中的信息聚合。|
|照片|[profilePhoto](profilephoto.md)| 用户的个人资料照片。只读。|
|照片|[照片](photo.md)集合| 只读。可为 NULL。|
|planner|[plannerUser](planneruser.md)| 选择性计划程序服务对用户可用。 只读。 可为 Null。 |
|SharePoint|[sharepoint](sharepoint.md)| 访问用户的 SharePoint 站点。只读。 |
|scopedRoleMemberOf|[scopedRoleMembership](scopedrolemembership.md)| 此用户的范围内的角色管理单元成员身份。 只读。 可为 Null。|
|settings|[设置](user-settings.md)集合| 只读。可为 Null。|
|registeredDevices|[directoryObject](directoryobject.md) 集合|已注册的用户的设备。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "insights": { "@odata.type": "microsoft.graph.officeGraphInsights" },
  "settings": { "@odata.type": "microsoft.graph.userSettings" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "joinedTeams": [ { "@odata.type": "microsoft.graph.group" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
