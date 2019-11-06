---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1cf5dc67aa4a3db8b495f8942f64e05ba0bbc6a4
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006717"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="d6366-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6366-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6366-104">有关 Microsoft 团队中的邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="d6366-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="d6366-105">属性</span><span class="sxs-lookup"><span data-stu-id="d6366-105">Properties</span></span>

| <span data-ttu-id="d6366-106">属性</span><span class="sxs-lookup"><span data-stu-id="d6366-106">Property</span></span>            | <span data-ttu-id="d6366-107">类型</span><span class="sxs-lookup"><span data-stu-id="d6366-107">Type</span></span>    | <span data-ttu-id="d6366-108">说明</span><span class="sxs-lookup"><span data-stu-id="d6366-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="d6366-109">messageId</span><span class="sxs-lookup"><span data-stu-id="d6366-109">messageId</span></span>           | <span data-ttu-id="d6366-110">String</span><span class="sxs-lookup"><span data-stu-id="d6366-110">String</span></span>  | <span data-ttu-id="d6366-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d6366-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="d6366-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="d6366-112">replyChainMessageId</span></span> | <span data-ttu-id="d6366-113">String</span><span class="sxs-lookup"><span data-stu-id="d6366-113">String</span></span>  | <span data-ttu-id="d6366-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="d6366-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="d6366-115">threadId</span><span class="sxs-lookup"><span data-stu-id="d6366-115">threadId</span></span>            | <span data-ttu-id="d6366-116">String</span><span class="sxs-lookup"><span data-stu-id="d6366-116">String</span></span>  | <span data-ttu-id="d6366-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d6366-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6366-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6366-118">JSON representation</span></span>

<span data-ttu-id="d6366-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6366-119">The following is a JSON representation of the resource.</span></span>

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
