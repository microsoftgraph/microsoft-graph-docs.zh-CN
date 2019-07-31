---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a2c7b705078e49c7e3bd68056b698e05d3f83bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012973"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="ed586-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed586-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed586-104">有关 Microsoft 团队中的邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="ed586-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="ed586-105">属性</span><span class="sxs-lookup"><span data-stu-id="ed586-105">Properties</span></span>

| <span data-ttu-id="ed586-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed586-106">Property</span></span>            | <span data-ttu-id="ed586-107">类型</span><span class="sxs-lookup"><span data-stu-id="ed586-107">Type</span></span>    | <span data-ttu-id="ed586-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed586-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ed586-109">messageId</span><span class="sxs-lookup"><span data-stu-id="ed586-109">messageId</span></span>           | <span data-ttu-id="ed586-110">String</span><span class="sxs-lookup"><span data-stu-id="ed586-110">String</span></span>  | <span data-ttu-id="ed586-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed586-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="ed586-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="ed586-112">replyChainMessageId</span></span> | <span data-ttu-id="ed586-113">String</span><span class="sxs-lookup"><span data-stu-id="ed586-113">String</span></span>  | <span data-ttu-id="ed586-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="ed586-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="ed586-115">threadId</span><span class="sxs-lookup"><span data-stu-id="ed586-115">threadId</span></span>            | <span data-ttu-id="ed586-116">String</span><span class="sxs-lookup"><span data-stu-id="ed586-116">String</span></span>  | <span data-ttu-id="ed586-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed586-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed586-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed586-118">JSON representation</span></span>

<span data-ttu-id="ed586-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed586-119">The following is a JSON representation of the resource.</span></span>

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
