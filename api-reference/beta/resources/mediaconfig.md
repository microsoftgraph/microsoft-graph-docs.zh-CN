---
title: mediaConfig 资源类型
description: 用于连接到呼叫的媒体配置。
author: VinodRavichandran
ms.openlocfilehash: 1b68d9236ba78ae1a83228b3382c96fc81516d1f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380259"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="968db-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="968db-103">mediaConfig resource type</span></span>

> <span data-ttu-id="968db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="968db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="968db-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="968db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="968db-106">用于连接到呼叫的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="968db-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="968db-107">属性</span><span class="sxs-lookup"><span data-stu-id="968db-107">Properties</span></span>

| <span data-ttu-id="968db-108">属性</span><span class="sxs-lookup"><span data-stu-id="968db-108">Property</span></span>       | <span data-ttu-id="968db-109">类型</span><span class="sxs-lookup"><span data-stu-id="968db-109">Type</span></span>    | <span data-ttu-id="968db-110">说明</span><span class="sxs-lookup"><span data-stu-id="968db-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="968db-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="968db-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="968db-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="968db-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="968db-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="968db-113">JSON representation</span></span>

<span data-ttu-id="968db-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="968db-114">The following is a JSON representation of the resource.</span></span>

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