---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 29402e813f6816ebea02ad2bb86c403408c2ff81
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006745"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="d02c4-103">callMediaState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d02c4-103">callMediaState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d02c4-104">表示[呼叫](call.md)的媒体状态。</span><span class="sxs-lookup"><span data-stu-id="d02c4-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d02c4-105">属性</span><span class="sxs-lookup"><span data-stu-id="d02c4-105">Properties</span></span>

| <span data-ttu-id="d02c4-106">属性</span><span class="sxs-lookup"><span data-stu-id="d02c4-106">Property</span></span>            | <span data-ttu-id="d02c4-107">类型</span><span class="sxs-lookup"><span data-stu-id="d02c4-107">Type</span></span>    | <span data-ttu-id="d02c4-108">说明</span><span class="sxs-lookup"><span data-stu-id="d02c4-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="d02c4-109">audio</span><span class="sxs-lookup"><span data-stu-id="d02c4-109">audio</span></span>           | <span data-ttu-id="d02c4-110">String</span><span class="sxs-lookup"><span data-stu-id="d02c4-110">String</span></span>  | <span data-ttu-id="d02c4-111">音频媒体状态。</span><span class="sxs-lookup"><span data-stu-id="d02c4-111">The audio media state.</span></span> <span data-ttu-id="d02c4-112">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="d02c4-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d02c4-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d02c4-113">JSON representation</span></span>

<span data-ttu-id="d02c4-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d02c4-114">The following is a JSON representation of the resource.</span></span>

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
