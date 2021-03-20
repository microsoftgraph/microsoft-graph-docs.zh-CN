---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: f8797aadf7e35000d799c4c8b879ef2ed6da6409
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952534"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="ad1a5-103">callMediaState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad1a5-103">callMediaState resource type</span></span>

<span data-ttu-id="ad1a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad1a5-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ad1a5-105">表示呼叫的媒体 [状态](call.md)。</span><span class="sxs-lookup"><span data-stu-id="ad1a5-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ad1a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad1a5-106">Properties</span></span>

| <span data-ttu-id="ad1a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad1a5-107">Property</span></span>            | <span data-ttu-id="ad1a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="ad1a5-108">Type</span></span>    | <span data-ttu-id="ad1a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad1a5-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="ad1a5-110">audio</span><span class="sxs-lookup"><span data-stu-id="ad1a5-110">audio</span></span>           | <span data-ttu-id="ad1a5-111">mediaState</span><span class="sxs-lookup"><span data-stu-id="ad1a5-111">mediaState</span></span>  | <span data-ttu-id="ad1a5-112">音频媒体状态。</span><span class="sxs-lookup"><span data-stu-id="ad1a5-112">The audio media state.</span></span> <span data-ttu-id="ad1a5-113">可取值为：`active`、`inactive`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ad1a5-113">Possible values are: `active`, `inactive`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad1a5-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad1a5-114">JSON representation</span></span>

<span data-ttu-id="ad1a5-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad1a5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

