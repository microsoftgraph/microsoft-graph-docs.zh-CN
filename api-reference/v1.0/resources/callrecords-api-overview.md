---
title: 使用 Microsoft Graph 中的通话记录 API
description: Microsoft Graph 通话记录 API 可用于检索组织内的通话和联机会议的使用情况和诊断数据。
author: williamlooney
doc_type: conceptualPageType
ms.prod: cloud-communications
ms.localizationpriority: high
ms.openlocfilehash: 7a672ae93421fe886cab06e13bb449d75f09659b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104353"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a>使用 Microsoft Graph 中的通话记录 API

通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。 可使用通话记录 API 来订阅通话记录，并按 ID 查找通话记录。

通话记录 API 在 OData 子命名空间中定，`microsoft.graph.callRecords`。

## <a name="key-resource-types"></a>重要资源类型

| Resource | Methods |
| :-- | :-- |
| [callRecord](callrecords-callrecord.md) | [获取 callRecord](../api/callrecords-callrecord-get.md) |
| [Session](callrecords-session.md) | [获取 callRecord](../api/callrecords-callrecord-get.md)<br />[列表会话](../api/callrecords-session-list.md) |
| [segment](callrecords-segment.md) | [获取 callRecord](../api/callrecords-callrecord-get.md)<br />[列表会话](../api/callrecords-session-list.md) |
| [pstnCallLogRow](callrecords-pstncalllogrow.md)|[getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) |
| [directRoutingLogRow](callrecords-directroutinglogrow.md) | [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md)|

## <a name="call-record-structure"></a>呼叫记录结构

[callRecord](callrecords-callrecord.md) 实体表示多个参与者之间的单个对等呼叫或群组呼叫，有时称为联机会议。

对等呼叫包含呼叫中两个参与者之间的单个 [session](callrecords-session.md)。 群组呼叫包含一个或多个 **session** 实体。 在群组呼叫中，每个 **session** 都介于参与者和服务终结点之间。

每个 **session** 都包含一个或多个 [segment](callrecords-segment.md) 实体。 **segment** 表示两个 [终结点](callrecords-endpoint.md)之间的媒体链接。 对于大多数呼叫，每个 **session** 仅显示一个 **segment**，但有时可能会有一个或多个中间 **终结点**。

![表示完整通话记录的数据结构的图像](/graph/images/callrecords-structure.png)

在上图中，数字表示每种类型可以有多少个子类型。 例如，**callRecord** 与 **session** 之间的 1..N 关系意味着一个 **callRecord** 实例可以包含一个或多个 **session** 实例。 同样，**segment** 与 **media** 之间的 1..N 关系意味着一个 **segment** 实例可以包含一个或多个 [media](callrecords-media.md) 流。

## <a name="see-also"></a>另请参阅

- [Webhook 订阅](/graph/api/resources/webhooks?view=graph-rest-1.0&preserve-view=true)

