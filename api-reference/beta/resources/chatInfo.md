---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 552844795d3ba7e8ad4c8a3c3a6dff3c18990bc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339691"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="a8ce5-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8ce5-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8ce5-104">有关 Microsoft 团队中的邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="a8ce5-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="a8ce5-105">属性</span><span class="sxs-lookup"><span data-stu-id="a8ce5-105">Properties</span></span>

| <span data-ttu-id="a8ce5-106">属性</span><span class="sxs-lookup"><span data-stu-id="a8ce5-106">Property</span></span>            | <span data-ttu-id="a8ce5-107">类型</span><span class="sxs-lookup"><span data-stu-id="a8ce5-107">Type</span></span>    | <span data-ttu-id="a8ce5-108">说明</span><span class="sxs-lookup"><span data-stu-id="a8ce5-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="a8ce5-109">messageId</span><span class="sxs-lookup"><span data-stu-id="a8ce5-109">messageId</span></span>           | <span data-ttu-id="a8ce5-110">String</span><span class="sxs-lookup"><span data-stu-id="a8ce5-110">String</span></span>  | <span data-ttu-id="a8ce5-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a8ce5-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="a8ce5-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="a8ce5-112">replyChainMessageId</span></span> | <span data-ttu-id="a8ce5-113">String</span><span class="sxs-lookup"><span data-stu-id="a8ce5-113">String</span></span>  | <span data-ttu-id="a8ce5-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="a8ce5-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="a8ce5-115">threadId</span><span class="sxs-lookup"><span data-stu-id="a8ce5-115">threadId</span></span>            | <span data-ttu-id="a8ce5-116">String</span><span class="sxs-lookup"><span data-stu-id="a8ce5-116">String</span></span>  | <span data-ttu-id="a8ce5-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a8ce5-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8ce5-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8ce5-118">JSON representation</span></span>

<span data-ttu-id="a8ce5-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8ce5-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
