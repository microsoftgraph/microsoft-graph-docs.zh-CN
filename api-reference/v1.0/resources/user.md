# <a name="user-resource-type"></a>用户资源类型

表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。
- 通过提供 [delta](../api/user_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[List users](../api/user_list.md) |[user](user.md) 集合| 获取用户对象列表。|
|[Create user](../api/user_post_users.md) |[user](user.md)| 新建用户对象。|
|[Get user](../api/user_get.md) | [user](user.md) |读取 user 对象的属性和关系。|
|[Update user](../api/user_update.md) | [user](user.md) |更新 user 对象。 |
|[Delete user](../api/user_delete.md) | None |删除 user 对象。 |
|[List messages](../api/user_list_messages.md) |[Message](message.md) collection| 获取已登录用户的邮箱中的所有邮件。|
|[Create Message](../api/user_post_messages.md) |[Message](message.md)| 通过发布到邮件集合新建邮件。|
|[List mailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) collection| 在已登录用户的根文件夹下获取邮件文件夹集合。 |
|[Create mailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 mailFolders 集合创建新 MailFolder。|
|[sendMail](../api/user_sendmail.md)|None|发送请求正文中指定的邮件。|
|[List events](../api/user_list_events.md) |[Event](event.md) collection| 获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。|
|[Create event](../api/user_post_events.md) |[Event](event.md)| 通过发布到事件集合创建新事件。|
|[List calendars](../api/user_list_calendars.md) |[Calendar](calendar.md) collection| 获取 Calendar 对象集合。|
|[Create calendar](../api/user_post_calendars.md) |[Calendar](calendar.md)| 通过发布到日历集合创建新日历。|
|[List calendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) collection| 获取 CalendarGroup 对象集合。|
|[Create calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| 通过发布到 calendarGroups 集合新建 CalendarGroup。|
|[List calendarView](../api/user_list_calendarview.md) |[Event](event.md) collection| 获取 Event 对象集合。|
|[List contacts](../api/user_list_contacts.md) |[Contact](contact.md) collection| 从已登录用户的默认联系人文件夹中获取联系人集合。|
|[Create Contact](../api/user_post_contacts.md) |[Contact](contact.md)| 通过发布到联系人集合新建联系人。|
|[List contactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) collection| 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。|
|[Create ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| 通过发布到 contactFolders 集合创建新 ContactFolder。|
|[List directReports](../api/user_list_directreports.md) |[directoryObject](directoryobject.md) collection| 从 directReports 导航属性中获取向此用户报告的用户和联系人。|
|[List manager](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | 从 manager 导航属性中获取是此用户的经理的用户或联系人。|
|[List memberOf](../api/user_list_memberof.md) |[directoryObject](directoryobject.md) collection| 从 memberOf 导航属性中获取此用户是其直接成员的组和目录角色。|
|[List ownedDevices](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md) collection| 从 ownedDevices 导航属性中获取此用户所拥有的设备。|
|[List ownedObjects](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md) collection| 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。|
|[List registeredDevices](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md) collection| 从 registeredDevices 导航属性中获取为此用户注册的设备。|
|[List createdObjects](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md) collection| 从 createdObjects 导航属性中获取此用户创建的目录对象。|
|[assignLicense](../api/user_assignlicense.md)|[user](user.md)|为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。|
|[List licenseDetails](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md) 集合| 获取 licenseDetails 对象集合。| 
|[checkMemberGroups](../api/user_checkmembergroups.md)|String collection|检查组列表中的成员身份。检查是可传递的。|
|[getMemberGroups](../api/user_getmembergroups.md)|String collection|返回用户是其成员的所有组。检查是可传递的。|
|[getMemberObjects](../api/user_getmemberobjects.md)|String collection| 返回用户所属的所有组和目录角色。检查是可传递的。 |
|[reminderView](../api/user_reminderview.md)|[Reminder](reminder.md) collection|返回指定开始时间和结束时间范围内的日历提醒列表。|
|[delta](../api/user_delta.md)|用户集合| 获取用户的增量更改。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|



## <a name="properties"></a>属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|aboutMe|String|任意形式的文本输入字段，用于介绍用户自身。|
|accountEnabled|Boolean| 启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|分配给该用户的许可证。不可为 null。            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|分配给该用户的计划。只读。不可为 null。 |
|birthday|DateTimeOffset|用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|businessPhones|String collection|用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。|
|城市|String|用户所在的城市。支持 $filter。|
|companyName|String|与用户关联的公司名称。|
|country|String|用户所在的国家/地区；例如，“美国”或“英国”。支持 $filter。|
|department|String|用户工作部门的名称。支持 $filter。|
|displayName|String|用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|givenName|String|用户的名。支持 $filter。|
|hireDate|DateTimeOffset|用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String|用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。|
|imAddresses|String collection|用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。|
|interests|String collection|用户介绍自身兴趣的列表。|
|jobTitle|String|用户的职务。支持 $filter。|
|邮件|String|用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。只读。支持 $filter。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|已登录用户的主邮箱的设置。可以[获取](../api/user_get_mailboxsettings.md)或[更新](../api/user_update_mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。|
|mailNickname|String|用户的邮件别名。创建用户时必须指定此属性。支持 $filter。|
|mobilePhone|String|用户的主要移动电话号码。|
|mySite|String|用户个人网站的 URL。|
|officeLocation|String|用户公司地点的办公室位置。|
|onPremisesImmutableId|String|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。**重要说明：**指定该属性时不能使用 **$** 和 **_** 字符。支持 $filter。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|onPremisesSecurityIdentifier|String|包含从本地同步到云的用户的本地安全标识符 (SID)。只读。|
|onPremisesSyncEnabled|Boolean| 如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。只读 |
|passwordPolicies|String|指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。|
|passwordProfile|[PasswordProfile](passwordprofile.md)|指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|
|pastProjects|String collection|供用户枚举其过去项目的列表。|
|postalCode|String|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。|
|preferredLanguage|String|用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。|
|preferredName|String|用户的首选名称。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|为用户设置的计划。只读。不可为 null。 |
|proxyAddresses|String collection|例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 需要多值属性筛选器表达式的 **any** 运算符。只读，不可为 Null。支持 $filter。          |
|responsibilities|String collection|供用户枚举其职责的列表。|
|schools|String collection|供用户枚举其学习过的学校列表。|
|skills|String collection|供用户枚举其技能的列表。|
|state|String|用户地址中的省/市/自治区或省。支持 $filter。|
|streetAddress|String|用户公司地点的街道地址。|
|surname|String|用户的姓氏。支持 $filter。|
|usageLocation|String|两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。
|userType|String|可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。          |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|calendar|[Calendar](calendar.md)|用户的主日历。只读。|
|calendarGroups|[CalendarGroup](calendargroup.md) collection|用户的日历组。只读。可为 Null。|
|calendarView|[Event](event.md) collection|日历的日历视图。只读。可为 Null。|
|calendars|[Calendar](calendar.md) collection|用户的日历。只读。可为 Null。|
|contactFolders|[ContactFolder](contactfolder.md) collection|用户的联系人文件夹。只读。可为 Null。|
|contacts|[Contact](contact.md) collection|用户的联系人。只读。可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) collection|由用户创建的 directory 对象。只读。可为 Null。|
|directReports|[directoryObject](directoryobject.md) collection|向此用户报告的用户和联系人。（其 manager 属性已设置为此用户的用户和联系人。）只读。可为 Null。 |
|drive|[drive](drive.md)|用户的 OneDrive。只读。|
|驱动器|[驱动器](drive.md)集合 | 该用户的可用驱动器集合。只读。 |
|events|[Event](event.md) collection|用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。|
|extensions|[扩展](extension.md)集合|为用户定义的开放扩展集合。只读。可为 Null。|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|mailFolders|[MailFolder](mailfolder.md) collection| 用户的邮件文件夹。只读。可为 Null。|
|manager|[directoryObject](directoryobject.md)|是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）|
|memberOf|[directoryObject](directoryobject.md) collection|用户所属的组和目录角色。只读。可为 Null。|
|messages|[Message](message.md) collection|邮箱或文件夹中的邮件。只读。可为 Null。|
|onenote|[OneNote](onenote.md)| 只读。|
|ownedDevices|[directoryObject](directoryobject.md) collection|用户拥有的设备。只读。可为 Null。|
|ownedObjects|[directoryObject](directoryobject.md) collection|用户拥有的 directory 对象。只读。可为 Null。|
|photo|[profilePhoto](profilephoto.md)| 用户的个人资料照片。只读。|
|registeredDevices|[directoryObject](directoryobject.md) collection|已注册的用户的设备。只读。可为 Null。|

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
    "messages",
    "oauth2PermissionGrants",
    "onenote",
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
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
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
