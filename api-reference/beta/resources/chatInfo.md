---
title: chatInfo 资源类型
description: 包含与 Microsoft 团队会议相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb3806cf28e5557d7b5e4bf0296083e3c595047c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913147"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="15c93-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="15c93-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15c93-104">包含与 Microsoft 团队会议相关的信息。</span><span class="sxs-lookup"><span data-stu-id="15c93-104">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="15c93-105">属性</span><span class="sxs-lookup"><span data-stu-id="15c93-105">Properties</span></span>

| <span data-ttu-id="15c93-106">属性</span><span class="sxs-lookup"><span data-stu-id="15c93-106">Property</span></span>            | <span data-ttu-id="15c93-107">类型</span><span class="sxs-lookup"><span data-stu-id="15c93-107">Type</span></span>    | <span data-ttu-id="15c93-108">说明</span><span class="sxs-lookup"><span data-stu-id="15c93-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="15c93-109">messageId</span><span class="sxs-lookup"><span data-stu-id="15c93-109">messageId</span></span>           | <span data-ttu-id="15c93-110">String</span><span class="sxs-lookup"><span data-stu-id="15c93-110">String</span></span>  | <span data-ttu-id="15c93-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="15c93-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="15c93-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="15c93-112">replyChainMessageId</span></span> | <span data-ttu-id="15c93-113">String</span><span class="sxs-lookup"><span data-stu-id="15c93-113">String</span></span>  | <span data-ttu-id="15c93-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="15c93-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="15c93-115">threadId</span><span class="sxs-lookup"><span data-stu-id="15c93-115">threadId</span></span>            | <span data-ttu-id="15c93-116">String</span><span class="sxs-lookup"><span data-stu-id="15c93-116">String</span></span>  | <span data-ttu-id="15c93-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="15c93-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15c93-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15c93-118">JSON representation</span></span>

<span data-ttu-id="15c93-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15c93-119">The following is a JSON representation of the resource.</span></span>

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
