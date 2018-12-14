---
title: 组资源类型
description: 代表 Azure Active Directory (Azure AD) 组，这可以是 Office 365 组、 团队中的 Microsoft 团队、 动态组或安全组。
ms.openlocfilehash: d48448991b75946f9ac60a037fee3b083601954a
ms.sourcegitcommit: 5747eb595bf0c7c391b2a5219c3ae9b6a48df26b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/14/2018
ms.locfileid: "27265232"
---
# <a name="group-resource-type"></a>组资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表 Azure Active Directory (Azure AD) 组，这可以是 Office 365 组、 团队中的 Microsoft 团队、 动态组或安全组。
继承自 [directoryObject](directoryobject.md)。

该资源支持：

- 将您自己的数据添加到自定义属性，作为[扩展](/graph/extensibility-overview)。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/user-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

> **Microsoft 团队和 Office 365 组支持组协作**。 大多数 Office 365 组 API 可用于 Microsoft 团队。 创建[团队](team.md)、 第一个[创建组](../api/group-post-groups.md)，然后[添加到该团队](../api/team-put-teams.md)。 有关详细信息，请参阅[Microsoft 团队概述](teams-api-overview.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**组管理**| | |
|[Create group](../api/group-post-groups.md) | [组](group.md) |创建指定一个新组。 它可以是 Office 365 组、 动态组、 安全组或团队。|
|[获取组](../api/group-get.md) | [组](group.md) |读取属性和组对象的关系。|
|[更新组](../api/group-update.md) | 无 |更新 group 对象的属性。 |
|[删除组](../api/group-delete.md) | 无 |删除组对象。 |
|[增量](../api/group-delta.md)|组集合| 获取组的增量更改。 |
|[列出 groupLifecyclePolicy](../api/group-list-grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合| 列出组生命周期策略。 |
|[列出所有者](../api/group-list-owners.md) |[directoryObject](directoryobject.md) 集合| 从 **owners** 导航属性中获取此组的所有者。|
|[添加所有者](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| 通过发布到 **owners** 导航属性，添加此组的新所有者（仅支持为安全组和启用邮件的安全组添加）。|
|[删除所有者](../api/group-delete-owners.md) | 无 |通过 **owners** 导航属性，删除 Office 365 组、安全组或启用邮件的安全组的所有者。|
|[列出成员](../api/group-list-members.md) |[directoryObject](directoryobject.md) 集合| 从 **members** 导航属性中获取属于此组的直接成员的用户和组。|
|[列出可传递成员](../api/group-list-transitivemembers.md) |[directoryObject](directoryobject.md) 集合| 获取用户、 组、 设备和服务主体的成员，包括嵌套此组的成员。|
|[添加成员](../api/group-post-members.md) |[directoryObject](directoryobject.md)| 通过发布到 **members** 导航属性将用户或组添加到此组（仅支持安全组和启用邮件的安全组）。|
|[删除成员](../api/group-delete-members.md) | 无 |通过 **members** 导航属性删除 Office 365 组、安全组或启用邮件的安全组中的成员。可以删除用户或其他组。 |
|[List memberOf](../api/group-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 获取组和管理单位属于此组直接成员的从 memberOf 导航属性。|
|[列表可传递 memberOf](../api/group-list-transitivememberof.md) |[directoryObject](directoryobject.md) 集合| 组和管理单元，此用户是其成员的列表。 此操作可传递，包括此组的嵌套的成员的组。 |
|[checkMemberGroups](../api/group-checkmembergroups.md)|String collection|检查列表中的组的成员资格。 可传递函数。|
|[getMemberGroups](../api/group-getmembergroups.md)|String collection|返回此组是其成员的所有组。此函数是可传递的。|
|[getMemberObjects](../api/group-getmemberobjects.md)|String collection|返回的所有组和管理单元的组的成员。 可传递函数。 |
|[创建设置](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |创建基于 directorySettingTemplate 设置对象。 POST 请求必须提供 settingValues 模板中定义的所有设置。 组特定模板可能用于此操作。|
|[获取设置](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |读取特定设置对象的属性。|
|[列出设置](../api/directorysetting-list.md) | [directorySetting](directorysetting.md)集合 |列出所有设置对象的属性。|
|[更新设置](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |更新 setting 对象。 |
|[删除设置](../api/directorysetting-delete.md) | 无 |删除设置对象。 |
|[列出终结点](../api/group-list-endpoints.md) |[终结点](endpoint.md)集合| 获取一个终结点对象集合。 |
|[获取终结点](../api/endpoint-get.md) | [终结点](endpoint.md) | 读取属性和终结点对象的关系。 |
|[delta](../api/group-delta.md)|组集合| 获取组的增量更改。 |
|[validateProperties](../api/group-validateproperties.md)|JSON| 验证 Office 365 组的显示名称或邮件昵称符合命名策略。 | 
|**日历**| | |
|[创建事件](../api/group-post-events.md) |[event](event.md)| 通过发布到事件集合新建事件。|
|[获取事件](../api/group-get-event.md) |[event](event.md)|读取 event 对象的属性。|
|[列出事件](../api/group-list-events.md) |[event](event.md) 集合| 获取 event 对象集合。|
|[更新事件](../api/group-update-event.md) |无|更新 event 对象的属性。|
|[删除事件](../api/group-delete-event.md) |无|删除 event 对象。|
|[列出 calendarView](../api/group-list-calendarview.md) |[event](event.md) 集合| 获取指定时间范围内的事件集合。|
|**对话**| | |
|[创建对话](../api/group-post-conversations.md) |[conversation](conversation.md)| 通过发布到对话集合新建对话。|
|[获取对话](../api/group-get-conversation.md) |[conversation](conversation.md)| 读取 conversation 对象的属性。|
|[列出对话](../api/group-list-conversations.md) |[conversation](conversation.md) 集合| 获取 conversation 对象集合。|
|[删除对话](../api/group-delete-conversation.md) |无|删除 conversation 对象。|
|[获取线程](../api/group-get-thread.md) |[conversationThread](conversationthread.md)| 读取 thread 对象的属性。|
|[列出线程](../api/group-list-threads.md) |[conversationThread](conversationthread.md) 集合| 获取组的所有线程。|
|[更新线程](../api/group-update-thread.md) |无| 更新 thread 对象的属性。|
|[删除线程](../api/group-delete-thread.md) |无| 删除线程对象
|[列出 acceptedSenders](../api/group-list-acceptedsenders.md) |[directoryObject](directoryobject.md) 集合| 获取此组 acceptedSenders 列表中的用户或组列表。|
|[添加 acceptedSender](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| 将用户或组添加到 acceptSenders 集合。|
|[删除 acceptedSender](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| 从 acceptedSenders 集合中删除用户或组。|
|[List rejectedSenders](../api/group-list-rejectedsenders.md) |[directoryObject](directoryobject.md) 集合| 获取此组的 rejectedSenders 列表中的用户或组列表。|
|[Add rejectedSender](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| 将新用户或组添加到 rejectedSenders 集合中。|
|[Remove rejectedSender](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| 从 rejectedSenders 集合中删除新用户或组。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**其他组资源**| | |
|[List photos](../api/group-list-photos.md) |[profilePhoto](photo.md) 集合| 获取组的个人资料照片集合。|
|[List plannerPlans](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) 集合| 获取组拥有的 Planner 计划。|
|**用户设置**| | |
|[addFavorite](../api/group-addfavorite.md)|无|将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。|
|[removeFavorite](../api/group-removefavorite.md)|无|从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。|
|[List memberOf](../api/group-list-memberof.md) |[directoryObject](directoryobject.md) 集合| 通过 **memberOf** 导航属性，获取此用户是其直接成员的组和管理单元。|
|[列出 joinedTeams](../api/user-list-joinedteams.md) |[组](group.md) 集合| 获取用户属于其直接成员的 Microsoft 团队。|
|[subscribeByMail](../api/group-subscribebymail.md)|无|将 isSubscribedByMail 属性设置为**true**。 使当前用户可以接收电子邮件对话。 Office 365 组仅支持。|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|无|将 isSubscribedByMail 属性设置为**false**。 禁用当前用户接收电子邮件对话。 Office 365 组仅支持。|
|[resetUnseenCount](../api/group-resetunseencount.md)|无|将 unseenCount 重置为 0 的上次访问后没有发现当前用户的所有文章。 Office 365 组仅支持。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|默认为 **false**。指明组织外部人员能否向群组发送邮件。|
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|分配给组的许可证。 只读。|
|autoSubscribeNewMembers|Boolean|默认为 **false**。指示添加到组中的新成员是否将自动订阅接收电子邮件通知。可以在 PATCH 请求中设置组的该属性；不要在创建该组的初始 POST 请求中设置该属性。|
|Classification|String|描述该组的分类（如低、中或高业务影响）。通过根据[模板定义](directorysettingtemplate.md)创建 ClassificationList [设置](directorysetting.md)值来定义此属性的有效值。|
|createdDateTime|DateTimeOffset| 组的创建时间戳。 值无法修改，并在组创建时自动填充。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 |
|说明|String|可选的组说明。|
|displayName|字符串|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|groupTypes|String collection| 指定要创建组的类型。 可能的值为`Unified`创建 Office 365 组，或`DynamicMembership`动态组。  所有其他组类型，如启用安全的组和已启用电子邮件的安全组，未设置此属性。|
|id|String|组的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。|
|isSubscribedByMail|Boolean|默认值为 **True**。指示当前用户是否订阅接收电子邮件对话。|
|licenseProcessingState|字符串|指示的组许可证分配给组的所有成员的状态。 只读。 可能的值： `QueuedForProcessing`， `ProcessingInProgress`，和`ProcessingComplete`。|
|mail|String|组的 SMTP 地址，例如，“serviceadmins@contoso.onmicrosoft.com”。只读。支持 $filter。|
|mailEnabled|Boolean|指定该组是否启用邮件。如果 **securityEnabled** 属性也为 **true**，则该组是已启用邮件的安全组；否则是 Microsoft Exchange 通讯组。|
|mailNickname|String|组的邮件别名，在组织中是唯一的。创建组时必须指定此属性。支持 $filter。|
|membershipRule|字符串|确定组是一个动态组对此组的成员的规则 (groupTypes 包含`DynamicMembership`)。 成员资格规则的语法的详细信息，请参阅[成员资格规则语法](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|字符串|指示动态成员资格处理上还是已暂停。 可能的值为"开"或"暂停"|
|onPremisesLastSyncDateTime|DateTimeOffset|指示的上次与内部部署目录同步对象的频率。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 支持 $filter。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)集合| 设置过程中使用 Microsoft 同步产品时错误。 |
|onPremisesSecurityIdentifier|String|包含从本地同步到云的组的本地安全标识符 (SID)。只读。 |
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。 只读。 支持 $filter。|
|preferredDataLocation|字符串|首选的数据组的位置。 有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。|
|preferredLanguage|字符串|Office 365 组首选的语言。 应按照操作 ISO 639 1 代码;如"EN-US"。|
|proxyAddresses|String collection| 例如： `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**运算符，则需要为多值属性的筛选器表达式。 只读。 不可为 null。 支持 $filter。 |
|renewedDateTime|DateTimeOffset| 组的上次续订时间戳。 值不能直接修改，只能通过[续订服务操作](../api/grouplifecyclepolicy-renewgroup.md)进行更新。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|securityEnabled|Boolean|指定是否为安全组。如果 **mailEnabled** 属性也为 true，则该组是已启用邮件的安全组；否则为安全组。对于 Office 365 组，必须为 **false**。支持 $filter。|
|主题|字符串|指定 Office 365 组的颜色主题。 可能的值为`Teal`， `Purple`， `Green`， `Blue`， `Pink`，`Orange`或`Red`。|
|unseenConversationsCount|Int32|向组的登录用户上次访问后已送达一个或多个新文章的对话数。 此属性是**unseenCount**相同。|
|unseenCount|Int32|向组的登录用户上次访问后已送达一个或多个新文章的对话数。 此属性是**unseenConversationsCount**相同。|
|unseenMessagesCount|Int32|已传递到组的对话到组的登录用户上次访问后的新文章的计数。|
|visibility|String| 指定 Office 365 组可见的性。 可能的值为： `private`， `public`，或`hiddenmembership`;空值被视为为公共。  请参阅[组可见性选项](#group-visibility-options)了解详细信息。<br>仅当创建一组; 时，可以设置可见性不可编辑。<br>仅支持统一组; 可见性不支持安全组。|

### <a name="group-visibility-options"></a>组可见性选项

下面是每个**可见性**属性值的含义：
 
|值|说明|
|:----|-----------|
| `public` | 任何人都可以加入的组，而无需所有者权限。<br>任何人都可以查看组的内容。|
| `private` | 所需的所有者权限加入的组。<br>非成员不能查看组的内容。|
| `hiddenmembership` | 所需的所有者权限加入的组。<br>非成员不能查看组的内容。<br>非成员看不到组的成员。<br>（全局、 公司、 用户和帮助台） 的管理员可以查看组成员资格。<br>组显示在全局通讯簿 (GAL)。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) 集合|允许在此组中创建帖子或日历事件的用户或组列表。如果此列表为非空，则仅允许此处列出的用户或组发布内容。|
|日历|[日历](calendar.md)|组日历。只读。|
|calendarView|[事件](event.md) 集合|日历的日历视图。只读。|
|conversations|[对话](conversation.md) 集合|组对话。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 创建组的用户（或应用程序）。注意：如果用户是管理员，则不设置此关系。只读。|
|驱动器|[驱动器](drive.md)|组的默认驱动器。 只读。|
|驱动器|[驱动器](drive.md) 集合|组的驱动器。 只读。|
|终结点|[终结点](endpoint.md)集合| 组的终结点。 只读。 可为 Null。|
|events|[事件](event.md) 集合|组的事件。|
|extensions|[扩展](extension.md)集合|为组定义的开放扩展集合。只读。可为 NULL。|
|groupLifecyclePolicies|[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合|对此组的生命周期策略的集合。 只读。 可为 Null。|
|memberOf|[directoryObject](directoryobject.md) 集合|组和管理单位属于此组的成员。 HTTP 方法： 获取 （支持的所有组）。 只读。 可为 Null。|
|members|[directoryObject](directoryobject.md) 集合| 用户、 联系人和组属于此组的成员。 HTTP 方法： 获取 （受支持的所有组），开机自检 （支持安全组和已启用邮件的安全组），删除 （只支持针对安全组） 只读的。 可为 Null。|
|membersWithLicenseErrors|[用户](user.md)集合|与此组基于许可证分配许可证错误的组成员的列表。 只读。|
|onenote|[OneNote](onenote.md)| 只读。|
|owners|[directoryObject](directoryobject.md) 集合|组的所有者。 所有者是一组的非管理员用户有权修改此对象。 HTTP 方法： 获取 （受支持的所有组），开机自检 （支持安全组和已启用邮件的安全组），删除 （只支持针对安全组） 只读的。 可为 Null。|
|photo|[profilePhoto](profilephoto.md)| 组的配置文件照片。 |
|photos|[profilePhoto](profilephoto.md) 集合| 组拥有的个人资料照片。只读。可为 Null。|
|planner|[plannerGroup](plannergroup.md)| 选择性可用到组的计划程序服务。 只读。 可为 Null。 |
|rejectedSenders|[directoryObject](directoryobject.md) 集合|不允许在此组中创建帖子或日历事件的用户或组列表。可为 Null|
|settings|[directorySetting](directorysetting.md)集合| 可以管理此组的行为，如成员是否可以邀请到组的来宾用户的设置。 可为 Null。|
|sites|[网站](site.md)集|该组中的 SharePoint 网站的列表。使用 /sites/root 访问默认网站。|
|threads|[conversationThread](conversationthread.md) 集合| 组的对话线程。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
以下是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",    
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isFavorite": true,  
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": ["string"],
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
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
