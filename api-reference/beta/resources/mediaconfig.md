---
title: mediaConfig 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: a04670d4c13299bde00c3812b9ecb996885330d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041780"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="1d075-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d075-103">mediaConfig resource type</span></span>

> <span data-ttu-id="1d075-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1d075-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d075-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d075-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="1d075-106">属性</span><span class="sxs-lookup"><span data-stu-id="1d075-106">Properties</span></span>

| <span data-ttu-id="1d075-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d075-107">Property</span></span>       | <span data-ttu-id="1d075-108">类型</span><span class="sxs-lookup"><span data-stu-id="1d075-108">Type</span></span>    | <span data-ttu-id="1d075-109">说明</span><span class="sxs-lookup"><span data-stu-id="1d075-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d075-110">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="1d075-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="1d075-111">布尔</span><span class="sxs-lookup"><span data-stu-id="1d075-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="1d075-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d075-112">JSON representation</span></span>

<span data-ttu-id="1d075-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d075-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->