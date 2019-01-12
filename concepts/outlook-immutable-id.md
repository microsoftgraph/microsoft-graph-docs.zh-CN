---
title: 获取 Outlook 资源的不可变标识符
description: Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。 虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。 借助不可变标识符，应用可以获取在项生存期内不变的 ID。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e88f4d457f76990dc3e6145ebf2730087ad2a74e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961713"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>获取 Outlook 资源的不可变标识符

Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。 虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。 借助不可变标识符，应用可以获取在项生存期内不变的 ID。

> **重要说明：** 不可变标识符仅适用于 Microsoft Graph /beta 版本。

## <a name="how-it-works"></a>工作原理

不可变 ID 是一项可选的 Microsoft Graph 功能。 若要选择使用此功能，应用必须在 API 请求中发送额外 HTTP 头：

```http
Prefer: IdType="ImmutableId"
```

此头仅适用于随附它的请求。 必须在每个 API 请求中随附此头，才能始终使用不可变 ID。

## <a name="lifetime-of-immutable-ids"></a>不可变 ID 生存期

只要项一直在同一邮箱中，它的不可变 ID 就不变。 也就是说，即使项移到邮箱中的其他文件夹中，不可变 ID 也不变。 不过，不可变 ID 在以下情况下会变：

- 用户将项移到存档邮箱中
- 用户先将项导出（到 PST 等，作为 MSG 文件），再将它重新导入邮箱

## <a name="items-that-support-immutable-id"></a>支持不可变 ID 的项

以下项支持不可变 ID：

- [message 资源类型](/graph/api/resources/message?view=graph-rest-beta)
- [attachment 资源类型](/graph/api/resources/attachment?view=graph-rest-beta)
- [event 资源类型](/graph/api/resources/event?view=graph-rest-beta)
- [eventMessage 资源类型](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [contact 资源类型](/graph/api/resources/contact?view=graph-rest-beta)
- [outlookTask 资源类型](/graph/api/resources/outlooktask?view=graph-rest-beta)

虽然容器类型（mailFolder、calendar 等）不支持不可变 ID，但其常规 ID 已是常量。

## <a name="immutable-id-with-change-notifications"></a>使用更改通知发送不可变 ID

可以在[创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)时添加 `Prefer: IdType="ImmutableId"` 头，从而请求 Microsoft Graph 在更改通知中发送不可变 ID。 未使用此头创建的的现有订阅将继续使用默认 ID 格式。 为了将现有订阅切换为使用不可变 ID，必须先删除它们，再使用此头重新创建它们。

## <a name="immutable-id-with-delta-query"></a>使用 delta 查询发送不可变 ID

可以通过添加 `Prefer: IdType="ImmutableId"` 头，请求 Microsoft Graph 在受支持资源类型的 [delta 查询响应](delta-query-overview.md)中返回不可变 ID。 由于 delta 查询返回的 `nextLink` 和 `deltaLink` 值与两种 ID 格式都兼容，因此应用无需重新同步，即可利用不可变 ID。 可以使用此头在以后获取不可变 ID，也可以单独[更新应用的存储](#updating-existing-data)。

## <a name="updating-existing-data"></a>更新现有数据

如果已获取填充有数千个常规 ID 的数据库，可使用 [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) 函数将这些 ID 迁移为不可变格式。 可以提供一组要转换为目标格式的 ID（最多 1000 个）。

> **注意：** 也可以使用 `translateExchangeIds` 将 Exchange Web 服务应用迁移到 Microsoft Graph。

### <a name="example"></a>示例

下面的示例将普通 Graph ID 转换为不可变 Graph ID。

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
