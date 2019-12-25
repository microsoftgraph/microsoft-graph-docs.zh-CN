---
title: mediaStream 资源类型
description: MediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 906eccc7004aaac26dc29948e51e42cfd5e86631
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865778"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="dc3e2-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc3e2-103">mediaStream resource type</span></span>

<span data-ttu-id="dc3e2-104">其中包含媒体通道的相关信息。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-104">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="dc3e2-105">属性</span><span class="sxs-lookup"><span data-stu-id="dc3e2-105">Properties</span></span>

| <span data-ttu-id="dc3e2-106">属性</span><span class="sxs-lookup"><span data-stu-id="dc3e2-106">Property</span></span>    | <span data-ttu-id="dc3e2-107">类型</span><span class="sxs-lookup"><span data-stu-id="dc3e2-107">Type</span></span>    | <span data-ttu-id="dc3e2-108">说明</span><span class="sxs-lookup"><span data-stu-id="dc3e2-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="dc3e2-109">direction</span><span class="sxs-lookup"><span data-stu-id="dc3e2-109">direction</span></span>   | <span data-ttu-id="dc3e2-110">String</span><span class="sxs-lookup"><span data-stu-id="dc3e2-110">String</span></span>  | <span data-ttu-id="dc3e2-111">方向。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-111">The direction.</span></span> <span data-ttu-id="dc3e2-112">可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="dc3e2-113">label</span><span class="sxs-lookup"><span data-stu-id="dc3e2-113">label</span></span>       | <span data-ttu-id="dc3e2-114">String</span><span class="sxs-lookup"><span data-stu-id="dc3e2-114">String</span></span>  | <span data-ttu-id="dc3e2-115">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="dc3e2-116">群组</span><span class="sxs-lookup"><span data-stu-id="dc3e2-116">mediaType</span></span>   | <span data-ttu-id="dc3e2-117">String</span><span class="sxs-lookup"><span data-stu-id="dc3e2-117">String</span></span>  | <span data-ttu-id="dc3e2-118">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-118">The media type.</span></span> <span data-ttu-id="dc3e2-119">可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="dc3e2-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="dc3e2-120">serverMuted</span></span> | <span data-ttu-id="dc3e2-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc3e2-121">Boolean</span></span> | <span data-ttu-id="dc3e2-122">如果服务器已将媒体设为静音。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="dc3e2-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="dc3e2-123">sourceId</span></span>    | <span data-ttu-id="dc3e2-124">String</span><span class="sxs-lookup"><span data-stu-id="dc3e2-124">String</span></span>  | <span data-ttu-id="dc3e2-125">源 ID。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="dc3e2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc3e2-126">JSON representation</span></span>

<span data-ttu-id="dc3e2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc3e2-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
