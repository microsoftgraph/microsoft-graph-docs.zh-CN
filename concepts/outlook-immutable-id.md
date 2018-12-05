---
title: 获取 Outlook 资源不可变标识符
description: Outlook 项目 （邮件、 事件、 联系人、 任务） 具有有趣的行为，您可能已之一永远不会注意到或已导致重大失望： 更改其 Id。 它不会经常发生，仅当项目将被移动，但它可能会导致应用程序的更高版本用于存储脱机 Id 实际问题。 不可变标识符使您的应用程序获取不会更改项目的生存期内的 ID。
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091902"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>获取 Outlook 资源不可变标识符

Outlook 项目 （邮件、 事件、 联系人、 任务） 具有有趣的行为，您可能已之一永远不会注意到或已导致重大失望： 更改其 Id。 它不会经常发生，仅当项目将被移动，但它可能会导致应用程序的更高版本用于存储脱机 Id 实际问题。 不可变标识符使您的应用程序获取不会更改项目的生存期内的 ID。

> **重要：** 不可变标识符是仅可供使用的 Microsoft Graph /beta 版本上。

## <a name="how-it-works"></a>工作原理

不可变 ID 是 Microsoft Graph 可选功能。 若要选择加入，您的应用程序需要发送 API 请求中的其他 HTTP 标头：

```http
Prefer: IdType="ImmutableId"
```

此标头仅适用于它是包含该请求。 如果您希望始终使用不可变 Id，您必须包含与每个 API 请求此标头。

## <a name="lifetime-of-immutable-ids"></a>不可变 Id 的生存期

只要项目将停留在同一邮箱，则不会更改项目的不可变 ID。 也就是说，如果项目将被移动到另一个邮箱中的文件夹不会更改变 ID。 但是，如果将更改变 ID:

- 用户将项目移动到存档邮箱
- 用户导出 （到 PST，作为 MSG 文件等) 的项并重新将它导入到其邮箱

## <a name="items-that-support-immutable-id"></a>支持变 ID 的项目

以下各项支持变 Id:

- [邮件资源类型](/graph/api/resources/message?view=graph-rest-beta)
- [attachment 资源类型](/graph/api/resources/attachment?view=graph-rest-beta)
- [事件资源类型](/graph/api/resources/event?view=graph-rest-beta)
- [eventMessage 资源类型](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [联系人资源类型](/graph/api/resources/contact?view=graph-rest-beta)
- [outlookTask 资源类型](/graph/api/resources/outlooktask?view=graph-rest-beta)

（mailFolder、 日历等） 的容器类型不支持变 ID，但是它们的正则 Id 已常量。

## <a name="immutable-id-with-change-notifications"></a>更改通知不可变 ID

您可以请求对 Microsoft Graph 发送变 Id 中的更改通知通过包括`Prefer: IdType="ImmutableId"`标头时[创建的订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。 创建没有标头的现有订阅将继续使用的默认 ID 格式。 为了切换现有订阅使用不可变 Id，则必须删除并重新创建这些使用头。

## <a name="immutable-id-with-delta-query"></a>不可变 ID 增量查询

您可以请求，Microsoft Graph 返回变 Id 中支持的资源类型的[增量查询响应](delta-query-overview.md)通过包括`Prefer: IdType="ImmutableId"`标头。 `nextLink`和`deltaLink`增量查询所返回的值都与两个 ID 格式，兼容，因此您的应用程序不需要重新同步利用变 id。 您可以使用标题获取变 Id 循序，并且可以[更新您的应用程序存储](#updating-existing-data)分开。

## <a name="updating-existing-data"></a>更新现有数据

如果您已经有了填充数千个正则 Id 的数据库，您可以为不可变格式使用[translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta)函数来迁移这些 Id。 您可以提供最多 1000 Id 为目标格式转换的数组。

> **注意：** 您还可以使用`translateExchangeIds`迁移到 Microsoft Graph 的 Exchange Web 服务应用程序。

### <a name="example"></a>示例

下面的示例将转换的普通图 ID 变图 id。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a>响应

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```