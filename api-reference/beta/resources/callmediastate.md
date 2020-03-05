---
title: callMediaState 资源类型
description: 表示呼叫的媒体状态。
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: c9c55908f62214c386aacee34be76bb11fc318b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507808"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="bfa9e-103">callMediaState 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfa9e-103">callMediaState resource type</span></span>

<span data-ttu-id="bfa9e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bfa9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa9e-105">表示[呼叫](call.md)的媒体状态。</span><span class="sxs-lookup"><span data-stu-id="bfa9e-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bfa9e-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfa9e-106">Properties</span></span>

| <span data-ttu-id="bfa9e-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfa9e-107">Property</span></span>            | <span data-ttu-id="bfa9e-108">类型</span><span class="sxs-lookup"><span data-stu-id="bfa9e-108">Type</span></span>    | <span data-ttu-id="bfa9e-109">说明</span><span class="sxs-lookup"><span data-stu-id="bfa9e-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="bfa9e-110">audio</span><span class="sxs-lookup"><span data-stu-id="bfa9e-110">audio</span></span>           | <span data-ttu-id="bfa9e-111">String</span><span class="sxs-lookup"><span data-stu-id="bfa9e-111">String</span></span>  | <span data-ttu-id="bfa9e-112">音频媒体状态。</span><span class="sxs-lookup"><span data-stu-id="bfa9e-112">The audio media state.</span></span> <span data-ttu-id="bfa9e-113">可取值为：`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="bfa9e-113">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfa9e-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfa9e-114">JSON representation</span></span>

<span data-ttu-id="bfa9e-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfa9e-115">The following is a JSON representation of the resource.</span></span>

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
