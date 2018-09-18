# <a name="user-resource-type"></a>用户资源类型

表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 将自己的数据作为[扩展](../../../concepts/extensibility_overview.md)添加到自定义属性。
- 订阅[更改通知](../../../concepts/webhooks.md)。
- 通过提供 [delta](../api/user_delta.md) 函数使用 [delta 查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列举用户](../api/user_list.md) |[user](user.md) 集合| 获取用户对象列表。|
|[创建用户](../api/user_post_users.md) |[用户](user.md)| 新建用户对象。|
|[获取用户](../api/user_get.md) | [用户](user.md) |读取 user 对象的属性和关系。|
|[更新用户](../api/user_update.md) | [用户](user.md) |更新 user 对象。 |
|[删除用户](../api/user_delete.md) | 无 |删除 user 对象。 |
|[列举消息](../api/user_list_messages.md) |[消息](message.md) 集合| 获取已登录用户的邮箱中的所有邮件。|
|[创建消息](../api/user_post_messages.md) |[消息](message.md)| 通过发布到邮件集合新建邮件。|
|[列举 mailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) 集合| 在已登录用户的根文件夹下获取邮件文件夹集合。 |
|[创建 mailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 mailFolders 集合创建新 MailFolder。|
|[sendMail](../api/user_sendmail.md)|无|发送请求正文中指定的邮件。|
|[列举事件](../api/user_list_events.md) |[事件](event.md) 集合| 获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/user_post_events.md) |[事件](event.md)| 通过发布到事件集合创建新事件。|
|[列举日历](../api/user_list_calendars.md) |[日历](calendar.md) 集合| 获取 Calendar 对象集合。|
|[创建日历](../api/user_post_calendars.md) |[日历](calendar.md)| 通过发布到日历集合创建新日历。|
|[列举 calendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) 集合| 获取 CalendarGroup 对象集合。|
|[创建 calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| 通过发布到 calendarGroups 集合新建 CalendarGroup。|
|[列举 calendarView](../api/user_list_calendarview.md) |[事件](event.md) 集合| 获取 Event 对象集合。|
|[列举联系人](../api/user_list_contacts.md) |[联系人](contact.md) 集合| 从已登录用户的默认联系人文件夹中获取联系人集合。|
|[创建联系人](../api/user_post_contacts.md) |[联系人](contact.md)| 通过发布到联系人集合新建联系人。|
|[列举 contactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) 集合| 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。|
|[创建 ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| 通过发布到 contactFolders 集合创建新 ContactFolder。|
|[列举 directReports](../api/user_list_directreports.md) |[directoryObject](directoryobject.md) 集合| 从 directReports 导航属性中获取向此用户报告的用户和联系人。|
|[列举管理员](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | 从 manager 导航属性中获取是此用户的经理的用户或联系人。|
|[列举 memberOf](../api/user_list_memberof.md) |[directoryObject](directoryobject.md) 集合| 从 memberOf 导航属性中获取此用户是其直接成员的组和目录角色。|
|[列举 ownedDevices](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md) 集合| 从 ownedDevices 导航属性中获取此用户所拥有的设备。|
|[列举 ownedObjects](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md) 集合| 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。|
|[列举 registeredDevices](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md) 集合| 从 registeredDevices 导航属性中获取为此用户注册的设备。|
|[列举 createdObjects](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md) 集合| 从 createdObjects 导航属性中获取此用户创建的目录对象。|
|[assignLicense](../api/user_assignlicense.md)|[用户](user.md)|为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。|
|[列举 licenseDetails](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md) 集合| 获取 licenseDetails 对象集合。|
|[checkMemberGroups](../api/user_checkmembergroups.md)|字符串集合|检查组列表中的成员身份。检查是可传递的。|
|[getMemberGroups](../api/user_getmembergroups.md)|字符串集合|返回用户是其成员的所有组。检查是可传递的。|
|[getMemberObjects](../api/user_getmemberobjects.md)|字符串集合| 返回用户所属的所有组和目录角色。检查是可传递的。 |
|[reminderView](../api/user_reminderview.md)|[提醒](reminder.md) 集合|返回指定开始时间和结束时间范围内的日历提醒列表。|
|[增量](../api/user_delta.md)|用户集合| 获取用户的增量更改。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|aboutMe|字符串|任意形式的文本输入字段，用于介绍用户自身。|
|accountEnabled|布尔| 启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。    |
|ageGroup|String|设置用户的年龄组。 允许值： `null`， `minor`， `notAdult` 和 `adult`。 请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) 以获取详细信息。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) 集合|分配给该用户的许可证。不可为 null。            |
|assignedPlans|[assignedPlan](assignedplan.md) 集合|分配给该用户的计划。只读。不可为 null。 |
|生日|DateTimeOffset|用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`|
|businessPhones|字符串集合|用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。|
|城市|字符串|用户所在的城市。支持 $filter。|
|companyName| 字符串 | 与用户关联的公司名称。 只读。
|consentProvidedForMinor|String|设置是否已为未成年人获得许可。 允许值： `null`， `granted`， `denied` 和 `notRequired`。 请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) 以获取详细信息。|
|country|字符串|用户所在的国家/地区；例如，“美国”或“英国”。支持 $filter。|
|部门|字符串|用户工作部门的名称。支持 $filter。|
|displayName|字符串|用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|givenName|字符串|用户的名。支持 $filter。|
|hireDate|DateTimeOffset|用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`|
|id|字符串|用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。|
|imAddresses|字符串集合|用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。|
|兴趣|字符串集合|用户介绍自身兴趣的列表。|
|jobTitle|字符串|用户的职务。支持 $filter。|
|legalAgeGroupClassification|String| 企业应用程序用于确定用户的法律年龄组。 此属性为只读，基于 `ageGroup` 和 `consentProvidedForMinor` 属性计算。 允许值： `null`， `minorWithOutParentalConsent`， `minorWithParentalConsent` 和 `minorNoParentalConsentRequired`。`notAdult``adult` 请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) i获取详细信息。|
|mail|字符串|用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。只读。支持 $filter。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|已登录用户的主邮箱的设置。可以[获取](../api/user_get_mailboxsettings.md)或[更新](../api/user_update_mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。|
|mailNickname|字符串|用户的邮件别名。创建用户时必须指定此属性。支持 $filter。|
|mobilePhone|字符串|用户的主要移动电话号码。|
|mySite|字符串|用户个人网站的 URL。|
|officeLocation|字符串|用户公司地点的办公室位置。|
|onPremisesDomainName|字符串| 包含本地 `domainFQDN`，也称为从本地目录同步的 dnsDomainName。 此属性仅针对正在通过 Azure AD Connect 同步本地目录到 Azure Active Directory 的客户填充。 只读。 |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|包含用户的 extensionAttributes 1-15。 请注意，单个扩展属性既不可选，也不可筛选。 对于 `onPremisesSyncEnabled` 用户，此组属性是在本地主控并且只读。 对于仅限云的用户（其 `onPremisesSyncEnabled`  为 false），这些属性可以在创建或更新过程中设置。 |
|onPremisesImmutableId|字符串|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。**重要说明：** 指定该属性时不能使用 **$** 和 **_** 字符。支持 $filter。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合| 设置过程中使用 Microsoft 同步产品时出错。 |
|onPremisesSamAccountName|String| 包含从本地目录同步的本地 `samAccountName`。 此属性仅针对正在通过 Azure AD Connect 同步本地目录到 Azure Active Directory 的客户填充。 只读。 |
|onPremisesSecurityIdentifier|字符串|包含从本地同步到云的用户的本地安全标识符 (SID)。只读。|
|onPremisesSyncEnabled|布尔值| 如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。只读 |
|onPremisesUserPrincipalName|String| 包含从本地目录同步的本地 `userPrincipalName`。 此属性仅针对正在通过 Azure AD Connect 同步本地目录到 Azure Active Directory 的客户填充。 只读。 |
|passwordPolicies|字符串|指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。|
|passwordProfile|[PasswordProfile](passwordprofile.md)|指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|
|pastProjects|字符串集合|供用户枚举其过去项目的列表。|
|postalCode|字符串|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。|
|preferredLanguage|字符串|用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。|
|preferredName|字符串|用户的首选名称。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) 集合|为用户设置的计划。只读。不可为 null。 |
|proxyAddresses|字符串集合|例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 需要多值属性筛选器表达式的 **any** 运算符。只读，不可为 Null。支持 $filter。          |
|责任|字符串集合|供用户枚举其职责的列表。|
|schools|字符串集合|供用户枚举其学习过的学校列表。|
|skills|字符串集合|供用户枚举其技能的列表。|
|state|字符串|用户地址中的省/市/自治区或省。支持 $filter。|
|streetAddress|字符串|用户公司地点的街道地址。|
|surname|字符串|用户的姓氏。支持 $filter。|
|usageLocation|字符串|两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。|
|userPrincipalName|字符串|用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。
|userType|字符串|可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。          |

### <a name="legal-age-group-property-definitions"></a>法律年龄分组属性定义

本节介绍如何三个由 Azure AD 管理员和企业应用程序开发人员使用以满足期限相关法规的年龄分组属性 (`legalAgeGroupClassification`, `ageGroup` 和 `consentProvidedForMinor`) 。

例如： Cameron 是英国 Holyport 小学目录的管理员。 本学年开始，据英国与年龄相关的法规要求，他使用入学通知书获得未成年人父母的许可。 获得父母许可以允许 Holyport 学校和 Microsoft 应用程序使用未成年人的帐户。 随后，Cameron创建所有帐户，并设置为"未成年人"ageGroup 和 consentProvidedForMinor 为"已获授权"。 学生使用的应用程序可以禁用部分不未成年人的功能。

#### <a name="legal-age-group-classification"></a>法律年龄分组分类

企业应用程序开发人员使用只读属性以确保基于所属法律年龄分组用户的正确处理。 计算基于用户的 `ageGroup` 和 `consentProvidedForMinor` 属性。

| 值    | #  |说明|
|:---------------|:--------|:----------|
|null|0|默认值，无 `ageGroup` 已经作为用户设置。|
|minorWithoutParentalConsent |1|（保留供将来使用）|
|minorWithParentalConsent|2| 基于其所在国家/地区的年龄相关规定，用户被视为未成年人，同时帐户管理员已从f父母之一或监护人获取适当许可。|
|adult|3|基于所在国家或地区的年龄相关法规，用户被视为成人。|
|notAdult|4|用户所在家或地区实施有其他年龄相关法规 （如美国、英国、欧盟或韩国），并且用户年龄处于未成年人和成人年龄之间 （根据所在国家或地区规定）。 一般来说，这意味着青少年都会被视为处于 `notAdult` 监管国家。|
|minorNoParentalConsentRequired|5|用户为未成年人，但所在国家或地区不存在与年龄相关的法规。|

#### <a name="age-group-and-minor-consent"></a>年龄分组和未成年人同意

年龄分组和未成年人同意属性是 Azure AD 管理员可选属性，在根据用户所在国家或地区与年龄相关的管理法规，用于帮助确保正确处理帐户的使用。

#### <a name="agegroup-property"></a>ageGroup 属性

| 值    | #  |说明|
|:---------------|:--------|:----------|
|null|0|默认值，无 `ageGroup` 已经作为用户设置。|
|minor|1|用户视为未成年人。|
|notAdult|2|用户来自有法定法规的国家（美国、英国、欧盟或韩国），并且用户年龄高于儿童年龄（根据国家/地区规定）的上限，并低于成人年龄的下限 （根据国家/地区规定）。 基本上，青少年视为在 `notAdult` 监管国家。|
|adult|3|用户应作为成人处理。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor 属性

| 值    | #  |说明|
|:---------------|:--------|:----------|
|null|0|默认值，无 `consentProvidedForMinor` 已经作为用户设置。|
|granted|1|用户已经获得配置账户许可。|
|denied|2|用户未获得许可配置账户。|
|notRequired|3|用户所在地不要求获得同意。|
 
## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|activities|[userActivity](projectrome_activity.md) 集合|跨设备的用户的活动。 只读。 可为 Null。|
|calendar|[日历](calendar.md)|用户的主日历。只读。|
|calendarGroups|[CalendarGroup](calendargroup.md) 集合|用户的日历组。只读。可为 Null。|
|calendarView|[事件](event.md) 集合|日历的日历视图。只读。可为 Null。|
|日历|[日历](calendar.md) 集合|用户的日历。只读。可为 Null。|
|contactFolders|[ContactFolder](contactfolder.md) 集合|用户的联系人文件夹。只读。可为 Null。|
|联系人|[联系人](contact.md) 集合|用户的联系人。只读。可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) 集合|由用户创建的 directory 对象。只读。可为 Null。|
|directReports|[directoryObject](directoryobject.md) 集合|向此用户报告的用户和联系人。（其 manager 属性已设置为此用户的用户和联系人。）只读。可为 Null。 |
|驱动器|[驱动器](drive.md)|用户的 OneDrive。只读。|
|drives|[drive](drive.md) 集合| 该用户的可用驱动器集合。只读。 |
|事件|[事件](event.md) 集合|用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。|
|扩展|[扩展](extension.md)集合|为用户定义的开放扩展集合。只读。可为 Null。|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|licenseDetails|[LicenseDetails](licensedetails.md) 集合|此用户的许可证详细信息集合。 可为 Null。|
|mailFolders|[MailFolder](mailfolder.md) 集合| 用户的邮件文件夹。只读。可为 Null。|
|管理员|[directoryObject](directoryobject.md)|是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）|
|memberOf|[directoryObject](directoryobject.md) 集合|用户所属的组和目录角色。只读。可为 Null。|
|消息|[邮件](message.md) 集合|邮箱或文件夹中的邮件。只读。可为 Null。|
|onenote|[Onenote](onenote.md)| 只读。|
|outlook|[OutlookUser](outlookuser.md)| 只读。|
|ownedDevices|[directoryObject](directoryobject.md) 集合|用户拥有的设备。只读。可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|用户拥有的 directory 对象。只读。可为 Null。|
|people|[person](person.md) 集合| 与用户相关的人员。 只读。 可为 Null。
|photo|[profilePhoto](profilephoto.md)| 用户的个人资料照片。只读。|
|planner|[plannerUser](planneruser.md)| Planner 资源可能存在的用户的入口点。 只读。|
|registeredDevices|[directoryObject](directoryobject.md) 集合|已注册的用户的设备。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
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
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
