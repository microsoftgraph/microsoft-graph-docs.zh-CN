---
title: 获取 Outlook 资源的不可变标识符
description: 使用不可变标识符 (ID) 使 Outlook 应用程序能够获取在项目生存期内不会更改的 ID。
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 352dfd7fe55b5d98fcf1477a4049965100572c46
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444738"
---
# <a name="obtain-immutable-identifiers-for-outlook-resources"></a>获取 Outlook 资源的不可变标识符

Outlook 项（邮件、事件、联系人、任务）有一个有趣行为，你可能从未注意到或已给你带来了极大挫败感，即它们的 ID 会变。 虽然这一行为不是经常发生（只在项移动时才会发生），但对于脱机存储 ID 以供日后使用的应用来说，这可能会导致真正的问题出现。 不可变的标识符 (ID) 使应用程序能够获得在项目生命周期内不会更改的 ID。

> [!NOTE]
> 不可变标识符（如 Microsoft Graph 中的所有标识符）区分大小写。 如果要比较 ID，请记住这一点。

## <a name="how-it-works"></a>运作方式

不可变 ID 是一项可选的 Microsoft Graph 功能。 若要选择使用此功能，应用必须在 API 请求中发送额外 HTTP 头：

```http
Prefer: IdType="ImmutableId"
```

此头仅适用于随附它的请求。 必须在每个 API 请求中随附此头，才能始终使用不可变 ID。

## <a name="lifetime-of-immutable-ids"></a>不可更改的 ID 生存期

只要项一直在同一邮箱中，它的不可变 ID 就不变。 也就是说，即使项移到邮箱中的其他文件夹中，不可变 ID 也不变。 不过，不可变 ID 在以下情况下会变：

- 用户将该项移到存档邮箱中。
- 用户先将该项导出（到 PST 等，作为 MSG 文件），再将它重新导入邮箱。

## <a name="items-that-support-immutable-ids"></a>支持不可更改 ID 的项

以下项支持不可变 ID：

- [message 资源类型](/graph/api/resources/message)
- [attachment 资源类型](/graph/api/resources/attachment)
- [event 资源类型](/graph/api/resources/event)
- [eventMessage 资源类型](/graph/api/resources/eventmessage)
- [contact 资源类型](/graph/api/resources/contact)
- [outlookTask 资源类型](/graph/api/resources/outlooktask)

虽然容器类型（mailFolder、calendar 等）不支持不可变 ID，但其常规 ID 已是常量。

## <a name="immutable-id-with-sending-mail"></a>已发送邮件的不可变 ID

发送邮件后，可以使用不可变 ID 在“已发送邮件”文件夹中查找邮件，步骤如下：

1. 使用 `Prefer: IdType="ImmutableId"` 标头[创建邮件草稿](/graph/api/user-post-messages)，并将邮件的 `id` 属性保存在回复中。
1. 使用上一步中的 ID [发送邮件](/graph/api/message-send)。
1. 使用第一步中的 ID [获取邮件](/graph/api/message-get)。 这是“已发送邮件”中的副本。

> [!NOTE]
> 发送邮件后，无法立即在“已发送邮件”中获取邮件。 在成功发送邮件之前，不会创建邮件的副本，这可能需要一些时间。

## <a name="immutable-id-with-change-notifications"></a>使用更改通知发送不可变 ID

可以在[创建订阅](/graph/api/subscription-post-subscriptions)时添加 `Prefer: IdType="ImmutableId"` 头，从而请求 Microsoft Graph 在更改通知中发送不可变 ID。 未使用此头创建的的现有订阅将继续使用默认 ID 格式。 为了将现有订阅切换为使用不可变 ID，必须先删除它们，再使用此头重新创建它们。

## <a name="immutable-id-with-delta-query"></a>使用 delta 查询发送不可变 ID

可以通过添加 `Prefer: IdType="ImmutableId"` 头，请求 Microsoft Graph 在受支持资源类型的 [delta 查询响应](delta-query-overview.md)中返回不可变 ID。 由于 delta 查询返回的 `@odata.nextLink` 和 `@odata.deltaLink` 值与两种 ID 格式都兼容，因此应用无需重新同步，即可利用不可变 ID。 可以使用此头在以后获取不可变 ID，也可以单独[更新应用的存储](#updating-existing-data)。

## <a name="updating-existing-data"></a>更新现有数据

如果已获取填充有数千个常规 ID 的数据库，可使用 [translateExchangeIds](/graph/api/user-translateexchangeids) 函数将这些 ID 迁移为不可变格式。 可以提供一组要转换为目标格式的 ID（最多 1000 个）。

> [!NOTE]
> 还可使用 `translateExchangeIds` 将 Exchange Web 服务应用程序迁移到 Microsoft Graph。

### <a name="example"></a>示例

下面的示例将普通 Microsoft Graph ID 转换为不可更改的 Microsoft Graph ID。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds

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
