---
title: noMediaConfig 资源类型
description: 指示没有媒体的媒体配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 64ab5c5bb6cbff6d9af677be9c85c13bfcd78d75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983385"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="96c4b-103">noMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="96c4b-103">noMediaConfig resource type</span></span>

> <span data-ttu-id="96c4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="96c4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96c4b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96c4b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96c4b-106">指示没有媒体的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="96c4b-106">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="96c4b-107">属性</span><span class="sxs-lookup"><span data-stu-id="96c4b-107">Properties</span></span>

| <span data-ttu-id="96c4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="96c4b-108">Property</span></span>       | <span data-ttu-id="96c4b-109">类型</span><span class="sxs-lookup"><span data-stu-id="96c4b-109">Type</span></span>    | <span data-ttu-id="96c4b-110">说明</span><span class="sxs-lookup"><span data-stu-id="96c4b-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96c4b-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="96c4b-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="96c4b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="96c4b-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="96c4b-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96c4b-113">JSON representation</span></span>

<span data-ttu-id="96c4b-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96c4b-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
