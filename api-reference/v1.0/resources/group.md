---
title: 组资源类型
description: '表示 Azure Active Directory (Azure AD) 组，可以是 Microsoft 365 组或安全组。 '
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5176d58c15530883f5bdabcbbd0325846b042382
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366483"
---
# <a name="group-resource-type"></a>组资源类型

命名空间：microsoft.graph

表示 Azure Active Directory (Azure AD) 组，可以是 Microsoft 365 组或安全组。

继承自 [directoryObject](directoryobject.md)。

出于性能原因，默认情况下 [create](../api/group-post-groups.md)、[get](../api/group-get.md) 和 [list](../api/group-list.md) 操作仅返回更常用属性的子集。 这些 _默认_ 属性将记录在 [属性](#properties)部分中。 若要获取非默认返回的任一属性，请在 `$select` OData 查询选项中指定这些属性。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。


## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:------ |:----------- |:----------- |
| **组管理** |||
| [Create group](../api/group-post-groups.md) | [组](group.md) | 创建新组。它可以是 Microsoft 365 组、动态组或安全组。 |
| [Get group](../api/group-get.md) | [组](group.md) | 读取 group 对象的属性。 |
| [列出组](../api/group-list.md) | [组](group.md) 集合 | 列出 group 对象及其属性。 |
| [更新组](../api/group-update.md) | 无 | 更新 group 对象的属性。 |
| [删除组](../api/group-delete.md) | 无 | 删除组对象。 |
| [增量](../api/group-delta.md) | 组集合 | 获取组的增量更改。 |
| [添加成员](../api/group-post-members.md) | 无 | 通过发布到 **members** 导航属性将用户或组添加到此组（仅支持安全组和启用邮件的安全组新）。 |
| [添加所有者](../api/group-post-owners.md) | 无 | 通过发布到 **owners** 导航属性，为此组添加新所有者（仅支持为安全组和启用邮件的安全组添加）。 |
| [Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) | 基于 groupSettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。只有组特定模板可用于此操作。 |
| [删除设置](../api/groupsetting-delete.md) | 无 | 删除 setting 对象。 |
| [Get setting](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
| [列出 groupLifecyclePolicy](../api/group-list-grouplifecyclepolicies.md)  | [groupLifecyclePolicy](grouplifecyclepolicy.md) 集合 | 列出组生命周期策略。 |
| [List members](../api/group-list-members.md) | [directoryObject](directoryobject.md) 集合 | 从 **members** 导航属性中获取属于此组的直接成员的用户和组。 |
| [List owners](../api/group-list-owners.md) | [directoryObject](directoryobject.md) 集合 | 从 **owners** 导航属性中获取此组的所有者。 |
| [List settings](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
| [List transitive members](../api/group-list-transitivemembers.md) | [directoryObject](directoryobject.md) 集合 | 获取属于此组成员（包括嵌套成员）的用户、组和设备。 |
| [List transitive memberOf](../api/group-list-transitivememberof.md) | [directoryObject](directoryobject.md) 集合 | 列出此组所属的组。 此操作是可传递的，并包括此组以嵌套方式所属的组。 |
| [删除成员](../api/group-delete-members.md) | 无 | 通过 **members** 导航属性删除 Microsoft 365 组、安全组，或这启用邮的安全组中的成员。您可以删除用户或其他组。 |
| [删除所有者](../api/group-delete-owners.md) | 无 | 通过 **owners** 导航属性，删除 Microsoft 365 组、安全组或启用邮件安全组的所有者。 |
| [Update setting](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 更新 setting 对象。 |
| [assignLicense](../api/group-assignlicense.md) | [组](group.md) | 为群组添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。 |
| [checkMemberGroups](../api/group-checkmembergroups.md) | String collection | 在一列组中检查此组的成员身份。此函数是可传递的。 |
| [checkMemberObjects](../api/group-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。该函数可传递。 |
| [getMemberGroups](../api/group-getmembergroups.md) | String collection | 返回此组是其成员的所有组。此函数是可传递的。 |
| [getMemberObjects](../api/group-getmemberobjects.md) | String collection | 返回此组所属的全部组。此函数可传递。 |
| [续订](../api/group-renew.md) | 布尔值 | 续订组以更新到期时间。续订后，组的有效期就会延长策略中定义的天数。 |
| [validateProperties](../api/group-validateproperties.md) | JSON | 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。 |
| **应用角色分配** |||
| [列出 appRoleAssignments](../api/group-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) 集合 | 获取已分配到此组的应用和应用角色。 |
| [添加 appRoleAssignment](../api/group-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | 向此组分配一个应用角色。 |
| [删除 appRoleAssignment](../api/group-delete-approleassignments.md) | 无。 | 从此组中删除一个应用角色分配。 |
| **Calendar** |||
| [创建事件](../api/group-post-events.md) | [event](event.md) | 通过发布到事件集合新建事件。 |
| [获取事件](../api/group-get-event.md) | [event](event.md) | 读取 event 对象的属性。 |
| [列出事件](../api/group-list-events.md) | [event](event.md) 集合 | 获取 event 对象集合。 |
| [更新事件](../api/group-update-event.md) | 无 | 更新 event 对象的属性。 |
| [删除事件](../api/group-delete-event.md) | 无 | 删除 event 对象。 |
| [列出 calendarView](../api/group-list-calendarview.md) | [event](event.md) 集合 | 获取指定时间范围内的事件集合。|
| **对话** |||
| [创建对话](../api/group-post-conversations.md) | [conversation](conversation.md) | 通过发布到对话集合新建对话。 |
| [获取对话](../api/group-get-conversation.md) | [conversation](conversation.md) | 读取 conversation 对象的属性。 |
| [列出对话](../api/group-list-conversations.md) | [conversation](conversation.md) 集合 | 获取 conversation 对象集合。 |
| [删除对话](../api/group-delete-conversation.md) | 无 | 删除 conversation 对象。 |
| [创建线程](../api/group-post-threads.md) | [conversationThread](conversationthread.md) | 创建新的对话线程。 |
| [获取线程](../api/group-get-thread.md) | [conversationThread](conversationthread.md) | 读取 thread 对象的属性。 |
| [列出线程](../api/group-list-threads.md) | [conversationThread](conversationthread.md) 集合 | 获取组的所有线程。 |
| [更新线程](../api/group-update-thread.md) | 无 | 更新 thread 对象的属性。 |
| [删除线程](../api/group-delete-thread.md) | 无 | 删除 thread 对象。 |
| [列出 acceptedSenders](../api/group-list-acceptedsenders.md) | [directoryObject](directoryobject.md) collection | 获取此组的“接受的发件人”列表中的用户或组列表。 |
| [添加 acceptedSender](../api/group-post-acceptedsenders.md) | [directoryObject](directoryobject.md) | 将用户或组添加到 acceptSenders 集合。 |
| [删除 acceptedSender](../api/group-delete-acceptedsenders.md) | [directoryObject](directoryobject.md) | 从 acceptedSenders 集合中删除用户或组。 |
| [List rejectedSenders](../api/group-list-rejectedsenders.md) | [directoryObject](directoryobject.md) collection | 获取此组的“遭拒的发件人”列表中的用户或组列表。 |
| [Add rejectedSender](../api/group-post-rejectedsenders.md)  | [directoryObject](directoryobject.md) | 将新用户或组添加到 rejectedSenders 集合中。 |
| [Remove rejectedSender](../api/group-delete-rejectedsenders.md) | [directoryObject](directoryobject.md) | 从 rejectedSenders 集合中删除新用户或组。 |
| [Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) | 基于 groupSettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。只有组特定模板可用于此操作。 |
| [获取设置](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
| [List settings](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
| [更新设置](../api/groupsetting-update.md) | 无 | 更新 setting 对象。 |
| [删除设置](../api/groupsetting-delete.md) | 无 | 删除 setting 对象。 |
| [获取设置模板](../api/groupsettingtemplate-get.md) | 无 | 读取设置模板的属性。 |
| [列出设置模板](../api/groupsettingtemplate-list.md) | 无 | 列出所有设置模板的属性。 |
| **开放扩展** |||
| [创建开放扩展](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | 创建开放扩展，并将自定义属性添加到新资源或现有资源。 |
| [获取开放扩展](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) 集合 | 获取扩展名称标识的开放扩展。 |
| **架构扩展** |||
| [添加架构扩展值](/graph/extensibility-schema-groups) | 无 | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。 |
| **其他组资源** |||
| [List photos](../api/group-list-photos.md) | [profilePhoto](photo.md) 集合 | 获取组的个人资料照片集合。 |
| [List plannerPlans](../api/plannergroup-list-plans.md) | [plannerPlan](plannerplan.md) 集合 | 获取组拥有的 Planner 计划。 |
| **用户设置** |||
| [addFavorite](../api/group-addfavorite.md) | 无 | 将组添加到登录用户的收藏夹组列表中。仅支持 Microsoft 365 组。 |
| [removeFavorite](../api/group-removefavorite.md) | 无 | 从登录用户收藏夹组列表中删除组。仅支持 Microsoft 365 组。 |
| [List memberOf](../api/group-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 通过 **memberOf** 导航属性，获取此用户为其直接成员的组和管理单元。 |
| [subscribeByMail](../api/group-subscribebymail.md) | 无 | 将 isSubscribedByMail 属性设置为 `true`。 使登录用户可以接收电子邮件对话。 仅支持 Microsoft 365 组。 |
| [unsubscribeByMail](../api/group-unsubscribebymail.md) | 无 | 将 isSubscribedByMail 属性设置为 `false`。 使登录用户无法接收电子邮件对话。 仅支持 Microsoft 365 组。 |
| [resetUnseenCount](../api/group-resetunseencount.md) | 无 | 将登录用户自上次访问后未查看的所有帖子的 unseenCount 重置为 0。仅支持 Microsoft 365 组。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean| 指明组织外部人员能否向群组发送邮件。 默认值为 `false`。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。 |
|assignedLabels|[assignedLabel](assignedlabel.md) 集合|与 Microsoft 365 组关联的敏感度标签对（标签 ID、标签名称）列表。 <br><br>仅在 `$select` 上返回。 只读。|
|assignedLicenses|[assignedLicense](assignedlicense.md) 集合|分配给该组的许可证。 <br><br>仅在 `$select` 上返回。 支持`$filter`（`eq`）。只读。|
|autoSubscribeNewMembers|布尔值|指示添加到组中的新成员是否将自动订阅接收电子邮件通知。 可以在 PATCH 请求中设置组的这个属性；不要在创建该组的初始 POST 请求中设置它。 默认值为 `false`。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。|
|classification|字符串|描述该组的分类（如低、中或高业务影响）。通过根据[模板定义](groupsettingtemplate.md)创建 ClassificationList [设置](groupsetting.md)值来定义此属性的有效值。<br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`startsWith`）。|
|createdDateTime|DateTimeOffset| 组的创建时间戳。 值无法修改，并在组创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`in`）。 只读。 |
|deletedDateTime|DateTimeOffset| 对于某些 Azure Active Directory 对象（用户、组、应用程序），如果该对象被删除，先逻辑删除，随后该属性随着对象删除的日期和时间更新。 否则此属性为`null`。 如果对象已还原，则此属性会更新为`null`。 |
|说明|String|可选的组说明。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`startsWith`）和 `$search`。|
|displayName|字符串|组的显示名称。创建组时需要此属性，更新期间无法清除此属性。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`in`、`startsWith`）、`$search` 和 `$orderBy`。 |
|expirationDateTime|DateTimeOffset| 设置的组的过期时间戳。 值无法修改，并在组创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`in`）。 只读。 |
|groupTypes|String collection| 指定组类型及其成员身份。  <br><br>如果集合中包含 `Unified`，则该组是一个 Microsoft 365 组，否则该组是一个安全组。 有关详细信息，请参阅[组概述](groups-overview.md)。<br><br>如果该集合包含 `DynamicMembership`，则该组具有动态成员身份；否则，成员身份是静态的。  <br><br>默认情况下返回。 支持 `$filter`（`eq`、`NOT`）。|
|hasMembersWithLicenseErrors|Boolean|指示此组中是否有该基于组的许可证分配中存在许可证错误的成员。 <br><br>GET 操作从未返回此属性。 可将它用作 $filter 参数，获取具有许可证错误的成员的组（也就是说，此属性的筛选器为 true）。 请参阅[示例](../api/group-list.md)。 <br><br>支持 `$filter`（`eq`）。|
|hideFromAddressLists |Boolean |如果该组未显示在 Outlook UI 的某些部分中（“**通讯簿**”中、用于选择邮件收件人的地址列表中以及用于搜索组的“**浏览组**”中），则为 true；否则为 false。 默认值为 `false`。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。|
|hideFromOutlookClients |Boolean |如果该组未显示在 Outlook 客户端（如 Outlook for Windows 和 Outlook 网页版）中，则为 true；否则为 false。 默认值为 `false`。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。|
|id|String|组的唯一标识符。 <br><br>默认情况下返回。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。<br><br>支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。|
|isAssignableToRole|Boolean|指示是否可以将此组分配给 Azure Active Directory 角色。<br><br>此属性只能在创建组时设置，并且不可变。 如果设置为 `true`，则 **securityEnabled** 属性也必须设置为 `true`，并且该组不能是动态组（即，**groupTypes** 不能包含 `DynamicMembership`）。 只有全局管理员和特权角色管理员角色中的调用方可以设置此属性。 调用方还必须分配有 *Directory.AccessAsUser.All* 权限才能设置此属性。 有关更多信息，请参阅[使用组来管理 Azure AD 角色分配](https://go.microsoft.com/fwlink/?linkid=2103037)<br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`）。|
|isSubscribedByMail|Boolean|指示登录用户是否订阅接收电子邮件对话。 默认值为 `true`。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。 |
|licenseProcessingState|String|指示对所有组成员的组许可证分配的状态。 默认值为 `false`。 只读。 可能的值是：`QueuedForProcessing`、`ProcessingInProgress` 和 `ProcessingComplete`。<br><br>仅在 `$select` 上返回。 只读。|
|mail|String|组的 SMTP 地址，例如，“serviceadmins@contoso.onmicrosoft.com”。 <br><br>默认情况下返回。 只读。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
|mailEnabled|布尔|指定是否为启用邮件的组。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`）。|
|mailNickname|String|组的邮件别名，在组织中是唯一的。 创建组时必须指定此属性。 无法在 mailNickName 中使用这些字符：`@()\[]";:.<>,SPACE`。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。|
|membershipRule|String|组为动态组时（groupTypes 包含 `DynamicMembership`），用于确定该组成员的规则。 有关成员身份规则语法的详细信息，请参阅[成员身份规则语法](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`startsWith`）。 |
|membershipRuleProcessingState|String|指示动态成员身份处理正在进行中，还是已暂停。 可能的值为 `On` 或 `Paused`。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。  |
|onPremisesLastSyncDateTime|DateTimeOffset|指示组最后一次与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 只读。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`）。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合| 在预配期间使用 Microsoft 同步产品时发生的错误。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`NOT`）。 |
|onPremisesSamAccountName|String|包含从本地目录同步的本地 **SAM 帐户名**。 仅当客户正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 时，才会填充该属性。<br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 只读。 |
|onPremisesSecurityIdentifier|String|包含从本地同步到云的组的本地安全标识符 (SID)。 <br><br>默认情况下返回。 支持 `null` 上的 `$filter`。 只读。 |
|onPremisesSyncEnabled|Boolean|如果此组从本地目录同步，则为 `true`；如果此组最初从本地目录同步，但以后不再同步，则为 `false`；如果此对象从未从本地目录同步，则为 **null**（默认值）。 <br><br>默认情况下返回。 只读。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。|
|preferredDataLocation|String|组的首选数据位置。 有关详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。 <br><br>默认情况下返回。|
|preferredLanguage|字符串|Microsoft 365 组的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。<br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `ge`、 `le`、 `in`、 `startsWith`）。 |
|proxyAddresses|String 集合| 指向同一组邮箱的组的电子邮件地址。 例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`。 需要 **any** 运算符筛选多值属性上的表达式。 <br><br>默认情况下返回。 只读。 不可为 null。 支持 `$filter`（`eq`、`NOT`、`ge`、`le`、`startsWith`）。 |
|renewedDateTime|DateTimeOffset| 组的上次续订时间戳。 值不能直接修改，只能通过[续订服务操作](../api/group-renew.md)进行更新。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`NOT`、`ge`、`le`、`in`）。 只读。|
|resourceBehaviorOptions|字符串集合|指定在创建期间可为 Microsoft 365 组设置的组行为。 可设置为只为创建的一部分（POST）。 可取值为：`AllowOnlyMembersToPost`、`HideGroupInOutlook`、`SubscribeNewGroupMembers`、`WelcomeEmailDisabled`。 有关详细信息，请参阅 [ 设置 Microsoft 365 组行为和预配选项 ](/graph/group-set-options)。|
|resourceProvisioningOptions|字符串集合|指定预配为创建 Microsoft 365 组的一部分，但通常不是创建默认组的组资源。 可能值为 `Team`。 有关详细信息，请参阅 [ 设置 Microsoft 365 组行为和预配选项 ](/graph/group-set-options)。|
|securityEnabled|布尔|指定是否为安全组。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `ne`、 `NOT`、 `in`）。|
|securityIdentifier|字符串|组的安全标识符，用于 Windows 方案。 <br><br>默认情况下返回。|
|theme|string|指定 Microsoft 365 组的颜色主题。 可能的值为：`Teal`、`Purple`、`Green`、`Blue`、`Pink`、`Orange` 或 `Red`。 <br><br>默认情况下返回。 |
|unseenCount|Int32|自登录用户上次访问该组以来收到新帖子的对话计数。 <br><br>仅在 `$select` 上返回。 仅支持"获取组 API"（`GET /groups/{ID}`）。 |
|visibility|String| 指定组的组加入策略和组内容可见性。 可能的值为： `Private`、 `Public`或 `Hiddenmembership`。 `Hiddenmembership` 仅在创建组时，<a0/&;<a1>为 Microsoft 365 组设置 </a1><a2/&;。 以后无法更新它。 创建组后，可更新其他可见性值。<br> 如果在 Microsoft Graph 上的组创建期间未指定可见性值，则默认创建安全组 `Private` Microsoft 365 组 `Public`。 请参阅[组可见性选项](#group-visibility-options)以了解详细信息。 <br><br>默认情况下返回。|


### <a name="group-visibility-options"></a>组可见性选项

|值|说明|
|:----|-----------|
| 公共 | 任何人均可在不需要所有者许可的情况下加入组。<br>任何人均可查看组的内容。|
| 私人 | 需要所有者许可才能加入组。<br>非成员无法查看组的内容。|
| Hiddenmembership | 需要所有者许可才能加入组。<br>非成员无法查看组的内容。<br>非成员无法查看组的成员。<br>管理员（全局、公司、用户和支持人员）可以查看组的成员资格。<br>该组显示在全局通讯簿 (GAL) 中。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) 集合|允许在此组中创建帖子或日历事件的用户或组列表。如果此列表为非空，则仅允许此处列出的用户或组发布内容。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|表示组已对应用程序授予的应用角色。 支持 `$expand`。|
|日历|[日历](calendar.md)|组日历。只读。|
|calendarView|[事件](event.md) 集合|日历的日历视图。只读。|
|conversations|[对话](conversation.md) 集合|组对话。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 创建组的用户（或应用程序）。注意：如果用户是管理员，则不设置此关系。只读。|
|驱动器|[drive](drive.md)|组的默认驱动器。只读。|
|drives|[drive](drive.md) 集合|组的驱动器。只读。|
|events|[事件](event.md) 集合|组的日历事件。|
|extensions|[扩展](extension.md)集合|为组定义的开放扩展集合。只读。可为 NULL。|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合|此组的生命周期策略集合。只读。可为空。|
|memberOf|[directoryObject](directoryobject.md) collection|此组所属的组。 HTTP 方法：GET（支持所有组） 只读。 可为 NULL。 支持 `$expand`。|
|members|[directoryObject](directoryobject.md) 集合| 属于此组成员的用户和组。 HTTP 方法：GET（支持所有组），POST（支持 Microsoft 365 组、安全组和启用邮件的安全组）、DELETE（支持 Microsoft 365 组和安全组）。 可为 NULL。 支持 `$expand`。|
|membersWithLicenseErrors|[User](user.md) 集合|在该基于组的许可证分配中存在许可证错误的组成员列表。只读。|
|onenote|[Onenote](onenote.md)| 只读。|
|owners|[directoryObject](directoryobject.md) 集合|组的所有者。 所有者是一组允许修改此对象的非管理员用户。 仅限 100 个所有者。 HTTP 方法：GET（支持所有组），POST（支持 Microsoft 365 组、安全组和启用邮件的安全组）、DELETE（支持 Microsoft 365 组和安全组）。 可为 NULL。 支持 `$expand`。|
|permissionGrants|[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)|已授予组对特定应用程序的权限。 支持 `$expand`。|
|photo|[profilePhoto](profilephoto.md)| 组的个人资料照片 |
|photos|[profilePhoto](profilephoto.md) 集合| 组拥有的个人资料照片。只读。可为 Null。|
|planner|[plannerGroup](plannergroup.md)| 统一组可能存在的 Planner 资源入口点。|
|rejectedSenders|[directoryObject](directoryobject.md) 集合|不允许在此组中创建帖子或日历事件的用户或组列表。可为 Null|
|设置|[groupSetting](groupsetting.md) 集合| 只读。可为 NULL。|
|sites|[网站](site.md)集|该组中的 SharePoint 网站的列表。使用 /sites/root 访问默认网站。|
|threads|[conversationThread](conversationthread.md) 集合| 组的对话线程。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "isAssignableToRole",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",
    "planner",
    "rejectedSenders",
    "settings",
    "sites",
    "threads",

    "allowExternalSenders",
    "assignedLicenses",
    "autoSubscribeNewMembers",
    "hasMembersWithLicenseErrors",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
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
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
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
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "hasMembersWithLicenseErrors": "Boolean",
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "isAssignableRole": false,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": ["String"],
  "resourceProvisioningOptions": ["String"],
  "securityEnabled": true,
  "securityIdentifier": "String",
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
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
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
