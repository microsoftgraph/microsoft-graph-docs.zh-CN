---
title: 用户资源类型
description: 表示 Azure AD 用户帐户。继承自 directoryObject。
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d51294b3325ead09cbf679904a9de5b33248bbac
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788561"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

表示 Azure Active Directory (Azure AD) 用户帐户。 此资源是允许传入其他属性的开放类型。 继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [List users](../api/user-list.md) | [user](user.md) 集合 | 获取用户对象列表。 |
| [Create user](../api/user-post-users.md) | [user](user.md) | 新建用户对象。 |
| [Get user](../api/user-get.md) | [user](user.md) | 读取 user 对象的属性和关系。 |
| [Update user](../api/user-update.md) | [user](user.md) | 更新 user 对象。 |
| [Delete user](../api/user-delete.md) | None | 删除 user 对象。 |
| [获取增量](../api/user-delta.md) | [user](user.md) 集合 | 获取用户的增量更改。 |
| [ChangePassword](../api/user-changepassword.md) | 无 | 更新自己的密码。 |
| **应用角色分配** |  |  |
| [列出 appRoleAssignments](../api/user-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) 集合 | 获取分配给此用户的应用和应用角色。 |
| [添加 appRoleAssignment](../api/user-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | 为此用户分配应用角色。 |
| [删除应用角分配](../api/user-delete-approleassignments.md) | 无 | 删除分配给此用户的应用角色。 |
| **Calendar** |  |  |
| [Create calendar](../api/user-post-calendars.md) | [Calendar](calendar.md) | 通过发布到日历集合创建新日历。 |
| [Create calendarGroup](../api/user-post-calendargroups.md) | [CalendarGroup](calendargroup.md) | 通过发布到 calendarGroups 集合新建 CalendarGroup。 |
| [Create event](../api/user-post-events.md) | [event](event.md) | 通过发布到事件集合新建事件。 |
| [findMeetingTimes](../api/user-findmeetingtimes.md) | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) | 基于与会者忙闲状态、位置或时间限制查找会议时间和位置。 |
| [getSchedule](../api/calendar-getschedule.md) | [scheduleInformation](scheduleinformation.md) | 获取用户、通讯组列表或资源（会议室或设备）在指定时间段内的忙/闲状态信息。 |
| [List calendars](../api/user-list-calendars.md) | [calendar](calendar.md) 集合 | 获取 Calendar 对象集合。 |
| [List calendarGroups](../api/user-list-calendargroups.md) | [calendarGroup](calendargroup.md) 集合 | 获取 CalendarGroup 对象集合。 |
| [List calendarView](../api/user-list-calendarview.md) | [event](event.md) 集合 | 获取 Event 对象集合。 |
| [List events](../api/user-list-events.md) | [event](event.md) 集合 | 获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。 |
| [reminderView](../api/user-reminderview.md) | [Reminder](reminder.md) collection | 返回指定开始时间和结束时间范围内的日历提醒列表。 |
| **联系人** |  |  |
| [创建联系人](../api/user-post-contacts.md) | [联系人](contact.md) | 通过发布到联系人集合新建联系人。 |
| [创建 contactFolder](../api/user-post-contactfolders.md) | [contactFolder](contactfolder.md) | 通过发布到 contactFolders 集合创建新 ContactFolder。 |
| [List contacts](../api/user-list-contacts.md) | [联系人](contact.md)集合 | 从已登录用户的默认联系人文件夹中获取联系人集合。 |
| [List contactFolders](../api/user-list-contactfolders.md) | [ContactFolder](contactfolder.md) 集合 | 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。 |
| **目录对象** |  |  |
| [assignLicense](../api/user-assignlicense.md) | [user](user.md) | 为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。 |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | String collection | 检查组列表中的成员身份。检查是可传递的。 |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。该函数可传递。 |
| [exportPersonalData](../api/user-exportpersonaldata.md) | 无 | 提交公司管理员发出的数据策略操作请求，以导出组织用户的数据。 |
| [getByIds](../api/directoryobject-getbyids.md) | 字符串集合 | 返回 ID 列表中指定的目录对象。 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | String collection | 返回用户是其成员的所有组。检查是可传递的。 |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | String collection | 返回用户所属的所有组、管理单元和目录角色。检查是可传递的。 |
| [List createdObjects](../api/user-list-createdobjects.md) | [directoryObject](directoryobject.md) collection | 从 createdObjects 导航属性中获取此用户创建的目录对象。 |
| [List licenseDetails](../api/user-list-licensedetails.md) | [licenseDetails](licensedetails.md) 集合 | 获取 licenseDetails 对象集合。 |
| [List ownedDevices](../api/user-list-owneddevices.md) | [directoryObject](directoryobject.md) collection | 从 ownedDevices 导航属性中获取此用户所拥有的设备。 |
| [List ownedObjects](../api/user-list-ownedobjects.md) | [directoryObject](directoryobject.md) collection | 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。 |
| [List registeredDevices](../api/user-list-registereddevices.md) | [directoryObject](directoryobject.md) collection | 从 registeredDevices 导航属性中获取为此用户注册的设备。 |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md) | [user](user.md) | 重新处理用户的订阅分配。 |
| [revokeSignInSessions](../api/user-revokesigninsessions.md) | 无 | 通过将 **signInSessionsValidFromDateTime** 用户属性重置为当前的日期时间来吊销向应用程序发出的用户的所有刷新和会话令牌。 这将强制用户再次登录到这些应用程序。 |
| [列出已删除的组](../api/directory-deleteditems-list.md) | [directoryObject](directoryobject.md) 集合 | 检索租户中过去 30 天内被删除的组。 |
| [列出用户拥有的已删除组](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | 检索租户中最近 30 天内删除的用户所有的组。 |
| [获取已删除的组](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) collection | 按 ID 检索已删除的组。 |
| [恢复已删除的组](../api/directory-deleteditems-delete.md) | [directoryObject](directoryobject.md) 集合 | 还原最近 30 天内在租户中删除的组。 |
| [永久删除组](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) collection | 从租户中永久删除已删除的组。 |
| **驱动器** |  |  |
| [获取驱动器](../api/drive-get.md) | [drive](drive.md) | 检索 Drive 资源的属性和关系。 |
| [列出子项](../api/driveitem-list-children.md) | [DriveItems](driveitem.md) | 在 DriveItem 的子项关系中返回 DriveItems 集合。 |
| **组** |  |  |
| [List joinedTeams](../api/user-list-joinedteams.md) | [团队](team.md) 集合 | 从 joinedTeams 导航属性中获取此用户直接所属的 Microsoft Teams 团队。 |
| [List memberOf](../api/user-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 获取用户直接所属的组、目录角色和管理单元。 此操作不可传递。 |
| [列出 transitiveMemberOf](../api/user-list-transitivememberof.md) | [directoryObject](directoryobject.md) 集合 | 获取用户直接所属或通过传递成员身份所属的组、目录角色和管理单元。 |
| **邮件** |  |  |
| [创建 inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | 创建由 SMTP 地址识别的发件人的重点收件箱替代。 |  |
| [Create mailFolder](../api/user-post-mailfolders.md) | [mailFolder](mailfolder.md) | 通过发布到 mailFolders 集合创建新 MailFolder。 |
| [创建邮件](../api/user-post-messages.md) | [邮件](message.md) | 通过发布到邮件集合新建邮件。 |
| [创建 messageRule](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) | 通过指定一组条件和操作来创建 messageRule 对象。 |
| [getMailTips](../api/user-getmailtips.md) | [邮件提醒](mailtips.md)集合 | 返回向已登录用户提供的一个或多个收件人的邮件提醒。 |
| [List mailFolders](../api/user-list-mailfolders.md) | [mailFolder](mailfolder.md) 集合 | 在已登录用户的根文件夹下获取邮件文件夹集合。 |
| [列出邮件](../api/user-list-messages.md) | [message](message.md) 集合 | 获取已登录用户的邮箱中的所有邮件。 |
| [列出替代](../api/inferenceclassification-list-overrides.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) 集合 | 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的重点收件箱替代。 |
| [List rules](../api/mailfolder-list-messagerules.md) | [messageRule](messagerule.md) 集合 | 获取为用户收件箱定义的所有 messageRule 对象。 |
| [发送邮件](../api/user-sendmail.md) | 无 | 发送请求正文中指定的邮件。 |
| **备注** |  |  |
| [创建笔记本](../api/onenote-post-notebooks.md) | [笔记本](notebook.md) | 新建 OneNote 笔记本。 |
| [列出笔记本](../api/onenote-list-notebooks.md) | [notebook](notebook.md) 集合 | 检索 notebook 对象列表。 |
| **开放扩展** |  |  |
| [创建开放扩展](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | 创建开放扩展，并将自定义属性添加到新资源或现有资源。 |
| [获取开放扩展](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) 集合 | 获取扩展名称标识的开放扩展。 |
| **组织层次结构** |  |  |
| [分配管理器](../api/user-post-manager.md) | [directoryObject](directoryobject.md) | 分配用户或组织联系人，作为该用户的经理。 |
| [获取管理器](../api/user-list-manager.md) | [directoryObject](directoryobject.md) | 从 manager 导航属性中获取是此用户的经理的用户或组织联系人。 |
| [List directReports](../api/user-list-directreports.md) | [directoryObject](directoryobject.md) collection | 从 directReports 导航属性中获取向此用户报告的用户和联系人。 |
| **Outlook 设置** |  |  |
| [创建 Outlook 类别](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) | 在用户主类别列表中创建 outlookCategory 对象。 |
| [获取 supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) 集合 | 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。 |
| [获取 supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md collection) | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。 |
| [获取用户的邮箱设置](../api/user-get-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | 获取用户的 mailboxSettings。 |
| [列出 Outlook 类别](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) 集合 | 获取为用户定义的所有类别。 |
| [转换 Exchange ID](../api/user-translateexchangeids.md) | [convertIdResult](convertidresult.md) 集合 | 对与 Outlook 相关的资源的标识符进行格式转换。 |
| [更新用户邮箱设置](../api/user-update-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | 启用、配置或禁用一个或多个用户的 mailboxSettings。 |
| **照片** |  |  |
| [获取照片](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) | 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。 |
| [更新 profilephoto](../api/profilephoto-update.md) | 无 | 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 |
| **计划表** |  |  |
| [List tasks](../api/planneruser-list-tasks.md) | [plannerTask](plannertask.md) 集合 | 获取分配给此用户的 plannerTasks。 |
| **架构扩展** |  |  |
| [添加架构扩展值](/graph/extensibility-schema-groups) | 无 | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。 |
| **Teamwork** |  |  |
| [列出为用户安装的应用](../api/userteamwork-list-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出安装在用户个人范围内的应用。 |
| [获取为用户安装的应用](../api/userteamwork-get-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 列出安装在用户个人范围内的指定应用。 |
| [为用户添加应用](../api/userteamwork-post-installedapps.md) | 无 | 在用户的个人范围内添加（安装）应用。 |
| [为用户删除应用](../api/userteamwork-delete-installedapps.md) | 无 | 删除（卸载）用户个人范围内的应用。 |
| [升级为用户安装的应用](../api/userteamwork-teamsappinstallation-upgrade.md) | 无 | 将安装在用户个人范围内的应用升级到最新版本。 |
| [获取用户和应用之间的聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md) | 列出用户和应用之间的一对一聊天。 |
| **待办任务** |  |  |
| [创建任务](../api/todotasklist-post-tasks.md) | [todoTask](todotask.md) | 在指定的任务列表中创建 [todoTask](todotask.md)。 |
| [创建任务列表](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在用户的邮箱中创建微软待办任务列表。 |
| [列出任务](../api/todotasklist-list-tasks.md) | [todoTask](todotask.md) 集合 | 获取指定列表中的所有 [todoTask](todotask.md) 资源。 |
| [列出任务列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户邮箱中的所有任务列表。 |
| **用户设置** |  |  |
| [获取设置](../api/usersettings-get.md) | [userSettings](usersettings.md) | 阅读用户和组织设置对象。 |
| [更新设置](../api/usersettings-update.md) | [userSettings](usersettings.md) | 更新 settings 对象的属性。 |


## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#user-properties)。

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|aboutMe|String|任意多边形的文本输入字段，用于介绍用户自身。仅在 `$select` 上返回。|
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。创建用户时此属性是必需的。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`和 `in`）。    |
|ageGroup|[ageGroup](#agegroup-values)|设置用户的年龄组。 允许的值：`null`、`Minor`、`NotAdult` 和 `Adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`和 `in`）。|
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|已分配给用户的许可证，包括继承的（基于组的）许可证。  不可为 null。 仅在 `$select` 上返回。 支持 `$filter`（`eq`、`not` 和计数空集合）。           |
|assignedPlans|[assignedPlan](assignedplan.md) collection|分配给该用户的计划。只读。不可为 null。<br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq` 和 `not`）。 |
|birthday|DateTimeOffset|用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>仅在 `$select` 上返回。|
|businessPhones|字符串集合|用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。本地目录同步的用户为只读。<br><br>默认返回。支持 `$filter` （`eq`、 `not`、 `ge`、 `le`、 `startsWith`）。|
|城市|String|用户所在的城市。最大长度为 128 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|CompanyName | String | 与用户关联的公司名称。 此属性可用于描述外部用户所属的公司。 最大长度为 64 个字符。<br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|consentProvidedForMinor|[consentProvidedForMinor](#consentprovidedforminor-values)|设置是否已获得未成年人的同意。 允许的值：`null`、`Granted`、`Denied` 和 `NotRequired`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`和 `in`）。|
|country|String|用户所在的国家/地区，例如 `US` 或 `UK`。最大长度为 128 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|createdDateTime | DateTimeOffset |用户对象的创建日期。只读<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `ge`、 `le`、 `in`）。|
| creationType | 字符串 | 指示是否通过以下方法之一创建用户帐户： <br/> <ul><li>作为常规学校或工作帐户（`null`）。 <li>作为外部帐户（`Invitation`）。 <li>作为 Azure Active Directory B2C 租户的本地帐户（`LocalAccount`）。 <li>通过使用电子邮件验证由内部用户（`EmailVerified`）进行自助注册。 <li>通过由外部用户通过属于用户流的链接注册的自助注册（`SelfServiceSignUp`）。</ul> <br>只读。<br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`）。 |
|deletedDateTime| DateTimeOffset | 删除用户的日期和时间。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`）。 |
|department|String|用户工作部门的名称。 最大长度为 64 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in` 和 `null` 值上的 `eq`）。|
|displayName|字符串|用户通讯簿中显示的名称。通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。最大长度为 256 个字符。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）、`$orderBy` 和 `$search`。|
| employeeHireDate | DateTimeOffset | 聘请用户或用户将开始工作（如是未来招聘）的日期和时间。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `ge`、 `le`、 `in`）。|
| employeeId | String | 由组织分配给该用户的员工标识符。 最大长度为 16 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |表示与用户相关联的组织数据（例如，分部和 costCenter）。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `ge`、 `le`、 `in`）。|
| employeeType | String | 捕获企业员工类型。 例如，`Employee`、`Contractor`、`Consultant` 或 `Vendor`。 仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `ge`、 `le`、 `in`、 `startsWith`）。|
|externalUserState|String|对于使用[邀请 API](../api/invitation-post.md) 邀请到租户的外部用户，此属性表示受邀用户的邀请状态。 对于受邀用户，状态可以是 `PendingAcceptance` 或 `Accepted`，而对于所有其他用户，状态为 `null`。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `in`）。|
|externalUserStateChangeDateTime|DateTimeOffset|显示最近一次修改 **externalUserState** 属性的时间戳。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not` 、 `in`）。|
|faxNumber|String|用户的传真号。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|givenName|String|用户的名。 最大长度为 64 个字符。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
| hireDate | DateTimeOffset | 用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。<br><br>仅在 `$select` 上返回。 <br> **注意：** 此属性特定于 SharePoint Online。建议使用本机器 **employeeHireDate** 属性通过 Microsoft Graph API 设置和更新雇佣日期值。 |
|id|String|用户的唯一标识符。 应视为不透明的标识符。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 <br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`、`in`）。|
|identities|[objectIdentity](objectIdentity.md) 集合| 表示可用于登录此用户帐户的标识。 标识可由 Microsoft （也称为本地帐户）、组织或社交身份提供商（如 Facebook、Google 和 Microsoft）提供，并绑定到用户帐户。 可能包含具有相同 **signInType** 值的多个项目。 <br><br>仅在 `$select`返回。仅当 **signInType** 不是`userPrincipalName`时，支持包括在`null`值上的`$filter`（`eq`）。|
|imAddresses|String collection|用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `not`、 `ge`、 `le`、 `startsWith`）。|
|interests|String collection|用户介绍自身兴趣的列表。 <br><br>仅在 `$select` 上返回。|
|isResourceAccount|布尔| 请勿使用 – 保留以备今后使用。|
|jobTitle|String|用户的职务。 最大长度为 128 个字符。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|lastPasswordChangeDateTime| DateTimeOffset | 此 Azure AD 用户上次更改密码或创建密码的时间，以最新操作的日期为准。日期和时间信息使用 ISO 8601 格式，并且始终以 UTC 时间标识。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。<br><br>仅在 `$select` 上返回。|
|legalAgeGroupClassification|[legalAgeGroupClassification](#legalagegroupclassification-values)| 由企业应用程序用于确定用户的法定年龄组。 此属性为只读，并且基于 **ageGroup** 和 **consentProvidedForMinor** 属性进行计算。 允许的值：`null`、`MinorWithOutParentalConsent`、`MinorWithParentalConsent`、`MinorNoParentalConsentRequired`、`NotAdult` 和 `Adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>仅在 `$select` 上返回。|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md) 集合|此用户的许可证分配状态。只读。<br><br>仅在 `$select` 上返回。|
|mail|String|用户的 SMTP 地址，例如， `jeff@contoso.onmicrosoft.com`。 对此属性进行更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。 此属性不能包含突出字符。 <br/> **注意：** 不建议为 Azure AD B2C 用户配置文件更新此属性。 请改用 **otherMails** 属性。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith`、`endsWith` 和 `null` 值上的 `eq`）。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|已登录用户的主邮箱的设置。可以[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。<br><br>仅在 `$select` 上返回。|
|mailNickname|String|用户的邮件别名。创建用户时必须指定此属性。最大长度为 64 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|mobilePhone|String|用户的主要移动电话号码。 本地目录同步的用户为只读。 最大长度为 64 个字符。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。 |
|mySite|String|用户个人网站的 URL。 <br><br>仅在 `$select` 上返回。|
|officeLocation|String|用户公司地点的办公室位置。 <br><br>默认返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|onPremisesDistinguishedName|String| 包含本地 Active Directory `distinguished name` 或 `DN`。仅针对通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。只读。<br><br>仅在 `$select` 上返回。 |
|onPremisesDomainName|String| 包含本地 `domainFQDN`，也称为 dnsDomainName。仅为正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。只读。<br><br>仅在 `$select` 上返回。|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|包含用户的 extensionAttributes1-15。 这些扩展属性也称 Exchange 自定义属性 1-15。 <br><li>对于 **onPremisesSyncEnabled** 用户，这组属性集的授权来源是本地，并且为只读。 </li><li>对于仅限云用户（其中 **onPremisesSyncEnabled** 为 `false`），可以在创建或更新用户对象期间设置这些属性。  </li><li>对于以前从本地 Active Directory 同步的仅限云用户，这些属性在 Microsoft Graph 中为只读，但可以通过 Exchange 管理中心或 PowerShell 中的 Exchange Online V2 模块进行完全托管。</li><br> 仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`）。 |
|onPremisesImmutableId|String|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，在 Graph 中创建新用户帐户时必须指定此属性。**注意：** 指定该属性时不能使用 **$** 和 **\_** 字符。<br><br>仅在 `$select` 上返回。 支持 `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`)..                            |
|onPremisesLastSyncDateTime|DateTimeOffset|指示对象最后一次与本地目录同步的时间。例如：`2013-02-16T03:04:54Z`。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。只读。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`）。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合| 在预配期间使用 Microsoft 同步产品时发生的错误。 <br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `not`、 `ge`、 `le`）。|
|onPremisesSamAccountName|String| 包含从本地目录同步的本地 `samAccountName`。仅为通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。只读。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`、 `startsWith`）。|
|onPremisesSecurityIdentifier|String|包含从本地同步到云的用户的本地安全标识符 (SID)。只读。<br><br>仅在 `$select` 上返回。  支持 `$filter`（`eq`包括在 `null` 值上）。 |
|onPremisesSyncEnabled|Boolean| 如果当前正在从本地 Active Directory (AD) 同步此用户对象，则为 `true`；否则不会同步用户，并且可在 Azure Active Directory (Azure AD) 中进行管理。 只读。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。|
|onPremisesUserPrincipalName|String| 包含从本地目录同步的本地 `userPrincipalName`。仅为通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。只读。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`、 `startsWith`）。|
|otherMails|字符串集合| 用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。 <br>注意：此属性不能包含突出字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`not`、`ge`、`le`、`in`、`startsWith`、`endsWith` 和计数空集合）。|
|passwordPolicies|String|指定用户的密码策略。此值是一个枚举，其中一个可能的值为 `DisableStrongPassword`，这允许指定比默认策略更弱的密码。也可指定 `DisablePasswordExpiration`。两者可以一起指定，例如：`DisablePasswordExpiration, DisableStrongPassword`。<br><br>只在 `$select` 返回。有关默认密码策略的详细信息，请参阅 [Azure AD 密码策略](/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)。支持 `$filter` (`null` 值上的 `ne`、`not`、`eq`)。|
|passwordProfile|[passwordProfile](passwordprofile.md)|指定用户的密码配置文件。 配置文件包含用户的密码。 创建用户时此属性是必需的。 配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。 默认情况下，必须使用强密码。 **注意：** 对于 Azure B2C 租户， **forceChangePasswordNextSignIn** 属性应设置为 `false` ，并且应在第一次登录时使用自定义策略和用户流强制重置密码。 请参阅 [首次登录时强制重置](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon)。<br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。|
|pastProjects|String collection|供用户枚举其过去项目的列表。 <br><br>仅在 `$select` 上返回。|
|postalCode|String|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。最大长度为 40 个字符。<br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
| preferredDataLocation | String | 用户的首选数据位置。 有关详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。|
|preferredLanguage|String|用户的首选语言。应遵循 ISO 639-1 代码，例如 `en-US`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）|
|preferredName|String|用户的首选名称。 **不受支持。此属性返回空字符串。**<br><br>仅在 `$select` 上返回。|
|provisionedPlans|[provisionedPlan](provisionedplan.md) 集合|为用户设置的计划。只读。不可为 null。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `not`、 `ge`、 `le`）。|
|proxyAddresses|String collection|例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`。 对 **mail** 属性的更改还将更新此集合，以将值作为 SMTP 地址包含在内。 有关详细信息，请参阅 [mail 和 proxyAddresses 属性](#mail-and-proxyaddresses-properties)。 以 `SMTP`（大写）为前缀的代理地址是主代理地址，而前缀为 `smtp` 的代理地址则是辅助代理地址。 对于 Azure AD B2C 帐户，此属性有 10 个唯一地址的限制。 Microsoft Graph 中的只读；只能通过 [Microsoft 365 管理中心](/exchange/recipients-in-exchange-online/manage-user-mailboxes/add-or-remove-email-addresses) 来更新此属性。 不可为 null。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`、`endsWith` 和计数空集合）。|
|refreshTokensValidFromDateTime|DateTimeOffset|在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 <br><br>仅在 `$select` 返回。只读。 |
|responsibilities|String collection|供用户枚举其职责的列表。 <br><br>仅在 `$select` 上返回。|
|schools|String collection|供用户枚举其学习过的学校列表。 <br><br>仅在 `$select` 上返回。|
|showInAddressList|Boolean|**请勿在 Microsoft Graph 中使用。请改为通过 Microsoft 365 管理中心管理此属性。** 表示是否应将用户包含在 Outlook 全局地址列表中。 请参阅 [已知问题](/graph/known-issues#showinaddresslist-property-is-out-of-sync-with-microsoft-exchange)。|
|skills|String collection|供用户枚举其技能的列表。 <br><br>仅在 `$select` 上返回。|
|signInSessionsValidFromDateTime|DateTimeOffset| 在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 只读。 使用 [revokeSignInSessions](../api/user-revokesigninsessions.md) 进行重置。 <br><br>仅在 `$select` 上返回。|
|state|String|用户地址中的省/市/自治区或省。 最大长度为 128 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|streetAddress|String|用户公司地点的街道地址。 最大长度为 1024 个字符。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|surname|String|用户的姓氏。 最大长度为 64 个字符。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|usageLocation|String|两个字母的国家/地区代码（ISO 标准 3166）。 由于法律要求，将被分配许可证的用户需要检查国家/地区的服务可用性。 示例包括：`US`、`JP`、`GB`。不可为 null。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md)的 **verifiedDomains** 属性访问租户的已验证域。<br>注意：此属性不能包含突出字符。 仅支持使用以下字符：`A - Z`、`a - z`、`0 - 9`、` ' . - _ ! # ^ ~`。 有关允许字符的完整列表，请参阅[用户名策略](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts)。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`、 `startsWith`、 `endsWith`） 和 `$orderBy`。
|userType|String|可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。 **注意：** 有关成员和来宾用户权限的详细信息，请参阅 [Azure Active Directory 中的默认用户权限是什么？](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users)         |

> [!TIP]
> 目录和架构扩展及其关联数据仅在 `$select` 上返回；开放扩展及其关联的数据仅在 `$expand` 上返回。

### <a name="mail-and-proxyaddresses-properties"></a>mail 和 proxyAddresses 属性
**mail** 和 **proxyAddresses** 都是与电子邮件相关的属性。 **proxyAddresses** 是仅与 Microsoft Exchange 服务器相关的地址集合。 它用于存储绑定到单个邮箱的用户的邮件地址列表。 将 **mail** 属性用作用户的电子邮件地址具有包括用户登录在内的各种用途，同时该属性定义了主代理地址。
 
可通过 MS Graph 上的 [GET 用户](/graph/api/user-get) API 检索 **mail** 和 **proxyAdress**。 可以通过 [更新用户的 PATCH 方法](/graph/api/user-update) API 来更新 **mail**，但 **proxyAddresses** 无法通过 Microsoft Graph 进行更新。 更新用户的 **mail** 属性时，将触发重新计算 **proxyAddresses**，并将新更新的邮件设置为主要代理地址，但在以下方案中除外： 
 
1. 如果用户具有包含 Microsoft Exchange 的许可证，则其所有代理地址必须属于租户上的已验证域。任何不属于已验证域的域都将以无提示方式删除。
2. 如果用户是来宾，并且主代理地址包含具有 #EXT# 的来宾用户 UPN 字符串，则不会将用户的邮件设置为主代理地址。
3. 如果用户是来宾，则即使用户不再具有代理地址，也将不会删除用户的邮件。
 
**proxyAddresses** 在目录对象（用户、组和组织联系人）中是唯一的。如果用户的 **mail** 属性与另一个对象的 **proxyAddresses** 之一发生冲突，你将成功更新 **mail** 属性；但是，新邮件值将不会添加到 **proxyAddresses** 集合。

### <a name="legal-age-group-property-definitions"></a>法定年龄组属性定义

本部分介绍 Azure AD 管理员和企业应用程序开发人员如何使用三个年龄组属性（**legalAgeGroupClassification**、**ageGroup** 和 **consentProvidedForMinor**）来满足与年龄相关的法规：
- **legalAgeGroupClassification** 属性为只读属性。 企业应用程序开发人员使用此只读属性来确保根据用户的法定年龄组正确处理用户。 此属性是基于用户的 **ageGroup** 和 **consentProvidedForMinor** 属性计算得出的。
- **ageGroup** 和 **consentProvidedForMinor** 属性是 Azure AD 管理员使用的可选属性，可帮助确保根据用户所在国家或地区与年龄相关的监管规则正确处理帐户的使用。

例如：Cameron 是英国 Holyport 小学的名录管理员。 新学年开始，他根据英国与年龄相关的法规，使用入学文件获得未成年人父母的同意。 征得父母同意后，Holyport 学校和 Microsoft 应用可以使用未成年人的帐户。 Cameron 随后创建所有帐户，将 **ageGroup** 设置为 `minor`，**consentProvidedForMinor** 设置为 `granted`。 然后，他的学生使用的应用程序可以禁止不适合未成年人的功能。

<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience but they are String types.-->

#### <a name="legalagegroupclassification-values"></a>legalAgeGroupClassification values

| 成员    | 说明|
|:---------------|:----------|
|空|默认值，尚未给用户设置 **ageGroup**。|
|MinorWithoutParentalConsent |（保留以备今后使用）|
|MinorWithParentalConsent| 根据用户所在国家或地区与年龄相关的法规，将用户视为未成年人，并且帐户管理员已相应获得父母或监护人的同意。|
|Adult|根据用户所在国家或地区与年龄相关的法规，将用户视为成年人。|
|NotAdult|用户所在国家或地区存在其他与年龄相关的法规（例如美国、英国、欧盟、韩国），用户的年龄介于未成年人和成年人之间（根据所在国家或地区的规定）。一般来说，这意味着在有管控的国家，青少年被认为是 `notAdult`。|
|MinorNoParentalConsentRequired|用户是未成年人，但所在国家或地区没有与年龄相关的法规。|

#### <a name="agegroup-values"></a>ageGroup 值

| 成员    | 说明|
|:---------------|:--------|
|空|默认值，尚未给用户设置 **ageGroup**。|
|次要|该用户被视为未成年人。|
|NotAdult|用户所在国家或地区存在相关法规（例如美国、英国、欧盟或韩国），而且用户年龄超过儿童年龄上限（根据所在国家或地区的规定）且低于成年人年龄下限（根据所在国家或地区的规定）。基本上，这就意味着在有管控的国家，青少年被认为是 `notAdult`。|
|Adult|应将用户视为成年人。|

#### <a name="consentprovidedforminor-values"></a>consentProvidedForMinor 值

| 成员    | 说明|
|:---------------|:----------|
|空|默认值，尚未给用户设置 **consentProvidedForMinor**。|
|Granted|已就用户拥有帐户获得同意。|
|Denied|尚未就用户拥有帐户获得同意。|
|NotRequired|用户所在地不要求获得同意。|

## <a name="relationships"></a>关系

| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md) 集合| 用户的使用条款接受状态。只读。可以为 null。|
|activities|[userActivity](projectrome-activity.md) 集合|用户的跨设备活动。只读。可以为 null。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|表示用户已被授予的某个应用程序的应用角色。支持 `$expand`。 |
|身份验证|[身份验证](../resources/authentication.md)| 用户支持的身份验证方法。|
|日历|[calendar](calendar.md)|用户的主日历。只读。|
|calendarGroups|[CalendarGroup](calendargroup.md) 集合|用户的日历组。只读。可为 Null。|
|calendarView|[event](event.md) 集合|日历的日历视图。只读。可为 Null。|
|calendars|[calendar](calendar.md) 集合|用户的日历。只读。可为 Null。|
|contactFolders|[ContactFolder](contactfolder.md) 集合|用户的联系人文件夹。只读。可为 Null。|
|contacts|[contact](contact.md) 集合|用户的联系人。只读。可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) collection|由用户创建的 directory 对象。只读。可为 Null。|
|directReports|[directoryObject](directoryobject.md) collection|向此用户报告的用户和联系人（针对管理器属性设置为此用户的用户和联系人）。只读。可为 null。支持 `$expand`。 |
|驱动器|[drive](drive.md)|用户的 OneDrive。只读。|
|drives|[drive](drive.md) 集合| 该用户的可用驱动器集合。只读。 |
|events|[event](event.md) 集合|用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。|
|extensions|[扩展](extension.md)集合|为用户定义的开放扩展集合。 只读。 支持 `$expand`。 可为 Null。|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|insights|[officeGraphInsights](officegraphinsights.md) | 只读。可为空。|
|licenseDetails|[licenseDetails](licensedetails.md) 集合|此用户的许可证详细信息集合。只读。|
|mailFolders|[mailFolder](mailfolder.md) 集合| 用户的邮件文件夹。只读。可为 Null。|
|manager|[directoryObject](directoryobject.md)|是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）。支持 `$expand`。|
|memberOf|[directoryObject](directoryobject.md) 集合|用户所属的组和目录角色。只读。可为 Null。支持 `$expand`。 |
|messages|[message](message.md) 集合|邮箱或文件夹中的邮件。只读。可为 Null。|
|onenote|[onenote](onenote.md)| 只读。|
|outlook|[outlookUser](outlookuser.md)| 只读。|
|ownedDevices|[directoryObject](directoryobject.md) collection|用户拥有的设备。只读。可为 Null。支持 `$expand`。|
|ownedObjects|[directoryObject](directoryobject.md) 集合|用户拥有的目录对象。只读。可为 Null。支持 `$expand`。|
|people|[person](person.md) 集合| 与用户相关的人员。只读。可以为 null。
|photo|[profilePhoto](profilephoto.md)| 用户的个人资料照片。只读。|
|planner|[plannerUser](planneruser.md)| 对于用户可能存在的 Planner 资源入口点。只读。|
|registeredDevices|[directoryObject](directoryobject.md) collection|已注册的用户的设备。只读。可为空。支持 `$expand`。|
|todo|[todo](todo.md)|表示用户可以使用的微软待办服务。 |
|transitiveMemberOf| [directoryObject](directoryobject.md) 集合 |  用户所属的组（包括嵌套组）和目录角色。 可为 Null。|

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
  "aboutMe": "String",
  "accountEnabled": true,
  "ageGroup": "String",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["String"],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "String (timestamp)",
  "creationType": "String",
  "department": "String",
  "displayName": "String",
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "String",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "String",
  "faxNumber" : "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "id": "String (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "imAddresses": ["String"],
  "interests": ["String"],
  "isResourceAccount": false,
  "jobTitle": "String",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "lastPasswordChangeDateTime": "String (timestamp)",
  "mail": "String",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "String",
  "mobilePhone": "String",
  "mySite": "String",
  "officeLocation": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesDomainName": "String",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "String",
  "otherMails": ["String"],
  "passwordPolicies": "String",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["String"],
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "preferredName": "String",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["String"],
  "responsibilities": ["String"],
  "schools": ["String"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "skills": ["String"],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",

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
  ],
  "section": "documentation",
  "tocPath": ""
}-->

