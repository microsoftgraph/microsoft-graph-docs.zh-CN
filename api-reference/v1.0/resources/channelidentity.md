---
title: channelIdentity 资源类型
description: 表示 Microsoft Teams 中频道的标识。
author: Kanaka
doc_type: resourcePageType
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: 866469745a4dd3aaf7b22c2a6710e327992e9fee
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582892"
---
# <a name="channelidentity-resource-type"></a><span data-ttu-id="32307-103">channelIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="32307-103">channelIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="32307-104">包含有关 Microsoft Teams 中频道的基本标识信息。</span><span class="sxs-lookup"><span data-stu-id="32307-104">Contains basic identification information about a channel in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="32307-105">属性</span><span class="sxs-lookup"><span data-stu-id="32307-105">Properties</span></span>

| <span data-ttu-id="32307-106">属性</span><span class="sxs-lookup"><span data-stu-id="32307-106">Property</span></span>   | <span data-ttu-id="32307-107">类型</span><span class="sxs-lookup"><span data-stu-id="32307-107">Type</span></span> |<span data-ttu-id="32307-108">说明</span><span class="sxs-lookup"><span data-stu-id="32307-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32307-109">channelId</span><span class="sxs-lookup"><span data-stu-id="32307-109">channelId</span></span>|<span data-ttu-id="32307-110">string</span><span class="sxs-lookup"><span data-stu-id="32307-110">string</span></span>|  <span data-ttu-id="32307-111">发布消息的频道的标识。</span><span class="sxs-lookup"><span data-stu-id="32307-111">The identity of the channel in which the message was posted.</span></span>|
|<span data-ttu-id="32307-112">teamId</span><span class="sxs-lookup"><span data-stu-id="32307-112">teamId</span></span>|<span data-ttu-id="32307-113">string</span><span class="sxs-lookup"><span data-stu-id="32307-113">string</span></span>|  <span data-ttu-id="32307-114">发布邮件的团队的标识。</span><span class="sxs-lookup"><span data-stu-id="32307-114">The identity of the team in which the message was posted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32307-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32307-115">JSON representation</span></span>

<span data-ttu-id="32307-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32307-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.channelIdentity"
}-->

```json
{
  "channelId": "string",
  "teamId": "string",
  
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
