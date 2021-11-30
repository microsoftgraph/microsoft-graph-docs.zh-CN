---
title: 组资源类型
description: 表示 Azure Active Directory (Azure AD) 组，可以是 Microsoft 365 组、Microsoft Teams 中的团队，或者安全组。
ms.localizationpriority: high
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 7b011d09483fc95b53dffac1f214991ddea38f91
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226181"
---
# <a name="group-resource-type"></a>组资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory (Azure AD) 组，可以是 Microsoft 365 组、Microsoft Teams 中的团队，或者安全组。 此资源是允许传入其他属性的开放类型。

继承自 [directoryObject](directoryobject.md)。

出于性能原因，默认情况下 [create](../api/group-post-groups.md)、[get](../api/group-get.md) 和 [list](../api/group-list.md) 操作仅返回更常用属性的子集。 这些 _默认_ 属性将记录在 [属性](#properties)部分中。 若要获取非默认返回的任一属性，请在 `$select` OData 查询选项中指定这些属性。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

> **Microsoft Teams 和 Microsoft 365 组支持组协作**。 您可结合使用大多数的 Microsoft 365 组 API 与 Microsoft Teams。 若要创建[团队](team.md)，首先要[创建组](../api/group-post-groups.md)，然后[向组添加团队](../api/team-put-teams.md)。 有关详细信息，请参阅 [Microsoft Teams 概述](teams-api-overview.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:------ |:----------- |:----------- |
| **组管理** |||
| [Create group](../api/group-post-groups.md) | [组](group.md) | 按指定方式创建新组。可以是 Microsoft 365 组、动态组、安全组或团队。 |
| [Get group](../api/group-get.md) | [group](group.md) | 读取 group 对象的属性和关系。 |
| [Update group](../api/group-update.md) | 无 | 更新 group 对象的属性。 |
| [删除组](../api/group-delete.md) | 无 | 删除组对象。 |
| [List groups](../api/group-list.md) | [group](group.md) | 读取所有 group 对象的属性和关系。 |
| [delta](../api/group-delta.md) | 组集合 | 获取组的增量更改。 |
| [添加成员](../api/group-post-members.md) | [directoryObject](directoryobject.md) | 通过发布到 **members** 导航属性将用户或组添加到此组（仅支持安全组和 Microsoft 365 组）。 |
| [添加所有者](../api/group-post-owners.md) | [directoryObject](directoryobject.md) | 通过发布到 **owners** 导航属性为组添加新所有者（仅支持安全组和 Microsoft 365 组）。 |
| [Create setting](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) | 基于 directorySettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。只有组特定模板可用于此操作。 |
| [删除设置](../api/directorysetting-delete.md) | 无 | 删除 setting 对象。 |
| [Get endpoint](../api/endpoint-get.md) | [endpoint](endpoint.md) | 读取 endpoint 对象的属性和关系。 |
| [Get setting](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) | 读取特定设置对象的属性。 |
| [List endpoints](../api/group-list-endpoints.md) | [endpoint](endpoint.md) 集合 | 获取 endpoint 对象集合。 |
| [List members](../api/group-list-members.md) | [directoryObject](directoryobject.md) 集合 | 从 **members** 导航属性中获取属于此组的直接成员的用户和组。 |
| [List memberOf](../api/group-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 通过 memberOf 导航属性，获取此组是其直接成员的组和管理单元。 |
| [列出 groupLifecyclePolicy](../api/group-list-grouplifecyclepolicies.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) 集合 | 列出组生命周期策略。 |
| [List owners](../api/group-list-owners.md) | [directoryObject](directoryobject.md) 集合 | 从 **owners** 导航属性中获取此组的所有者。 |
| [List settings](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) 集合 | 列出所有设置对象的属性。 |
| [List transitive members](../api/group-list-transitivemembers.md) | [directoryObject](directoryobject.md) 集合 | 获取属于此组成员（包括嵌套成员）的用户、组、设备和服务主体。 |
| [List transitive memberOf](../api/group-list-transitivememberof.md) | [directoryObject](directoryobject.md) 集合 | 列出此组所属的组和管理单元。 此操作是可传递的，并包括此组以嵌套方式所属的组。 |
| [删除所有者](../api/group-delete-owners.md) | 无 | 通过 **owners** 导航属性，删除 Microsoft 365 组、安全组或启用邮件安全组的所有者。 |
| [删除成员](../api/group-delete-members.md) | 无 | 通过 **members** 导航属性删除 Microsoft 365 组、安全组，或这启用邮的安全组中的成员。您可以删除用户或其他组。 |
| [Update setting](../api/directorysetting-update.md) | [directorySetting](directorysetting.md) | 更新 setting 对象。 |
| [assignLicense](../api/group-assignlicense.md) | [组](group.md) | 为群组添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。 |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | String 集合 | 在一列组中检查成员身份。此函数是可传递的。 |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | String 集合 | 检查组、目录角色或管理单元对象列表中的成员身份。该函数可传递。 |
| [evaluateDynamicMembership](../api/group-evaluatedynamicmembership.md) | [evaluateDynamicMembershipResult](evaluatedynamicmembershipresult.md) | 评估用户或设备是否为动态组的成员。 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | String collection | 返回此组是其成员的所有组。此函数是可传递的。 |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | String 集合 | 返回组所属的所有组和管理单元。此函数是可传递的。 |
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
| [列出 calendarView](../api/group-list-calendarview.md) | [event](event.md) 集合 | 获取指定时间范围内的事件集合。 |
| **对话** |||
| [创建对话](../api/group-post-conversations.md) | [conversation](conversation.md) | 通过发布到对话集合新建对话。 |
| [获取对话](../api/group-get-conversation.md) | [conversation](conversation.md) | 读取 conversation 对象的属性。 |
| [列出对话](../api/group-list-conversations.md) | [conversation](conversation.md) 集合 | 获取 conversation 对象集合。 |
| [删除对话](../api/group-delete-conversation.md) | 无 | 删除 conversation 对象。 |
| [创建线程](../api/group-post-threads.md) | [conversationThread](conversationthread.md) | 创建新的对话线程。 |
| [获取线程](../api/group-get-thread.md) | [conversationThread](conversationthread.md) | 读取 thread 对象的属性。 |
| [列出线程](../api/group-list-threads.md) | [conversationThread](conversationthread.md) 集合 | 获取组的所有线程。 |
| [更新线程](../api/group-update-thread.md) | 无 | 更新 thread 对象的属性。 |
| [删除线程](../api/group-delete-thread.md) | 无 | 删除 thread 对象 |
| [List acceptedSenders](../api/group-list-acceptedsenders.md) | [directoryObject](directoryobject.md) collection | 获取此组的“接受的发件人”列表中的用户或组列表。 |
| [添加 acceptedSender](../api/group-post-acceptedsenders.md) | [directoryObject](directoryobject.md) | 将用户或组添加到 acceptSenders 集合。 |
| [删除 acceptedSender](../api/group-delete-acceptedsenders.md) | [directoryObject](directoryobject.md) | 从 acceptedSenders 集合中删除用户或组。 |
| [List rejectedSenders](../api/group-list-rejectedsenders.md) | [directoryObject](directoryobject.md) collection | 获取此组的“遭拒的发件人”列表中的用户或组列表。 |
| [Add rejectedSender](../api/group-post-rejectedsenders.md) | [directoryObject](directoryobject.md) | 将新用户或组添加到 rejectedSenders 集合中。 |
| [Remove rejectedSender](../api/group-delete-rejectedsenders.md) | [directoryObject](directoryobject.md) | 从 rejectedSenders 集合中删除新用户或组。 |
| **开放扩展** |||
| [创建开放扩展](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | 创建开放扩展，并将自定义属性添加到新资源或现有资源。 |
| [获取开放扩展](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) 集合 | 获取扩展名称标识的开放扩展。 |
| **架构扩展** |||
| [添加架构扩展值](/graph/extensibility-schema-groups) | 无 | 创建架构扩展定义，然后使用它向资源添加自定义键入数据。 |
| **其他组资源** |||
| [List photos](../api/group-list-photos.md) | [profilePhoto](photo.md) 集合 | 获取组的个人资料照片集合。 |
| [List plannerPlans](../api/plannergroup-list-plans.md) | [plannerPlan](plannerplan.md) 集合 | 获取组拥有的 Planner 计划。 |
| [List permissionGrants](../api/group-list-permissiongrants.md) | [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合 | 列出已授予应用访问组的权限。 |
| **用户设置** |||
| [addFavorite](../api/group-addfavorite.md) | 无 | 将组添加到登录用户的收藏夹组列表中。仅支持 Microsoft 365 组。 |
| [removeFavorite](../api/group-removefavorite.md) | 无 | 从登录用户收藏夹组列表中删除组。仅支持 Microsoft 365 组。 |
| [List memberOf](../api/group-list-memberof.md) | [directoryObject](directoryobject.md) 集合 | 通过 **memberOf** 导航属性，获取此用户为其直接成员的组和管理单元。 |
| [List joinedTeams](../api/user-list-joinedteams.md) | [group](group.md) 集合 | 获取用户属于其直接成员的相应 Microsoft Teams。 |
| [subscribeByMail](../api/group-subscribebymail.md) | 无 | 将 isSubscribedByMail 属性设置为 `true`。启用已登录用户以接收电子邮件对话。仅支持 Microsoft 365 组。 |
| [unsubscribeByMail](../api/group-unsubscribebymail.md) | 无 | 将 isSubscribedByMail 属性设置为 `false`。禁用登录用户接收电子邮件对话。仅支持 Microsoft 365 组。 |
| [resetUnseenCount](../api/group-resetunseencount.md) | 无 | 将登录用户自上次访问后未查看的所有帖子的 unseenCount 重置为 0。仅支持 Microsoft 365 组。 |

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean| 指示组织外部的人员是否可以向组发送消息。默认值为 `false`。 <br><br>仅在 `$select`返回。仅在 Get 组 API （`GET /groups/{ID}`） 上受支持。 |
|assignedLabels|[assignedLabel](assignedlabel.md) 集合|与 Microsoft 365 组关联的敏感度标签对（标签 ID、标签名称）列表。 <br><br>仅在 `$select` 上返回。|
|assignedLicenses|[assignedLicense](assignedlicense.md) 集合|分配给该组的许可证。 <br><br>仅在 `$select` 上返回。 支持 `$filter`（`eq`）。 只读。|
|autoSubscribeNewMembers|布尔值|指示是否将自动订阅添加到组中的新成员以接收电子邮件通知。可以在组的 PATCH 请求中设置此属性;请勿在创建组的初始 POST 请求中设置它。默认值为 `false`。 <br><br>仅在 `$select`返回。仅在 Get 组 API （`GET /groups/{ID}`） 上受支持。|
|classification|字符串|描述该组的分类（如低、中或高业务影响）。通过根据[模板定义](directorysettingtemplate.md)创建 ClassificationList [设置](directorysetting.md)值来定义此属性的有效值。<br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`startsWith`）。|
|createdByAppId|字符串|用于创建组的应用 ID 对于部分组可能为 null。 <br><br>默认情况下返回。 只读。 支持 `$filter` （`eq`、 `ne`、 `not`、 `in`、 `startsWith`）。|
|createdDateTime|DateTimeOffset| 组的创建时间戳。 值无法修改，并在组创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`）。 只读。 |
|deletedDateTime|DateTimeOffset| 对于某些Azure Active Directory对象（用户、组、应用程序），如果删除对象，则首先在逻辑上删除该对象，并且此属性将更新为删除对象的日期和时间。否则，此属性为 null。如果还原对象，则此属性将更新为 null。 |
|说明|String|可选的组说明。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`startsWith`）和 `$search`。|
|displayName|String|组的显示名称。 必填。<br><br>默认情况下返回。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。|
|expirationDateTime|DateTimeOffset| 设置的组的过期时间戳。 值无法修改，并在组创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`）。 只读。 |
|groupTypes|String collection| 指定组类型及其成员身份。  <br><br>如果集合包含 `Unified`，则该组为Microsoft 365组；否则，它是安全组或通讯组。有关详细信息，请参阅 [组概述](groups-overview.md)。<br><br>如果该集合包含 `DynamicMembership`，则该组具有动态成员身份；否则，成员身份是静态的。  <br><br>默认返回。支持 `$filter`（`eq`、`not`）。|
|hasMembersWithLicenseErrors|Boolean| 指示此组中是否有该基于组的许可证分配中存在许可证错误的成员。 <br><br>在 GET 操作中从不返回此属性。可以将其用作 $filter 参数，以获取具有许可证错误成员的组（即筛选此属性为 `true`）<br><br>支持 `$filter`（`eq`）。|
|hideFromAddressLists |Boolean |如果 Outlook 用户界面的某些部分中未显示该组，则为 `true`：在 **通讯簿** 中、在选择邮件收件人的地址列表中，以及用于搜索组的 **浏览组** 对话框中；否则为 false。默认值为 `false`。 <br><br>仅在 `$select`返回。仅在 Get 组 API （`GET /groups/{ID}`） 上受支持。|
|hideFromOutlookClients |Boolean |如果在 Outlook 客户端（如 Outlook for Windows 和 Outlook 网页版）中未显示改组，则为 `true`，否则为 false。默认值为 `false`。 <br><br>仅在 `$select` 上返回。仅在 Get 组 API（`GET /groups/{ID}`）上受支持。|
|id|String|组的唯一标识符。 <br><br>默认情况下返回。 继承自 [directoryObject](directoryobject.md)。 键。 不可为 null。 只读。 <br><br>支持 `$filter` （`eq`、 `ne`、 `not`、 `in`）。|
|isAssignableToRole|Boolean|指示是否可以将此组分配给 Azure Active Directory 角色。 可选。<br><br>此属性只能在创建组时设置，并且不可变。 如果设置为 `true`，则 **securityEnabled** 属性也必须设置为 `true`，并且该组不能是动态组（即，**groupTypes** 不能包含 `DynamicMembership`）。 只有全局管理员和特权角色管理员角色中的调用方可以设置此属性。 必须向调用方分配 *RoleManagement.ReadWrite.Directory* 权限，才能设置此属性或更新此类组成员的身份。 有关更多信息，请参阅[使用组来管理 Azure AD 角色分配](https://go.microsoft.com/fwlink/?linkid=2103037)<br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`）。|
|infoCatalogs|字符串集合|标识分配给组的信息段。默认返回。支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）|
|isSubscribedByMail|Boolean|指示是否订阅已登录用户以接收电子邮件对话。默认值为 `true`。 <br><br>仅在 `$select`返回。仅在 Get 组 API （`GET /groups/{ID}`） 上受支持。 |
|licenseProcessingState|String|指示对该组所有成员的组许可证分配的状态。可能的值：`QueuedForProcessing`、`ProcessingInProgress` 和 `ProcessingComplete`。 <br><br>仅在 `$select` 返回。只读。 |
|mail|String|组的 SMTP 地址，例如，“serviceadmins@contoso.onmicrosoft.com”。 <br><br>默认情况下返回。 只读。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。|
|mailEnabled|Boolean|指定组是否启用邮件。必需。<br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not` 和 `null` 值上的 `eq`）。|
|mailNickname|String|组的邮件别名，在组织中是唯一的。 最大长度为 64 个字符。 此属性只能包含[ASCII 字符集 0 - 127](/office/vba/language/reference/user-interface-help/character-set-0127) 中的字符，以下除外：` @ () \ [] " ; : . <> , SPACE`。 <br><br>默认返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`、 `startsWith`）。|
|membershipRule|String|组为动态组时（groupTypes 包含 `DynamicMembership`），用于确定该组成员的规则。 有关成员身份规则语法的详细信息，请参阅[成员身份规则语法](https://azure.microsoft.com/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)。 <br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`startsWith`）。 |
|membershipRuleProcessingState|String|指示动态成员身份处理是打开还是暂停。可能的值为 `On` 或 `Paused`。 <br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`、`in`）。 |
|membershipRuleProcessingStatus|[membershipRuleProcessingStatus](membershipruleprocessingstatus.md) |描述基于规则的动态组的处理状态。 该属性 `null` 针对非基于规则的动态组或如果动态组处理已暂停。 <br><br>仅在 `$select` 上返回。仅在 Get 组 API (`GET /groups/{ID}`) 上受支持。只读。 |
|onPremisesDomainName|String|包含从本地目录同步的本地 **域 FQDN**，也称为 **dnsDomainName**。仅为正在通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。<br><br>默认返回。只读。 |
|onPremisesLastSyncDateTime|DateTimeOffset|指示上次将组与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 只读。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`）。|
|onPremisesNetBiosName|String|包含从本地目录同步的本地 **netBios 名称**。仅为通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充该属性。<br><br>默认返回。只读。 |
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合| 在预配期间使用 Microsoft 同步产品时发生的错误。 <br><br>默认返回。支持 `$filter`（`eq`、`not`）。 |
|onPremisesSamAccountName|String|包含从本地目录同步的本地 **SAM 帐户名称**。该属性仅为通过 Azure AD Connect 将其本地目录同步到 Azure Active Directory 的客户填充。<br><br>默认返回。 支持 `$filter` （`eq`、 `ne`、 `not`、 `ge`、 `le`、 `in`、 `startsWith`）。 只读。 |
|onPremisesSecurityIdentifier|String|包含从本地同步到云的组的本地安全标识符 (SID)。 <br><br>默认情况下返回。 支持 `null` 值上的 `$filter`。 只读。 |
|onPremisesSyncEnabled|Boolean|如果此组从本地目录同步，则为 `true`；如果此组最初从本地目录同步，但以后不再同步，则为 `false`；如果此对象从未从本地目录同步，则为 **null**（默认值）。 <br><br>默认情况下返回。 只读。 支持 `$filter`（`eq`、`ne`、`not`、`in` 和 `null` 值上的 `eq`）。 |
|preferredDataLocation|String|Microsoft 365 组的首选数据位置。 默认情况下，组继承组创建者的首选数据位置。 若要设置此属性，必须为调用用户分配以下 [Azure AD 角色之一](/azure/active-directory/roles/permissions-reference)： <br><ul><li> 全局管理员 <li> 用户帐户管理员 <li>目录写入程序 <li> Exchange 管理员 <li> SharePoint 管理员 </ul><br/> 有关此属性的详细信息，请参阅  [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。 <br><br>默认返回。可为空。|
|preferredLanguage|String|Microsoft 365 组的首选语言。应遵循 ISO 639-1 代码；例如，`en-US`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`）。 |
|proxyAddresses|String 集合| 指向同一组邮箱的组的电子邮件地址。 例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`。 需要多值属性筛选器表达式的 **any** 运算符。 <br><br>默认情况下返回。 只读。 不可为 null。 支持 `$filter`（`eq`、`not`、`ge`、`le`、`startsWith`）。 |
|renewedDateTime|DateTimeOffset| 组的上次续订时间戳。 值不能直接修改，只能通过[续订服务操作](../api/grouplifecyclepolicy-renewgroup.md)进行更新。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 <br><br>默认情况下返回。 支持 `$filter`（`eq`、`ne`、`not`、`ge`、`le`、`in`）。 只读。|
|resourceBehaviorOptions|字符串集合|指定在创建期间可为 Microsoft 365 组设置的组行为。 可设置为只为创建的一部分（POST）。 可取值为：`AllowOnlyMembersToPost`、`HideGroupInOutlook`、`SubscribeNewGroupMembers`、`WelcomeEmailDisabled`。 有关详细信息，请参阅 [ 设置 Microsoft 365 组行为和预配选项 ](/graph/group-set-options)。|
|resourceProvisioningOptions|字符串集合|指定预配为创建 Microsoft 365 组的一部分，但通常不是创建默认组的组资源。 可能值为 `Team`。 有关详细信息，请参阅 [ 设置 Microsoft 365 组行为和预配选项 ](/graph/group-set-options)。 <br><br>默认情况下返回。 支持 `$filter` （`eq`、 `not`、 `startsWith`。|
|securityEnabled|Boolean|指定组是否为安全组。必需。<br><br>默认返回。支持 `$filter`（`eq`、`ne`、`not`、`in`）。|
|securityIdentifier|字符串|组的安全标识符，用于 Windows 方案。 <br><br>默认情况下返回。|
|theme|String|指定 Microsoft 365 组的颜色主题。 可能的值为：`Teal`、`Purple`、`Green`、`Blue`、`Pink`、`Orange` 或 `Red`。 <br><br>默认情况下返回。 |
|unseenConversationsCount|Int32|自登录用户上次访问该组以来已传递一个或多个新帖子的对话计数。此属性与 **unseenCount** 相同。<br><br>仅在 `$select` 上返回。|
|unseenCount|Int32|自登录用户上次访问该组以来已收到新帖子的对话计数。此属性与 **unseenConversationsCount** 相同。<br><br>仅在 `$select` 上返回。仅在 Get 组 API（`GET /groups/{ID}`）上受支持。 |
|unseenMessagesCount|Int32|自登录用户上次访问该组以来已传递到组对话的新帖子计数。 <br><br>仅在 `$select` 上返回。|
|visibility|String| 指定组的组加入策略和组内容可见性。 可能的值为： `Private`、 `Public`或 `Hiddenmembership`。 `Hiddenmembership` 仅在创建组时，<a0/&;<a1>为 Microsoft 365 组设置 </a1><a2/&;。 以后无法更新它。 创建组后，可更新其他可见性值。<br> 如果在 Microsoft Graph 上的组创建期间未指定可见性值，则默认创建安全组 `Private` Microsoft 365 组 `Public`。  可分配给角色的组始终为 `Private`。 请参阅[组可见性选项](#group-visibility-options)以了解详细信息。 <br><br>默认返回。可为空。|

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
|appRoleAssignments|[appRoleAssignment](approleassignment.md) 集合|表示已为应用程序授予组的应用角色。支持 `$expand`。 |
|日历|[日历](calendar.md)|组日历。只读。|
|calendarView|[事件](event.md) 集合|日历的日历视图。只读。|
|conversations|[对话](conversation.md) 集合|组对话。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 创建组的用户（或应用程序）。**注意：** 如果用户是管理员，则不设置此项。只读。|
|drive|[drive](drive.md)|组的默认驱动器。只读。|
|drives|[drive](drive.md) 集合|组的驱动器。只读。|
|endpoints|[Endpoint](endpoint.md) 集合| 组的终结点。 只读。 可为 NULL。|
|events|[event](event.md) 集合|组事件。|
|extensions|[扩展](extension.md)集合|为组定义的开放扩展集合。只读。可为 NULL。|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合|此组的生命周期策略集合。只读。可为空。|
|memberOf|[directoryObject](directoryobject.md) collection|此组所属的组和管理单元。HTTP 方法：GET（支持所有组）。只读。可为 Null。支持 `$expand`。|
|members|[directoryObject](directoryobject.md) collection| 属于此组成员的用户、联系人和组。HTTP 方法：GET（支持所有组）、POST（支持安全组和已启用邮件的安全组）、DELETE（仅支持安全组）只读，可为 Null。支持 `$expand`。|
|membersWithLicenseErrors|[user](user.md) 集合|在该基于组的许可证分配中存在许可证错误的组成员列表。只读。|
|onenote|[onenote](onenote.md)| 只读。|
|owners|[directoryObject](directoryobject.md) 集合|组的所有者。 所有者是一组允许修改此对象的非管理员用户。 可为 NULL。 如果在创建 Microsoft 365 组时未指定此属性，则会自动将调用用户分配为组所有者。 支持 `$expand`。|
|permissionGrants|[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)|已授予针对组的特定应用程序的权限。支持 `$expand`。|
|photo|[profilePhoto](profilephoto.md)| 组的个人资料照片。 |
|photos|[profilePhoto](profilephoto.md) 集合| 组拥有的个人资料照片。只读。可为 Null。|
|planner|[plannerGroup](plannergroup.md)| 组可以使用的选择性计划程序服务。只读。可为 null。 |
|rejectedSenders|[directoryObject](directoryobject.md) 集合|不允许在此组中创建帖子或日历事件的用户或组列表。可为 Null|
|settings|[directorySetting](directorysetting.md) 集合| 可以管理此组行为的设置，例如成员是否可以将来宾用户邀请到此组。可为 null。|
|sites|[网站](site.md)集|该组中的 SharePoint 网站的列表。使用 /sites/root 访问默认网站。|
|threads|[conversationThread](conversationthread.md) 集合| 组的对话线程。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "endpoints",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "memberOf",
    "members",
    "membersWithLicenseErrors",
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
    "isAssignableToRole",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenConversationsCount",
    "unseenCount",
    "unseenMessagesCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLabels": [{"@odata.type": "microsoft.graph.assignedLabel"}],
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdByAppId": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": ["string"],
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "string (identifier)",
  "isFavorite": true,
  "isAssignableRole": false,
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesDomainName": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "string",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": ["String"],
  "resourceProvisioningOptions": ["String"],
  "securityEnabled": true,
  "securityIdentifier": "string",
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "string",
  "acceptedSenders": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "calendar": {"@odata.type": "microsoft.graph.calendar"},
  "calendarView": [{"@odata.type": "microsoft.graph.event"}],
  "conversations": [{"@odata.type": "microsoft.graph.conversation"}],
  "createdOnBehalfOf": {"@odata.type": "microsoft.graph.directoryObject"},
  "drive": {"@odata.type": "microsoft.graph.drive"},
  "events": [{"@odata.type": "microsoft.graph.event"}],
  "memberOf": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "members": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "photo": {"@odata.type": "microsoft.graph.profilePhoto"},
  "rejectedSenders": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "sites": [{"@odata.type": "microsoft.graph.site"}],
  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}],
  "classification": "string",
  "hasMembersWithLicenseErrors": true,
  "membershipRule": "string",
  "membershipRuleProcessingState": "string",
  "membershipRuleProcessingStatus":{"@odata.type": "microsoft.graph.membershipRuleProcessingStatus"},
  "preferredLanguage": "string",
  "theme": "string"
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
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

