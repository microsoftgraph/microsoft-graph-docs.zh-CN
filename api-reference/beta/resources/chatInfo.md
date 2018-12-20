---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
ms.openlocfilehash: 45af1a7e178286c77ed4bf90528eb602fd48a6bb
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380413"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="73927-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="73927-103">chatInfo resource type</span></span>

> <span data-ttu-id="73927-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73927-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73927-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73927-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73927-106">有关 Microsoft 团队中的邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="73927-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="73927-107">属性</span><span class="sxs-lookup"><span data-stu-id="73927-107">Properties</span></span>

| <span data-ttu-id="73927-108">属性</span><span class="sxs-lookup"><span data-stu-id="73927-108">Property</span></span>            | <span data-ttu-id="73927-109">类型</span><span class="sxs-lookup"><span data-stu-id="73927-109">Type</span></span>    | <span data-ttu-id="73927-110">说明</span><span class="sxs-lookup"><span data-stu-id="73927-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="73927-111">messageId</span><span class="sxs-lookup"><span data-stu-id="73927-111">messageId</span></span>           | <span data-ttu-id="73927-112">字符串</span><span class="sxs-lookup"><span data-stu-id="73927-112">String</span></span>  | <span data-ttu-id="73927-113">Microsoft 团队通道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73927-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="73927-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="73927-114">replyChainMessageId</span></span> | <span data-ttu-id="73927-115">字符串</span><span class="sxs-lookup"><span data-stu-id="73927-115">String</span></span>  | <span data-ttu-id="73927-116">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="73927-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="73927-117">threadId</span><span class="sxs-lookup"><span data-stu-id="73927-117">threadId</span></span>            | <span data-ttu-id="73927-118">字符串</span><span class="sxs-lookup"><span data-stu-id="73927-118">String</span></span>  | <span data-ttu-id="73927-119">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73927-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73927-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73927-120">JSON representation</span></span>

<span data-ttu-id="73927-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73927-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
