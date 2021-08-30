---
title: 用户资源类型
description: 表示 Azure AD 用户帐户。继承自 directoryObject。
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 929f647a68e453529daaabf2b3f0b0dfdd3a76c7
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696965"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。

**用户** 资源允许应用指定语言的用户首选项，以及用户主要 Exchange 邮箱和 Azure AD 配置文件的日期/时间格式。 了解更多信息，请参阅 [语言和区域格式的用户首选项](#user-preferences-for-languages-and-regional-formats)。

出于性能原因，默认情况下 [create](../api/user-post-users.md)、[get](../api/user-get.md) 和 [list](../api/user-list.md) 操作仅返回更常用属性的子集。 这些默认属性将记录在[属性](#properties)部分中。 若要获取非默认返回的任一属性，请在 `$select` OData 查询选项中指定这些属性。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:------ |:----------- |:----------- |
| [List users](../api/user-list.md) | [user](user.md) 集合 | 获取用户对象列表。 |
| [Create user](../api/user-post-users.md) | [user](user.md) | 新建用户对象。 |
| [Get user](../api/user-get.md) | [user](user.md) | 读取 user 对象的属性和关系。 |
| [Update user](../api/user-update.md) | [user](user.md) | 更新 user 对象。 |
| [Delete user](../api/user-delete.md) | None | 删除 user 对象。 |
| [Get delta](../api/user-delta.md) | 用户集合 | 获取用户的增量更改。 |
| [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) | 无 | 使发给应用程序的所有用户刷新令牌无效。 |
| [ChangePassword](../api/user-changepassword.md) | 无 | 更新自己的密码。 |
| **应用角色分配**|||
| [列出 appRoleAssignments](../api/user-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) 集合 | 获取分配给此用户的应用和应用角色。 |
| [添加 appRoleAssignment](../api/user-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | 为此用户分配应用角色。 |
| [删除应用角分配](../api/user-delete-approleassignments.md) | 无 | 删除分配给此用户的应用角色。 |
| **Calendar** |||
| [Create calendar](../api/user-post-calendars.md) | [Calendar](calendar.md) | 通过发布到日历集合创建新日历。 |
| [Create calendarGroup](../api/user-post-calendargroups.md) | [CalendarGroup](calendargroup.md) | 通过发布到 calendarGroups 集合新建 CalendarGroup。 |
| [Create event](../api/user-post-events.md) | [event](event.md) | 通过发布到事件集合新建事件。 |
| [findMeetingTimes](../api/user-findmeetingtimes.md) | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) | 基于与会者忙闲状态、位置或时间限制查找会议时间和位置。 |
| [findRooms](../api/user-findrooms.md) | [emailaddress.md](emailaddress.md) 集合 | 获取用户租户中或特定房间列表中的所有会议室。 |
| [findRoomLists](../api/user-findroomlists.md) | [emailaddress.md](emailaddress.md) 集合 | 获取租户中定义的会议室列表。 |
| [getSchedule](../api/calendar-getschedule.md) | [scheduleInformation](scheduleinformation.md) | 获取用户、通讯组列表或资源（会议室或设备）在指定时间段内的忙/闲状态信息。 |
| [List calendars](../api/user-list-calendars.md) | [Calendar](calendar.md) collection | 获取 Calendar 对象集合。 |
| [List calendarGroups](../api/user-list-calendargroups.md) | [CalendarGroup](calendargroup.md) collection | 获取 CalendarGroup 对象集合。 |
| [List calendarView](../api/user-list-calendarview.md) | [event](event.md) 集合 | 获取 event 对象集合。 |
| [List events](../api/user-list-events.md) | [event](event.md) 集合 | 获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。 |
| [reminderView](../api/user-reminderview.md) | [Reminder](reminder.md) collection | 返回指定开始时间和结束时间范围内的日历提醒列表。|
| **联系人**|||
| [创建联系人](../api/user-post-contacts.md)| [contact](contact.md) | 通过发布到联系人集合创建新联系人。 |
| [创建 contactFolder](../api/user-post-contactfolders.md) | [contactFolder](contactfolder.md) | 通过发布到 contactFolders 集合创建新 contactFolder。 |
| [List contacts](../api/user-list-contacts.md) | [contact](contact.md) 集合 | 从已登录用户的默认联系人文件夹中获取联系人集合。 |
| [List contactFolders](../api/user-list-contactfolders.md) | [ContactFolder](contactfolder.md) 集合 | 获取已登录用户的默认联系人文件夹中的联系人文件夹集合。 |
| **目录对象**|||
| [activateServicePlan](../api/user-activateserviceplan.md) | 无 | 为给定给定用户或`servicePlanId``skuId`许可证和[服务](user.md)。 |
| [assignLicense](../api/user-assignlicense.md) | [user](user.md) | 为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。 |
| [checkMemberGroups](../api/user-checkmembergroups.md) | String collection | 检查组列表中的成员身份。检查是可传递的。 |
| [checkMemberObjects](../api/user-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。检查是可传输的。 |
| [exportPersonalData](../api/user-exportpersonaldata.md) | 无 | 提交公司管理员发出的数据策略操作请求，以导出组织用户的数据。 |
| [getByIds](../api/directoryobject-getbyids.md) | String collection | 返回 ID 列表中指定的目录对象。 |
| [getMemberGroups](../api/user-getmembergroups.md) | String collection | 返回用户是其成员的所有组。检查是可传递的。 |
| [getMemberObjects](../api/user-getmemberobjects.md) | String 集合 | 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。 |
| [Get transitiveReports](../api/user-get-transitivereports.md) | 整数 | 从 transitiveReports 导航属性获取用户的可传递报表计数。 |
| [List createdObjects](../api/user-list-createdobjects.md) | [directoryObject](directoryobject.md) collection | 从 createdObjects 导航属性中获取此用户创建的目录对象。 |
| [List licenseDetails](../api/user-list-licensedetails.md) | [licenseDetails](licensedetails.md) 集合 | 获取 licenseDetails 对象集合。 |
| [List ownedDevices](../api/user-list-owneddevices.md) | [directoryObject](directoryobject.md) collection | 从 ownedDevices 导航属性中获取此用户所拥有的设备。 |
| [List ownedObjects](../api/user-list-ownedobjects.md) | [directoryObject](directoryobject.md) collection | 从 ownedObjects 导航属性中获取此用户所拥有的目录对象。 |
| [List registeredDevices](../api/user-list-registereddevices.md) | [directoryObject](directoryobject.md) 集合 | 从 registeredDevices 导航属性中获取为此用户注册的设备。 |
| [List scoped-role memberships](../api/user-list-scopedrolememberof.md) | [scopedRoleMembership](scopedrolemembership.md) 集合 | 获取此用户的作用域角色管理单元成员身份。 |
| [列表 usageRights](../api/user-list-usagerights.md) | [usageRight](usageright.md) 集合 | 获取已授予用户的使用权限集合。 |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md) | [user](user.md) | 重新处理用户的订阅分配。 |
| [revokeSignInSessions](../api/user-revokesigninsessions.md) | 无 | 通过将 **signInSessionsValidFromDateTime** 用户属性重置为当前的日期时间来吊销向应用程序发出的用户的所有刷新和会话令牌。 这将强制用户再次登录到这些应用程序。 此方法将替换 **invalidateAllRefreshTokens**。 |
| **Drive** |||
| [获取驱动器](../api/drive-get.md) | [drive](drive.md) | 检索 Drive 资源的属性和关系。 |
| [列出子项](../api/driveitem-list-children.md) | [DriveItems](driveitem.md) | 在 DriveItem 的子项关系中返回 DriveItems 集合。 |
| **组** |||
| [List joinedTeams](../api/user-list-joinedteams.md) | [团队](team.md) 集合 | 从 joinedTeams 导航属性中获取此用户直接所属的 Microsoft Teams 团队。 |
| [List memberOf](../api/user-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 从 memberOf 导航属性中获取此用户直接所属的组、目录角色和管理单元。 |
| [List transitive memberOf](../api/user-list-transitivememberof.md) | [directoryObject](directoryobject.md) 集合 | 列出用户所属的所有组、目录角色和管理单元。 此操作是可传递的，并包括用户以嵌套方式所属的组。 |
| **见解** |||
| [共享的列表](../api/insights-list-shared.md) | [sharedInsight](insights-shared.md) 集合 | 计算得出的见解，可返回与用户共享的文件列表。 |
| [列出趋势](../api/insights-list-trending.md) | [trending](insights-trending.md) 集合 | 计算得出的见解，可返回用户常用的项目列表。 |
| [使用的列表](../api/insights-list-used.md) | [usedInsight](insights-used.md) 集合 | 计算得出的见解，可返回用户使用的文件列表。 |
| **邮件** |||
| [创建 inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | 无 | 创建由 SMTP 地址识别的发件人的重点收件箱替代。 |
| [Create mailFolder](../api/user-post-mailfolders.md) | [mailFolder](mailfolder.md) | 通过发布到 mailFolders 集合创建新 mailFolder |
| [创建邮件](../api/user-post-messages.md) | [message](message.md) | 通过发布到邮件集合创建邮件。 |
| [创建 messageRule](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) | 通过指定一组条件和操作来创建 messageRule 对象。 |
| [getMailTips](../api/user-getmailtips.md) | [邮件提醒](mailtips.md)集合 | 返回向已登录用户提供的一个或多个收件人的邮件提醒。 |
| [List mailFolders](../api/user-list-mailfolders.md) | [mailFolder](mailfolder.md) 集合 | 在已登录用户的根文件夹下获取邮件文件夹集合。 |
| [列出邮件](../api/user-list-messages.md) | [message](message.md) 集合 | 获取已登录用户的邮箱中的所有邮件。 |
| [列出替代](../api/inferenceclassification-list-overrides.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) 集合 | 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的重点收件箱替代。 |
| [List rules](../api/mailfolder-list-messagerules.md) | [messageRule](messagerule.md) 集合 | 获取为用户收件箱定义的所有 messageRule 对象。 |
| [发送邮件](../api/user-sendmail.md) | 无 | 发送请求正文中指定的邮件。 |
| **备注** |||
| [创建笔记本](../api/onenote-post-notebooks.md) | [笔记本](notebook.md) | 新建 OneNote 笔记本。 |
| [列出笔记本](../api/onenote-list-notebooks.md) | [notebook](notebook.md) 集合 | 检索 notebook 对象列表。 |
| **开放扩展** |||
| [创建开放扩展](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | 创建开放扩展，并将自定义属性添加到新资源或现有资源。 |
| [获取开放扩展](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) 集合 | 获取扩展名称标识的开放扩展。 |
| **组织层次结构** |||
| [分配经理](../api/user-post-manager.md) | 无 | 分配用户的经理。 |
| [获取经理](../api/user-list-manager.md) | [directoryObject](directoryobject.md) | 从 manager 导航属性中获取是此用户的经理的用户或联系人。 |
| [List directReports](../api/user-list-directreports.md) | [directoryObject](directoryobject.md) collection | 从 directReports 导航属性中获取向此用户报告的用户和联系人。 |
| **Outlook 设置** |||
| [创建 Outlook 类别](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) | 在用户主类别列表中创建 outlookCategory 对象。 |
| [获取 supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) 集合 | 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。 |
| [获取 supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md collection) | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。 |
| [获取用户的邮箱设置](../api/user-get-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | 获取用户的 mailboxSettings。 |
| [列出 Outlook 类别](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) 集合                                 | 获取为用户定义的所有类别。 |
| [转换 Exchange ID](../api/user-translateexchangeids.md) | [convertIdResult](convertidresult.md) 集合 | 对与 Outlook 相关的资源的标识符进行格式转换。 |
| [更新用户邮箱设置](../api/user-update-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | 启用、配置或禁用一个或多个用户的 mailboxSettings。 |
| **人员** |||
| [列出人员](../api/user-list-people.md) | [person](person.md) | 检索 person 对象列表，这些对象按与 user 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。 |
| **照片** |||
| [获取照片](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) | 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。 |
| [更新 profilephoto](../api/profilephoto-update.md) | 无 | 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 |
| **Planner** |||
| [获取 plannerUser](../api/planneruser-get.md) | [plannerUser](planneruser.md) | 检索 plannerUser 对象的属性和关系。 |
| [列出 favoritePlans](../api/planneruser-list-favoriteplans.md) | [plannerPlan](plannerplan.md) 集合 | 检索由用户标记为收藏的 plannerPlans 列表。 |
| [列出 recentPlans](../api/planneruser-list-recentplans.md) | [plannerPlan](plannerplan.md) 集合 | 检索用户最近查看的 plannerPlans 列表。 |
| [List tasks](../api/planneruser-list-tasks.md) | [plannerTask](plannertask.md) 集合 | 获取分配给此用户的 plannerTasks。|
| [更新 plannerUser](../api/planneruser-update.md) | 无 | 更新 plannerUser 对象的属性。 |
| **个人资料** |||
| [获取个人资料](../api/profile-get.md) | [profile](profile.md) | 检索给定用户的 profile 对象的属性和关系。 |
| [删除个人资料](../api/profile-delete.md) | 无 | 从用户帐户中删除 profile 对象。 |
| **架构扩展** |||
| [添加架构扩展值](/graph/extensibility-schema-groups) | 无 | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。 |
| **Teamwork** |||
|[列出为用户安装的应用](../api/userteamwork-list-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合 | 列出安装在用户个人范围内的应用。|
|[获取为用户安装的应用](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | 列出安装在用户个人范围内的指定应用。 |
|[为用户添加应用](../api/userteamwork-post-installedapps.md) | 无 | 在用户的个人范围内添加（安装）应用。|
|[为用户删除应用](../api/userteamwork-delete-installedapps.md) | 无 | 删除（卸载）用户个人范围内的应用。|
|[升级为用户安装的应用](../api/userteamwork-teamsappinstallation-upgrade.md) | 无 | 将安装在用户个人范围内的应用升级到最新版本。|
|[获取用户和应用之间的聊天](../api/userscopeteamsappinstallation-get-chat.md)| [聊天](chat.md)| 列出用户和应用之间的一对一聊天。 |
| **待办任务** |||
|[创建任务](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| 在指定的任务列表中创建 [todoTask](todotask.md)。|
|[创建任务列表](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | 在用户的邮箱中创建微软待办任务列表。 |
|[列出任务](../api/todotasklist-list-tasks.md)|[todoTask](todotask.md) 集合|获取指定列表中的所有 [todoTask](todotask.md) 资源。|
|[列出任务列表](../api/todo-list-lists.md) | [todoTaskList](todotasklist.md) 集合 | 获取用户邮箱中的所有任务列表。 |
| **用户设置** |||
| [获取设置](../api/usersettings-get.md) | [userSettings](usersettings.md) | 阅读用户和组织设置对象。 |
| [更新设置](../api/usersettings-update.md) | [userSettings](usersettings.md) | 更新 settings 对象的属性。 |
| **Outlook 任务**（已弃用）|||
| [创建 outlookTask](../api/outlookuser-post-tasks.md)（已弃用） | [outlookTask](outlooktask.md) | 在用户邮箱的默认任务组（“我的任务”）和默认任务文件夹（“任务”）中创建 Outlook 任务。 |
| [列出任务](../api/outlookuser-list-tasks.md)（已弃用） | [outlookTask](outlooktask.md) 集合 | 获取用户邮箱中的所有 Outlook 任务。 |


## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

| 属性       | 类型    | 说明 |
|:---------------|:--------|:------------|
| aboutMe | String | 任意形式的文本输入字段，用于介绍用户自身。 <br><br>仅在 `$select` 上返回。 |
| accountEnabled | Boolean | 启用帐户时为 `true`，否则为 `false`。 创建用户时此属性是必需的。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`和 `in`）。 |
| ageGroup | [ageGroup](#agegroup-values) | 设置用户的年龄组。 允许的值：`null`、`minor`、`notAdult` 和 `adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`和 `in`）。 |
| assignedLicenses | [assignedLicense](assignedlicense.md) collection | 已分配给用户的许可证，包括继承的（基于组的）许可证。 <br><br>不可为 null。 支持 `$filter`（`eq` 和 `NOT`）。 |
| assignedPlans | [assignedPlan](assignedplan.md) collection | 分配给该用户的计划。只读。不可为 null。<br><br>支持 `$filter`（`eq` 和 `NOT`）。 |
| birthday | DateTimeOffset | 用户的生日。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z` <br><br>仅在 `$select` 上返回。 |
| businessPhones | String collection | 用户的电话号码。仅可以为此属性设置一个数字。<br><br>对于从本地目录同步的用户而言为只读。 支持 `$filter`（`eq` 和 `NOT`）。|
| 城市 | String | 用户所在的城市。最大长度为 128 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| companyName | String | 与用户关联的公司名称。 此属性可用于描述外部用户所属的公司。 公司名称的最大长度为 64 个字符。<br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| consentProvidedForMinor | [consentProvidedForMinor](#consentprovidedforminor-values) | 设置是否已获得未成年人的同意。 允许的值：`null`、`granted`、`denied` 和 `notRequired`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`和 `in`）。|
| country | String | 用户所在的国家/地区;例如， `US` 或 `UK`。 最大长度为 128 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| createdDateTime | DateTimeOffset | 创建用户的日期和时间。 值无法修改，并在实体创建时自动填充。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 属性可为 Null。 Null 值表示无法为用户确定准确的创建时间。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`和 `in` 运算符）。 |
| creationType | 字符串 | 指示是否通过以下方法之一创建用户帐户： <br/> <ul><li>作为常规学校或工作帐户（`null`）。 <li>作为外部帐户（`Invitation`）。 <li>作为 Azure Active Directory B2C 租户的本地帐户（`LocalAccount`）。 <li>通过使用电子邮件验证由内部用户（`EmailVerified`）进行自助注册。 <li>通过由外部用户通过属于用户流的链接注册的自助注册（`SelfServiceSignUp`）。 </ul> <br>只读。<br>支持 `$filter` （`eq`、 `ne`、 `NOT`和 `in`）。 |
| deletedDateTime | DateTimeOffset | 删除用户的日期和时间。 <br><br>支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le` 和 `in`）。 |
| 部门 | String | 用户工作部门的名称。 最大长度为 64 个字符。<br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`和 `in` 运算符）。 |
| displayName | String | 用户通讯簿中显示的名称。通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。最大长度为 256 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`、 `$orderBy`和 `$search`。|
| employeeHireDate | DateTimeOffset | 聘请用户或用户将开始工作（如是未来招聘）的日期和时间。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`）。|
| employeeId | String | 由组织分配给该用户的员工标识符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`）。|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |表示与用户相关联的组织数据（例如，分部和 costCenter）。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`）。|
| employeeType | String | 捕获企业员工类型。 例如，`Employee`、`Contractor`、`Consultant` 或 `Vendor`。 支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`）。|
| externalUserState | String | 对于使用[邀请 API](../api/invitation-post.md) 邀请到租户的外部用户，此属性表示受邀用户的邀请状态。 对于受邀用户，状态可以是 `PendingAcceptance` 或 `Accepted`，而对于所有其他用户，状态为 `null`。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `in`）。 |
| externalUserStateChangeDateTime | String | 显示对 externalUserState 属性的最新更改的时间戳。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `in`）。 |
| faxNumber | String | 用户的传真号。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| givenName | String | 用户的名。 最大长度为 64 个字符。 支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`）。|
| hireDate | DateTimeOffset | 用户的雇佣日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br> 仅在 `$select` 上返回。 <br> **注意：** 此属性特定于 SharePoint Online。 建议使用本地 **employeeHireDate** 属性来设置和更新使用 Microsoft Graph API 的聘用日期值。 |
| id | String | 用户的唯一标识符。 应视为不透明的标识符。 继承自 [directoryObject](directoryobject.md)。 不可为空。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。 |
| identities | [objectIdentity](objectIdentity.md) 集合 | 表示可用于登录此用户帐户的标识。 标识可由 Microsoft （也称为本地帐户）、组织或社交身份提供商（如 Facebook、Google 和 Microsoft）提供，并绑定到用户帐户。 可能包含具有相同 **signInType** 值的多个项目。 <br><br>仅在 **signInType** 不是 `userPrincipalName` 才支持 `$filter` （`eq`） 。 |
| imAddresses | String collection | 用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。 只读。 支持 `$filter` （`eq`、 `NOT`、 `ge`、 `le`、 `startsWith`）。|
| infoCatalogs | 字符串集合 | 标识分配给用户的信息片段。  支持 `$filter` （`eq`、 `NOT`、 `ge`、 `le`、 `startsWith`）。 |
| interests | String collection | 用户介绍自身兴趣的列表。 <br><br>仅在 `$select` 上返回。 |
| isResourceAccount | 布尔 | 请勿使用 – 保留以备今后使用。 |
| jobTitle | String | 用户的职务。 最大长度为 128 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT` 、 `ge`、 `le`、 `in`、 `startsWith`）。|
| lastPasswordChangeDateTime | DateTimeOffset | 此 Azure AD 用户上次更改其密码的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 <br><br>仅在 `$select` 上返回。  |
| legalAgeGroupClassification | [legalAgeGroupClassification](#legalagegroupclassification-values) | 由企业应用程序用于确定用户的法定年龄组。 此属性为只读，并且基于 **ageGroup** 和 **consentProvidedForMinor** 属性进行计算。 允许的值：`null`、`minorWithOutParentalConsent`、`minorWithParentalConsent`、`minorNoParentalConsentRequired`、`notAdult` 和 `adult`。 请参阅[法定年龄组属性定义](#legal-age-group-property-definitions)以了解详细信息。 <br><br>仅在 `$select` 上返回。 |
| licenseAssignmentStates | [licenseAssignmentState](licenseassignmentstate.md) 集合 | 此用户的许可证分配状态。只读。<br><br>仅在 `$select` 上返回。 |
| mail | String | 用户的 SMTP 地址，例如， `admin@contoso.com`。 对此属性进行更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。 对于 Azure AD B2C 帐户，此属性最多可以使用唯一的 SMTP 地址更新 10 次。 此属性不能包含突出字符。 <br><br> 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`、 `endsWith`）。 |
| mailboxSettings | [mailboxSettings](mailboxsettings.md) | 已登录用户的主邮箱的设置。可以[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。 <br><br>仅在 `$select` 上返回。 |
| mailNickname | String | 用户的邮件别名。创建用户时必须指定此属性。最大长度为 64 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| mobilePhone | String | 用户的主要移动电话号码。 本地目录同步的用户为只读。 <br><br> 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| mySite | String | 用户个人网站的 URL。 <br><br>仅在 `$select` 上返回。 |
| officeLocation | String | 用户公司地点的办公室位置。 最大长度为 128 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| onPremisesDistinguishedName | String | 包含本地 Active Directory `distinguished name` 或 `DN`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。  |
| onPremisesDomainName | String | 包含从本地目录同步的本地 `domainFQDN`（也称为 dnsDomainName）。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 |
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | 包含用户的 extensionAttributes 1-15。 请注意，单个扩展属性既不可选择，也不可筛选。 对于 `onPremisesSyncEnabled` 用户，这组属性集的授权来源是本地，并且为只读。 对于只使用云的用户（其中 `onPremisesSyncEnabled` 为假），可以在创建或更新期间设置这些属性。 这些扩展属性也称 Exchange 自定义属性 1-15。 <br><br>支持 `$filter` （`eq`、 `NOT`、 `ge`、 `le`、 `in`）。  |
| onPremisesImmutableId | String | 此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。 如果对用户的 `userPrincipalName` (UPN) 属性使用联盟域，必须在 Graph 中创建新用户帐户时指定此属性。 **注意：** 指定此属性时，不能使用 **$** 和 **\_** 字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`）。 |
| onPremisesLastSyncDateTime | DateTimeOffset | 表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`）。 |
| onPremisesProvisioningErrors | [onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合 | 在预配期间使用 Microsoft 同步产品时发生的错误。 <br> 支持 `$filter`（`eq`、`NOT`、`ge`、`le`）。|
| onPremisesSamAccountName | String | 包含从本地目录同步的本地 `sAMAccountName`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。<br><br> 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| onPremisesSecurityIdentifier | String | 包含从本地同步到云的用户的本地安全标识符 (SID)。只读。 |
| onPremisesSyncEnabled | Boolean | 如果此对象从本地目录同步，则为 `true`；如果此对象最初从本地目录同步，但以后不再同步，则为 `false`；如果此对象从未从本地目录同步，则为 `null`（默认值）。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。 |
| onPremisesUserPrincipalName | String | 包含从本地目录同步的本地 `userPrincipalName`。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| otherMails | 字符串集合 | 用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。<br>注意：此属性不能包含突出字符。<br><br>支持 `$filter` （`eq`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| passwordPolicies | String | 指定用户的密码策略。 此值表示枚举，其中一个可能 `DisableStrongPassword`为枚举值，允许指定超过默认策略的密码。 `DisablePasswordExpiration` 也可以指定 。 可同时指定两者;例如： `DisablePasswordExpiration, DisableStrongPassword`。 有关默认密码策略的详细信息，请参阅 [Azure AD pasword 策略](/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)。 <br><br>支持 `$filter`（`ne`、`NOT`）。|
| passwordProfile | [passwordProfile](passwordprofile.md) | 指定用户的密码配置文件。 配置文件包含用户的密码。 创建用户时此属性是必需的。 配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。 默认情况下，必须使用强密码。 **注意：** 对于 Azure B2C 租户， **forceChangePasswordNextSignIn** 属性应设置为 `false` ，并且应在第一次登录时使用自定义策略和用户流强制重置密码。 请参阅 [首次登录时强制重置](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon)。 <br><br>支持 `$filter`（`eq`、`ne`、`NOT`、`in`）。|
| pastProjects | String collection | 供用户枚举其过去项目的列表。 <br><br>仅在 `$select` 上返回。 |
| postalCode | String | 用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。最大长度为 40 个字符。<br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| preferredDataLocation | String | 用户的首选数据位置。 有关详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。|
| preferredLanguage | String | 用户的首选语言。 应遵循 ISO 639-1 代码;例如， `en-US`。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| preferredName | String | 用户的首选名称。 <br><br>仅在 `$select` 上返回。 |
| provisionedPlans | [provisionedPlan](provisionedplan.md) 集合 | 为用户设置的计划。 只读。 不可为 null。 支持 `$filter`（`eq`、`NOT`、`ge`、`le`）。|
| proxyAddresses | String collection | 例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`。  对于 Azure AD B2C 帐户，此属性有 10 个唯一地址的限制。 只读，不可为 Null。 <br><br>支持 `$filter` （`eq`、 `NOT`、 `ge`、 `le`、 `startsWith`）。 |
| refreshTokensValidFromDateTime | DateTimeOffset | 在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 只读。 使用 [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) 进行重置。|
| responsibilities | String collection | 供用户枚举其职责的列表。 <br><br>仅在 `$select` 上返回。 |
| schools | String collection | 供用户枚举其学习过的学校列表。 <br><br>仅在 `$select` 上返回。 |
| showInAddressList | Boolean | 如果 Outlook 全局地址列表应包含此用户，则值为 `true`，否则为 `false`。 如果未设置，则将其视为 `true`。 对于通过邀请管理器邀请的用户，此属性将设置为 `false`。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。 |
| signInSessionsValidFromDateTime | DateTimeOffset | 在此时间之前发出的任何刷新令牌或会话令牌（会话 Cookie）都是无效的，并且当使用无效的刷新令牌或会话令牌获取委托的访问令牌（用于访问 Microsoft Graph 等 API）时，应用程序将收到错误。  如果发生这种情况，应用程序将需要通过向授权端点发出请求来获取新的刷新令牌。 只读。 使用 [revokeSignInSessions](../api/user-revokesigninsessions.md) 进行重置。|
| skills | String collection | 供用户枚举其技能的列表。 <br><br>仅在 `$select` 上返回。 |
| signInActivity | [signInActivity](signinactivity.md) | 获取指定用户登录的最后一个登录日期和请求 ID。只读。<br><br>仅在 `$select` 上返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`） *但是*，不支持任何其他的可筛选属性。 **注意：** 此属性的详细信息需要 Azure AD Premium P1/P2 许可证和 **AuditLog.Read.All** 权限。|
| state | String | 用户地址中的省/市/自治区或省。 最大长度为 128 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| streetAddress | String | 用户公司地点的街道地址。 最大长度为 1024 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| surname | String | 用户的姓氏。 最大长度为 64 个字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
| usageLocation | String | 两个字母的国家/地区代码（ISO 标准 3166）。 为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。  示例包括： `US`、 `JP`和 `GB`。 不可为 null。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
| userPrincipalName | String | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中 domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。<br>注意：此属性不能包含突出字符。 <br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`、 `endsWith`） 和 `$orderBy`。
| userType | String | 可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。 <br><br>支持 `$filter`（`eq`、`ne`、`NOT`、`in`）。 |

### <a name="legal-age-group-property-definitions"></a>法定年龄组属性定义

本部分介绍 Azure AD 管理员和企业应用程序开发人员如何使用三个年龄组属性（**legalAgeGroupClassification**、**ageGroup** 和 **consentProvidedForMinor**）来满足与年龄相关的法规：
- **legalAgeGroupClassification** 属性为只读属性。 企业应用程序开发人员使用此只读属性来确保根据用户的法定年龄组正确处理用户。 此属性是基于用户的 **ageGroup** 和 **consentProvidedForMinor** 属性计算得出的。
- **ageGroup** 和 **consentProvidedForMinor** 属性是 Azure AD 管理员使用的可选属性，可帮助确保根据用户所在国家或地区与年龄相关的监管规则正确处理帐户的使用。

例如：Cameron 是英国 Holyport 小学的名录管理员。 新学年开始，他根据英国与年龄相关的法规，使用入学文件获得未成年人父母的同意。 征得父母同意后，Holyport 学校和 Microsoft 应用可以使用未成年人的帐户。 Cameron 随后创建所有帐户，将 ageGroup 设置为“minor”，并将 consentProvidedForMinor 设置为“granted”。 然后，他的学生使用的应用程序可以禁止不适合未成年人的功能。
<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience.
For some reason they are not defined as enums in the CSDL.
Hence the type of the corresponding 3 properties remain as string type in the Properties table.
-->

#### <a name="legalagegroupclassification-values"></a>legalAgeGroupClassification values

| 成员    | 说明|
|:---------------|:----------|
|空|默认值，尚未给用户设置 **ageGroup**。|
|minorWithoutParentalConsent |（保留以备今后使用）|
|minorWithParentalConsent| 根据用户所在国家或地区与年龄相关的法规，将用户视为未成年人，并且帐户管理员已相应获得父母或监护人的同意。|
|adult|根据用户所在国家或地区与年龄相关的法规，将用户视为成年人。|
|notAdult|用户所在国家或地区存在其他与年龄相关的法规（例如美国、英国、欧盟和韩国），用户的年龄介于未成年人和成年人之间（根据所在国家或地区的规定）。 通常，这意味着会在管控的国家或地区将青少年视为 `notAdult`。|
|minorNoParentalConsentRequired|用户是未成年人，但所在国家或地区没有与年龄相关的法规。|

#### <a name="agegroup-values"></a>ageGroup 值

| 成员    | 说明|
|:---------------|:--------|
|空|默认值，尚未给用户设置 **ageGroup**。|
|未成年人|该用户被视为未成年人。|
|notAdult|用户所在国家或地区存在相关法规（例如美国、英国、欧盟或韩国），而且用户年龄超过儿童年龄上限（根据所在国家或地区的规定）且低于成年人年龄下限（根据所在国家或地区的规定）。 因此，基本上会在管控的国家或地区将青少年视为 `notAdult`。|
|adult|应将用户视为成年人。|

#### <a name="consentprovidedforminor-values"></a>consentProvidedForMinor 值

| 成员    | 说明|
|:---------------|:----------|
|空|默认值，尚未给用户设置 **consentProvidedForMinor**。|
|granted|已就用户拥有帐户获得同意。|
|denied|尚未就用户拥有帐户获得同意。|
|notRequired|用户所在地不要求获得同意。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md) 集合| 用户的使用条款接受状态。只读。可以为 null。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|表示已向应用程序授予用户的应用角色。 支持 `$expand`。 |
|日历|[calendar](calendar.md)|用户的主日历。只读。|
|calendarGroups|[CalendarGroup](calendargroup.md) 集合|用户的日历组。只读。可为 Null。|
|calendarView|[event](event.md) 集合|日历的日历视图。只读。可为 Null。|
|calendars|[calendar](calendar.md) 集合|用户的日历。只读。可为 Null。|
|contactFolders|[ContactFolder](contactfolder.md) 集合|用户的联系人文件夹。只读。可为 Null。|
|contacts|[contact](contact.md) 集合|用户的联系人。只读。可为 Null。|
|createdObjects|[directoryObject](directoryobject.md) collection|由用户创建的 directory 对象。只读。可为 Null。|
|directReports|[directoryObject](directoryobject.md) collection|向该用户报告的用户和联系人。 （将其经理属性设置为此用户的用户和联系人。）只读。 可为空。 支持 `$expand`。 |
|驱动器|[drive](drive.md)|用户的 OneDrive。只读。|
|drives|[drive](drive.md) 集合| 该用户的可用驱动器集合。只读。 |
|events|[event](event.md) 集合|用户的事件。 默认是在默认日历下显示事件。 只读。 可为空。|
|extensions|[扩展](extension.md)集合|为用户定义的开放扩展集合。可为空。|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| 基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。 |
|insights|[itemInsights](iteminsights.md) | 只读。可为 Null。|
|joinedGroups|[group](group.md) 集合| 只读。可为 Null。|
|mailFolders|[mailFolder](mailfolder.md) 集合| 用户的邮件文件夹。只读。可为 Null。|
|manager|[directoryObject](directoryobject.md)|是此用户的经理的用户或联系人。 只读。 （HTTP 方法：GET、PUT、DELETE） 支持 `$expand`。|
|memberOf|[directoryObject](directoryobject.md) 集合|用户所属的所有组、目录角色和管理单元。 只读。 可为 NULL。 支持 `$expand`。 |
|joinedTeams|[团队](team.md) 集合|用户是成员的 Microsoft Teams 团队。只读。空。|
|messages|[message](message.md) 集合|邮箱或文件夹中的邮件。只读。可为 Null。|
|onenote|[onenote](onenote.md)| 只读。|
|outlook|[outlookUser](outlookuser.md)| 用户可以选择性 Outlook 服务。只读。空。|
|ownedDevices|[directoryObject](directoryobject.md) collection|用户拥有的设备。 只读。 可为 NULL。 支持 `$expand`。|
|ownedObjects|[directoryObject](directoryobject.md) collection|用户拥有的 directory 对象。 只读。 可为 NULL。 支持 `$expand`。|
|pendingAccessReviewInstances|[accessReviewInstance](accessreviewinstance.md) | 用于获取等待审阅者批准的访问审阅列表的导航属性。 |
|people|[person](person.md) 集合| 只读。与用户最相关的人员。该集合按其与用户的相关性排序，相关性由用户的通信、协作和业务关系决定。人脉是邮件、联系人和社交网络中的信息聚合。|
|photo|[profilePhoto](profilephoto.md)| 用户的个人资料照片。只读。|
|photos|[photo](photo.md) 集合| 只读。可为 Null。|
|planner|[plannerUser](planneruser.md)| 用户可以使用的选择性计划程序服务。 只读。 可为空。 |
|个人资料 |[个人资料](profile.md) | 表示在租户中描述用户的属性。 |
|registeredDevices|[directoryObject](directoryobject.md) collection|已注册的用户的设备。只读。可为空。支持 `$expand`。|
|scopedRoleMemberOf|[scopedRoleMembership](scopedrolemembership.md) 集合| 此用户的作用域角色管理单位成员身份。 只读。 可为空。|
|settings|[userSettings](usersettings.md) | 只读。可为 Null。|
|团队合作|[userTeamwork](userteamwork.md)| 用户可以使用的Microsoft Teams功能的容器。 只读。 可为空。|
|todo|[todo](todo.md)|表示用户可以使用的微软待办服务。 |
|transitiveReports|[directoryObject](directoryobject.md) 集合 | 用户的可传递报告。只读。|
|usageRight|[usageRight](usageright.md) 集合|表示已授予用户的使用权限。 |

### <a name="user-preferences-for-languages-and-regional-formats"></a>语言和区域格式的用户首选项
**用户** 资源包含 [mailboxSettings](../resources/mailboxsettings.md)属性，其中包括用户的首选语言、数据和时间格式、默认时区以及其他专用于主要 Exchange 邮箱的设置。 这些首选项针对邮件客户端，且仅在用户已预配邮箱的情况下可用。 如果你的应用场景专注于 Outlook 邮件、日历、联系人或待办任务，可选择使用 **mailboxSettings**。

除了 **mailboxSettings**，**用户** 还包括通过 [userSettings](../resources/usersettings.md) 到 [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) 的关系，这是语言和区域格式设置首选项的超集，任何应用程序都可以使用它来向用户提供最佳的语言和区域格式设置体验。 使用 **userSettings** 以获得跨应用的一致体验，这些应用会接入 Azure AD 用户配置文件，以反映相同的用户首选项。

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
    "drives",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "teamwork",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "profile",
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
  "createdDateTime": "2019-02-07T21:53:13.067Z",
  "creationType": "string",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "string",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "faxNumber": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
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
  "otherMails": ["string"],
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "refreshTokensValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "responsibilities": ["string"],
  "schools": ["string"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",
  "calendar": {"@odata.type": "microsoft.graph.calendar"},
  "calendarGroups": [{"@odata.type": "microsoft.graph.calendarGroup"}],
  "calendarView": [{"@odata.type": "microsoft.graph.event"}],
  "calendars": [{"@odata.type": "microsoft.graph.calendar"}],
  "contacts": [{"@odata.type": "microsoft.graph.contact"}],
  "contactFolders": [{"@odata.type": "microsoft.graph.contactFolder"}],
  "createdObjects": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directReports": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "drive": {"@odata.type": "microsoft.graph.drive"},
  "drives": [{"@odata.type": "microsoft.graph.drive"}],
  "insights": {"@odata.type": "microsoft.graph.itemInsights"},
  "settings": {"@odata.type": "microsoft.graph.userSettings"},
  "events": [{"@odata.type": "microsoft.graph.event"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "inferenceClassification": {"@odata.type": "microsoft.graph.inferenceClassification"},
  "mailFolders": [{"@odata.type": "microsoft.graph.mailFolder"}],
  "manager": {"@odata.type": "microsoft.graph.directoryObject"},
  "memberOf": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "joinedTeams": [{"@odata.type": "microsoft.graph.group"}],
  "teamwork": {"@odata.type": "microsoft.graph.teamwork"},
  "messages": [{ "@odata.type": "microsoft.graph.message"}],
  "outlook": {"@odata.type": "microsoft.graph.outlookUser"},
  "ownedDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "photo": {"@odata.type": "microsoft.graph.profilePhoto"},
  "profile": {"@odata.type": "microsoft.graph.profile"},
  "registeredDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "signInActivity": {"@odata.type": "microsoft.graph.signInActivity"}
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
