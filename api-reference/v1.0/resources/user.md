---
title: 用户资源类型
description: Represents an Azure AD user account. Inherits from directoryObject.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f18cc3f56a39f072a6501c94e7f4179746d893f4
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845315"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法                                                                                     | 返回类型                                                                      | 说明                                                                                                                                                                                                                         |
|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [List users](../api/user-list.md)                                                          | [user](user.md) 集合                                                       | 获取用户对象列表。                                                                                                                                                                                                         |
| [Create user](../api/user-post-users.md)                                                   | [user](user.md)                                                                  | 新建用户对象。                                                                                                                                                                                                           |
| [Get user](../api/user-get.md)                                                             | [user](user.md)                                                                  | 读取 user 对象的属性和关系。                                                                                                                                                                                   |
| [Update user](../api/user-update.md)                                                       | [user](user.md)                                                                  | 更新 user 对象。                                                                                                                                                                                                                 |
| [Delete user](../api/user-delete.md)                                                       | None                                                                             | 删除 user 对象。                                                                                                                                                                                                                 |
| [获取增量](../api/user-delta.md)                                                          | [user](user.md) 集合                                                       | 获取用户的增量更改。                                                                                                                                                                                                  |
| **应用程序角色分配**                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [列出 appRoleAssignments](../api/user-list-approleassignments.md)                          | [appRoleAssignment](approleassignment.md) 集合                             | 获取已分配此用户的应用和应用角色。                                                                                                                                                                       |
| [添加 appRoleAssignment](../api/user-post-approleassignments.md)                            | [appRoleAssignment](approleassignment.md)                                        | 向此用户分配应用程序角色。                                                                                                                                                                                                    |
| [删除 appRoleAssignment](../api/user-delete-approleassignments.md)                       | 无                                                                             | 从此用户中删除应用程序角色分配。                                                                                                                                                                                       |
| **Calendar**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Create calendar](../api/user-post-calendars.md)                                           | [Calendar](calendar.md)                                                          | 通过发布到日历集合创建新日历。                                                                                                                                                                       |
| [Create calendarGroup](../api/user-post-calendargroups.md)                                 | [CalendarGroup](calendargroup.md)                                                | 通过发布到 calendarGroups 集合新建 CalendarGroup。                                                                                                                                                             |
| [Create event](../api/user-post-events.md)                                                 | [event](event.md)                                                                | 通过发布到事件集合新建事件。                                                                                                                                                                             |
| [findMeetingTimes](../api/user-findmeetingtimes.md)                                        | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)                  | 基于与会者忙闲状态、位置或时间限制查找会议时间和位置。                                                                                                                                      |
| [getSchedule](../api/calendar-getschedule.md)                                              | [scheduleInformation](scheduleinformation.md)                                    | 获取用户、通讯组列表或资源（会议室或设备）在指定时间段内的忙/闲状态信息。                                                                           |
| [List calendars](../api/user-list-calendars.md)                                            | [calendar](calendar.md) 集合                                               | 获取 Calendar 对象集合。                                                                                                                                                                                                   |
| [List calendarGroups](../api/user-list-calendargroups.md)                                  | [calendarGroup](calendargroup.md) 集合                                     | 获取 CalendarGroup 对象集合。                                                                                                                                                                                              |
| [List calendarView](../api/user-list-calendarview.md)                                      | [event](event.md) 集合                                                     | 获取 Event 对象集合。                                                                                                                                                                                                      |
| [List events](../api/user-list-events.md)                                                  | [事件](event.md) 集合                                                     | Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.                                                                                                                   |
| [reminderView](../api/user-reminderview.md)                                                | [Reminder](reminder.md) collection                                               | 返回指定开始时间和结束时间范围内的日历提醒列表。                                                                                                                                                       |
| **联系人**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [创建联系人](../api/user-post-contacts.md)                                             | [联系人](contact.md)                                                            | 通过发布到联系人集合新建联系人。                                                                                                                                                                         |
| [创建 contactFolder](../api/user-post-contactfolders.md)                                 | [contactFolder](contactfolder.md)                                                | 通过发布到 contactFolders 集合创建新 ContactFolder。                                                                                                                                                             |
| [List contacts](../api/user-list-contacts.md)                                              | [联系人](contact.md)集合                                                 | 从已登录用户的默认联系人文件夹中获取联系人集合。                                                                                                                                                    |
| [List contactFolders](../api/user-list-contactfolders.md)                                  | [ContactFolder](contactfolder.md) 集合                                     | 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。                                                                                                                                             |
| **目录对象**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [assignLicense](../api/user-assignlicense.md)                                              | [用户](user.md)                                                                  | Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.                                                                                                            |
| [checkMemberGroups](../api/user-checkmembergroups.md)                                      | String collection                                                                | Check for membership in a list of groups. The check is transitive.                                                                                                                                                                  |
| [checkMemberObjects](../api/user-checkmemberobjects.md)                                    | String 集合                                                                | 检查组、目录角色或管理单元对象列表中的成员身份。 此函数可传递。                                                                                                                |
| [exportPersonalData](../api/user-exportpersonaldata.md)                                    | 无                                                                             | 提交公司管理员发出的数据策略操作请求，以导出组织用户的数据。                                                                                                                   |
| [getByIds](../api/directoryobject-getbyids.md)                                             | String collection                                                                | 返回 ID 列表中指定的目录对象。                                                                                                                                                                           |
| [getMemberGroups](../api/user-getmembergroups.md)                                          | String collection                                                                | Return all the groups that the user is a member of. The check is transitive.                                                                                                                                                        |
| [getMemberObjects](../api/user-getmemberobjects.md)                                        | String 集合                                                                | Return all of the groups and directory roles that the user is a member of. The check is transitive.                                                                                                                                 |
| [List createdObjects](../api/user-list-createdobjects.md)                                  | [directoryObject](directoryobject.md) collection                                 | 从 createdObjects 导航属性中获取此用户创建的目录对象。                                                                                                                                          |
| [List licenseDetails](../api/user-list-licensedetails.md)                                  | [licenseDetails](licensedetails.md) 集合                                   | 获取 licenseDetails 对象集合。                                                                                                                                                                                             |
| [List ownedDevices](../api/user-list-owneddevices.md)                                      | [directoryObject](directoryobject.md) 集合                                 | 从 ownedDevices 导航属性中获取此用户所拥有的设备。                                                                                                                                               |
| [List ownedObjects](../api/user-list-ownedobjects.md)                                      | [directoryObject](directoryobject.md) 集合                                 | 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。                                                                                                                                     |
| [List registeredDevices](../api/user-list-registereddevices.md)                            | [directoryObject](directoryobject.md) 集合                                 | 从 registeredDevices 导航属性中获取为此用户注册的设备。                                                                                                                                    |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md)                              | [user](user.md)                                                                  | 重新处理用户的订阅分配。                                                                                                                                                                                    |
| [revokeSignInSessions](../api/user-revokesigninsessions.md)                                | 无                                                                             | 通过将 **signInSessionsValidFromDateTime** 用户属性重置为当前的日期时间来吊销向应用程序发出的用户的所有刷新和会话令牌。 这将强制用户再次登录到这些应用程序。 |
| **驱动器**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [获取驱动器](../api/drive-get.md)                                                           | [drive](drive.md)                                                                | 检索驱动器资源的属性和关系。                                                                                                                                                                      |
| [列出子项](../api/driveitem-list-children.md)                                         | [DriveItems](driveitem.md)                                                       | 在 DriveItem 的子项关系中返回 DriveItems 集合。                                                                                                                                                      |
| **组**                                                                                 |                                                                                  |                                                                                                                                                                                                                                     |
| [List joinedTeams](../api/user-list-joinedteams.md)                                        | [团队](team.md) 集合                                                       | 从 joinedTeams 导航属性中获取此用户直接所属的 Microsoft Teams 团队。                                                                                                                         |
| [List memberOf](../api/user-list-memberof.md)                                              | [directoryObject](directoryobject.md) 集合                                 | 从 memberOf 导航属性中获取此用户是其直接成员的组和目录角色。                                                                                                                       |
| [List transitive memberOf](../api/user-list-transitivememberof.md)                         | [directoryObject](directoryobject.md) collection                                 | 列出用户所属的组和目录角色。 此操作是可传递的，并包括用户以嵌套方式所属的组。                                                                         |
| **邮件**                                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [创建 inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | 创建由 SMTP 地址识别的发件人的重点收件箱替代。      |                                                                                                                                                                                                                                     |
| [Create mailFolder](../api/user-post-mailfolders.md)                                       | [mailFolder](mailfolder.md)                                                      | 通过发布到 mailFolders 集合创建新 MailFolder。                                                                                                                                                                   |
| [创建邮件](../api/user-post-messages.md)                                             | [邮件](message.md)                                                            | 通过发布到邮件集合新建邮件。                                                                                                                                                                         |
| [创建 messageRule](../api/mailfolder-post-messagerules.md)                               | [messageRule](messagerule.md)                                                    | 通过指定一组条件和操作来创建 messageRule 对象。                                                                                                                                                          |
| [getMailTips](../api/user-getmailtips.md)                                                  | [邮件提醒](mailtips.md)集合                                               | 返回向已登录用户提供的一个或多个收件人的邮件提醒。                                                                                                                                                   |
| [List mailFolders](../api/user-list-mailfolders.md)                                        | [mailFolder](mailfolder.md) 集合                                           | 在已登录用户的根文件夹下获取邮件文件夹集合。                                                                                                                                                         |
| [列出邮件](../api/user-list-messages.md)                                              | [message](message.md) 集合                                                 | 获取已登录用户的邮箱中的所有邮件。                                                                                                                                                                               |
| [列出替代](../api/inferenceclassification-list-overrides.md)                         | [inferenceClassificationOverride](inferenceclassificationoverride.md) 集合 | 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的重点收件箱替代。                                                                                                           |
| [List rules](../api/mailfolder-list-messagerules.md)                                       | [messageRule](messagerule.md) 集合                                         | 获取为用户收件箱定义的所有 messageRule 对象。                                                                                                                                                                       |
| [发送邮件](../api/user-sendmail.md)                                                       | None                                                                             | 发送请求正文中指定的邮件。                                                                                                                                                                                     |
| **备注**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [创建笔记本](../api/onenote-post-notebooks.md)                                        | [笔记本](notebook.md)                                                          | 新建 OneNote 笔记本。                                                                                                                                                                                                      |
| [列出笔记本](../api/onenote-list-notebooks.md)                                         | [notebook](notebook.md) 集合                                               | 检索 notebook 对象列表。                                                                                                                                                                                                |
| **开放扩展**                                                                        |                                                                                  |                                                                                                                                                                                                                                     |
| [创建开放扩展](../api/opentypeextension-post-opentypeextension.md)                | [openTypeExtension](opentypeextension.md)                                        | 创建开放扩展，并将自定义属性添加到新资源或现有资源。                                                                                                                                                   |
| [获取开放扩展](../api/opentypeextension-get.md)                                      | [openTypeExtension](opentypeextension.md) 集合                             | 获取扩展名称标识的开放扩展。                                                                                                                                                                             |
| **组织层次结构**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [分配管理器](../api/user-post-manager.md)                                              | [directoryObject](directoryobject.md)                                            | 分配用户或组织联系人，作为该用户的经理。                                                                                                                                                                  |
| [获取管理器](../api/user-list-manager.md)                                                 | [directoryObject](directoryobject.md)                                            | 从 manager 导航属性中获取是此用户的经理的用户或组织联系人。                                                                                                                            |
| [List directReports](../api/user-list-directreports.md)                                    | [directoryObject](directoryobject.md) 集合                                 | 从 directReports 导航属性中获取向此用户报告的用户和联系人。                                                                                                                                      |
| **Outlook 设置**                                                                       |                                                                                  |                                                                                                                                                                                                                                     |
| [创建 Outlook 类别](../api/outlookuser-post-mastercategories.md)                     | [outlookCategory](outlookcategory.md)                                            | 在用户主类别列表中创建 outlookCategory 对象。                                                                                                                                                           |
| [获取 supportedLanguages](../api/outlookuser-supportedlanguages.md)                         | [localeInfo](localeinfo.md) 集合                                           | 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。                                                                                                                  |
| [获取 supportedTimeZones](../api/outlookuser-supportedtimezones.md)                         | [timeZoneInformation](timezoneinformation.md collection)                         | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。                                                                                                                             |
| [获取用户的邮箱设置](../api/user-get-mailboxsettings.md)                            | [mailboxSettings](mailboxsettings.md)                                            | 获取用户的 mailboxSettings。                                                                                                                                                                                                     |
| [列出 Outlook 类别](../api/outlookuser-list-mastercategories.md)                     | [outlookCategory](outlookcategory.md) 集合                                 | 获取为用户定义的所有类别。                                                                                                                                                                         |
| [转换 Exchange ID](../api/user-translateexchangeids.md)                              | [convertIdResult](convertidresult.md) 集合                                 | 对与 Outlook 相关的资源的标识符进行格式转换。                                                                                                                                                                 |
| [更新用户邮箱设置](../api/user-update-mailboxsettings.md)                      | [mailboxSettings](mailboxsettings.md)                                            | 启用、配置或禁用一个或多个用户的 mailboxSettings。                                                                                                                                                                   |
| **照片**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [获取照片](../api/profilephoto-get.md)                                                    | [profilePhoto](profilephoto.md)                                                  | 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。                                                                                                                                                           |
| [更新 profilephoto](../api/profilephoto-update.md)                                       | 无                                                                             | 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。                                                                                                                        |
| **计划表**                                                                                |                                                                                  |                                                                                                                                                                                                                                     |
| [List tasks](../api/planneruser-list-tasks.md)                                             | [plannerTask](plannertask.md) 集合                                         | 获取分配给此用户的 plannerTasks。                                                                                                                                                                                              |
| **架构扩展**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [添加架构扩展值](/graph/extensibility-schema-groups)                          | 无                                                                             | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。                                                                                                                                        |
| **用户设置**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [获取设置](../api/usersettings-get.md)                                                 | [userSettings](usersettings.md)                                                  | 阅读用户和组织设置对象。                                                                                                                                                                                     |
| [更新设置](../api/usersettings-update.md)                                           | [userSettings](usersettings.md)                                                  | 更新 settings 对象的属性。                                                                                                                                                                                       |

## <a name="properties"></a>属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|aboutMe|String|任意形式的文本输入字段，用于介绍用户自身。|
|accountEnabled|布尔| **true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.    |
|ageGroup|String|设置用户的年龄组。 允许的值：`null`、`minor`、`notAdult` 和 `adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|The licenses that are assigned to the user. Not nullable.            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|The plans that are assigned to the user. Read-only. Not nullable. |
|birthday|DateTimeOffset|The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|businessPhones|字符串集合|The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.|
|城市|String|The city in which the user is located. Supports $filter.|
|companyName | String | 与用户关联的公司名称。 此属性可用于描述外部用户所属的公司。 |
|consentProvidedForMinor|String|设置是否已获得未成年人的同意。 允许的值：`null`、`granted`、`denied` 和 `notRequired`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。|
|country|String|The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.|
|createdDateTime | DateTimeOffset |用户对象的创建日期。 |
|creationType|字符串|指示创建的用户帐户是普通学校或工作帐户 (`null`)、外部帐户 (`Invitation`)、Azure Active Directory B2C 租户的本地帐户 (`LocalAccount`) 还是使用电子邮件验证的自助注册帐户 (`EmailVerified`)。 只读。|
|deletedDateTime| DateTimeOffset | 删除用户的日期和时间。 <br><br>仅在 $select 上返回。 |
|department|String|The name for the department in which the user works. Supports $filter.|
|displayName|String|The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|employeeId|String|由组织分配给该用户的员工标识符。 支持 $filter。|
|externalUserState|String|对于使用[邀请 API](../api/invitation-post.md) 邀请到租户的外部用户，此属性表示受邀用户的邀请状态。 对于受邀用户，状态可以是 `PendingAcceptance` 或 `Accepted`，而对于所有其他用户，状态为 `null`。 <br><br>仅在上返回 `$select` 。 支持 `$filter` 具有受支持的值。 例如：`$filter=externalUserState eq 'PendingAcceptance'`。|
|externalUserStateChangeDateTime|DateTimeOffset|显示**externalUserState**属性的最新更改的时间戳。 <br><br>仅在上返回 `$select` 。|
|faxNumber|String|用户的传真号。|
|givenName|String|The given name (first name) of the user. Supports $filter.|
|hireDate|DateTimeOffset|The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|id|String|The unique identifier for the user. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.|
|identities|[objectIdentity](objectIdentity.md) 集合| 表示可用于登录此用户帐户的标识。 标识可由 Microsoft （也称为本地帐户）、组织或社交身份提供商（如 Facebook、Google 和 Microsoft）提供，并绑定到用户帐户。 可能包含具有相同 **signInType** 值的多个项目。 <br>支持 $filter。|
|imAddresses|String collection|The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.|
|interests|String collection|用户介绍自身兴趣的列表。|
|isResourceAccount|Boolean| 如果用户是资源帐户，则为 **true**，否则为 **false**。 Null 值应视为 **false**。|
|jobTitle|String|The user’s job title. Supports $filter.|
|lastPasswordChangeDateTime| DateTimeOffset | 此 Azure AD 用户上次更改其密码的时间。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”|
|legalAgeGroupClassification|String| 由企业应用程序用于确定用户的法定年龄组。 此属性为只读状态，基于 `ageGroup` 和 `consentProvidedForMinor` 属性计算得出。 允许的值：`null`、`minorWithOutParentalConsent`、`minorWithParentalConsent`、`minorNoParentalConsentRequired`、`notAdult` 和 `adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md) 集合|此用户的许可证分配状态。 只读。|
|mail|String|The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com". Read-Only. Supports $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Settings for the primary mailbox of the signed-in user. You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) settings for sending automatic replies to incoming messages, locale and time zone.|
|mailNickname|String|The mail alias for the user. This property must be specified when a user is created. Supports $filter.|
|mobilePhone|String|用户的主要移动电话号码。|
|mySite|String|用户个人网站的 URL。|
|officeLocation|String|用户公司地点的办公室位置。|
|onPremisesDistinguishedName|String| 包含本地 Active Directory `distinguished name` 或 `DN`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 |
|onPremisesDomainName|String| 包含从本地目录同步的本地 `domainFQDN`（也称为 dnsDomainName）。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|包含用户的 extensionAttributes 1-15。 请注意，单个扩展属性既不可选择，也不可筛选。 对于 `onPremisesSyncEnabled` 用户，此属性集是在本地主控的，并且为只读。 对于只使用云的用户（其中 `onPremisesSyncEnabled` 为 false），可以在创建或更新期间设置这些属性。 |
|onPremisesImmutableId|字符串|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。 如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。 **重要说明：** 指定此属性时不能使用 **$** 和 **\_** 字符。 支持 $filter。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indicates the last time at which the object was synced with the on-premises directory; for example: "2013-02-16T03:04:54Z". The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合| 在预配期间使用 Microsoft 同步产品时发生的错误。 |
|onPremisesSamAccountName|字符串| 包含从本地目录同步的本地 `samAccountName`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 |
|onPremisesSecurityIdentifier|String|Contains the on-premises security identifier (SID) for the user that was synchronized from on-premises to the cloud. Read-only.|
|onPremisesSyncEnabled|Boolean| **true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default). Read-only |
|onPremisesUserPrincipalName|String| 包含从本地目录同步的本地 `userPrincipalName`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 |
|otherMails|String| 用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。 支持 $filter。|
|passwordPolicies|String|Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.|
|pastProjects|String collection|供用户枚举其过去项目的列表。|
|postalCode|String|The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.|
|preferredDataLocation|String|用户的首选数据位置。 有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。|
|preferredLanguage|String|The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".|
|preferredName|String|用户的首选名称。|
|provisionedPlans|[provisionedPlan](provisionedplan.md) 集合|The plans that are provisioned for the user. Read-only. Not nullable. |
|proxyAddresses|String collection|For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties. Read-only, Not nullable. Supports $filter.|
|refreshTokensValidFromDateTime|DateTimeOffset|在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 <br><br>仅在 $select 上返回。 只读。 |
|responsibilities|String collection|供用户枚举其职责的列表。|
|schools|String collection|供用户枚举其学习过的学校列表。|
|showInAddressList|Boolean|如果 Outlook 全局地址列表应包含此用户，则值为 **true**，否则为 **false**。 如果未设置，则将其视为 **true**。 对于通过邀请管理器邀请的用户，此属性将设置为 **false**。|
|skills|String collection|供用户枚举其技能的列表。|
|signInSessionsValidFromDateTime|DateTimeOffset| 在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 此为只读属性。 使用 [revokeSignInSessions](../api/user-revokesigninsessions.md) 进行重置。|
|state|String|The state or province in the user's address. Supports $filter.|
|streetAddress|String|用户公司地点的街道地址。|
|surname|String|The user's surname (family name or last name). Supports $filter.|
|usageLocation|字符串|A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.|
|userPrincipalName|字符串|The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](organization.md). Supports $filter and $orderby.
|userType|String|A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.          |

### <a name="legal-age-group-property-definitions"></a>法定年龄组属性定义

本部分介绍 Azure AD 管理员和企业应用程序开发人员如何使用三个法定年龄组属性（`legalAgeGroupClassification`、`ageGroup` 和 `consentProvidedForMinor`）来满足与年龄相关的法规。

例如：Cameron 是英国 Holyport 小学的名录管理员。 新学年开始，他根据英国与年龄相关的法规，使用入学文件获得未成年人父母的同意。 征得父母同意后，Holyport 学校和 Microsoft 应用可以使用未成年人的帐户。 Cameron 随后创建所有帐户，将 ageGroup 设置为“minor”，并将 consentProvidedForMinor 设置为“granted”。 然后，他的学生使用的应用程序可以禁止不适合未成年人的功能。

#### <a name="legal-age-group-classification"></a>法定年龄组分类

企业应用程序开发人员使用此只读属性来确保根据用户的法定年龄组正确处理用户。 此属性是基于用户的 `ageGroup` 和 `consentProvidedForMinor` 属性计算得出的。

| 值    | #  |说明|
|:---------------|:--------|:----------|
|空|0|默认值，尚未给用户设置 `ageGroup`。|
|minorWithoutParentalConsent |1 |（保留以备今后使用）|
|minorWithParentalConsent|双面| 根据用户所在国家或地区与年龄相关的法规，将用户视为未成年人，并且帐户管理员已相应获得父母或监护人的同意。|
|adult|第三章|根据用户所在国家或地区与年龄相关的法规，将用户视为成年人。|
|notAdult|4 |用户所在国家或地区存在其他与年龄相关的法规（例如美国、英国、欧盟和韩国），用户的年龄介于未成年人和成年人之间（根据所在国家或地区的规定）。 通常，这意味着会在管控的国家或地区将青少年视为 `notAdult`。|
|minorNoParentalConsentRequired|5 |用户是未成年人，但所在国家或地区没有与年龄相关的法规。|

#### <a name="age-group-and-minor-consent"></a>年龄组和未成年人同意

年龄组和未成年人同意属性是 Azure AD 管理员使用的可选属性，可帮助确保根据用户所在国家或地区与年龄相关的监管规则正确处理帐户的使用。

#### <a name="agegroup-property"></a>ageGroup 属性

| 值    | #  |说明|
|:---------------|:--------|:----------|
|空|0|默认值，尚未给用户设置 `ageGroup`。|
|minor|1 |用户被视为次要。|
|notAdult|双面|用户所在国家或地区存在其他法规（例如美国、英国、欧盟和韩国），用户年龄超过儿童年龄上限（根据所在国家或地区的规定）且低于成年人年龄下限（根据所在国家或地区的规定）。 因此，基本上会在管控的国家或地区将青少年视为 `notAdult`。|
|adult|第三章|应将用户视为成年人。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor 属性

| 值    | #  |说明|
|:---------------|:--------|:----------|
|空|0|默认值，尚未给用户设置 `consentProvidedForMinor`。|
|granted|1 |已就用户拥有帐户获得同意。|
|denied|双面|尚未就用户拥有帐户获得同意。|
|notRequired|第三章|用户所在地不要求获得同意。|

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|activities|[userActivity](projectrome-activity.md) 集合|跨设备的用户活动。 此为只读属性。 可为 NULL。|
|日历|[calendar](calendar.md)|The user's primary calendar. Read-only.|
|calendarGroups|[CalendarGroup](calendargroup.md) 集合|The user's calendar groups. Read-only. Nullable.|
|calendarView|[event](event.md) 集合|The calendar view for the calendar. Read-only. Nullable.|
|calendars|[calendar](calendar.md) 集合|The user's calendars. Read-only. Nullable.|
|contactFolders|[ContactFolder](contactfolder.md) 集合|The user's contacts folders. Read-only. Nullable.|
|contacts|[contact](contact.md) 集合|The user's contacts. Read-only. Nullable.|
|createdObjects|[directoryObject](directoryobject.md) 集合|Directory objects that were created by the user. Read-only. Nullable.|
|directReports|[directoryObject](directoryobject.md) 集合|The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable. |
|drive|[drive](drive.md)|The user's OneDrive. Read-only.|
|drives|[drive](drive.md) 集合| A collection of drives available for this user. Read-only. |
|events|[event](event.md) 集合|The user's events. Default is to show Events under the Default Calendar. Read-only. Nullable.|
|extensions|[扩展](extension.md)集合|The collection of open extensions defined for the user. Read-only. Nullable.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|insights|[officeGraphInsights](officegraphinsights.md) | Read-only. Nullable.|
|licenseDetails|[licenseDetails](licensedetails.md) 集合|此用户许可证详细信息的集合。 只读。|
|mailFolders|[mailFolder](mailfolder.md) 集合| The user's mail folders. Read-only. Nullable.|
|manager|[directoryObject](directoryobject.md)|The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)|
|memberOf|[directoryObject](directoryobject.md) 集合|The groups and directory roles that the user is a member of. Read-only. Nullable.|
|messages|[message](message.md) 集合|The messages in a mailbox or folder. Read-only. Nullable.|
|onenote|[onenote](onenote.md)| 只读。|
|outlook|[outlookUser](outlookuser.md)| 只读。|
|ownedDevices|[directoryObject](directoryobject.md) collection|Devices that are owned by the user. Read-only. Nullable.|
|ownedObjects|[directoryObject](directoryobject.md) 集合|Directory objects that are owned by the user. Read-only. Nullable.|
|people|[person](person.md) 集合| 与用户相关的人员。 此为只读属性。 可为 NULL。
|photo|[profilePhoto](profilephoto.md)| The user's profile photo. Read-only.|
|planner|[plannerUser](planneruser.md)| 用户可能存在的 Planner 资源入口点。 只读。|
|registeredDevices|[directoryObject](directoryobject.md) collection|Devices that are registered for the user. Read-only. Nullable.|

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
  "createdDateTime": "String (timestamp)",
  "creationType": "string",
  "department": "string",
  "displayName": "string",
  "employeeId": "string",
  "faxNumber" : "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "imAddresses": ["string"],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "lastPasswordChangeDateTime": "String (timestamp)",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDistinguishedName": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "otherMails": "string",
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
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
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

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
