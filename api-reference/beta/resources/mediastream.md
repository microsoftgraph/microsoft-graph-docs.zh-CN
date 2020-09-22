---
title: mediaStream 资源类型
description: 包含媒体通道的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37ed8ce10f62888a7bf1be67f489c6b8a0b95c76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971732"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="78e11-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="78e11-103">mediaStream resource type</span></span>

<span data-ttu-id="78e11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78e11-105">包含媒体通道的相关信息。</span><span class="sxs-lookup"><span data-stu-id="78e11-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="78e11-106">属性</span><span class="sxs-lookup"><span data-stu-id="78e11-106">Properties</span></span>

| <span data-ttu-id="78e11-107">属性</span><span class="sxs-lookup"><span data-stu-id="78e11-107">Property</span></span>    | <span data-ttu-id="78e11-108">类型</span><span class="sxs-lookup"><span data-stu-id="78e11-108">Type</span></span>    | <span data-ttu-id="78e11-109">说明</span><span class="sxs-lookup"><span data-stu-id="78e11-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="78e11-110">direction</span><span class="sxs-lookup"><span data-stu-id="78e11-110">direction</span></span>   | <span data-ttu-id="78e11-111">String</span><span class="sxs-lookup"><span data-stu-id="78e11-111">String</span></span>  | <span data-ttu-id="78e11-112">方向。</span><span class="sxs-lookup"><span data-stu-id="78e11-112">The direction.</span></span> <span data-ttu-id="78e11-113">可能的值为 `inactive` 、 `sendOnly` 、 `receiveOnly` 、 `sendReceive` 。</span><span class="sxs-lookup"><span data-stu-id="78e11-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="78e11-114">label</span><span class="sxs-lookup"><span data-stu-id="78e11-114">label</span></span>       | <span data-ttu-id="78e11-115">String</span><span class="sxs-lookup"><span data-stu-id="78e11-115">String</span></span>  | <span data-ttu-id="78e11-116">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="78e11-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="78e11-117">mediaType</span><span class="sxs-lookup"><span data-stu-id="78e11-117">mediaType</span></span>   | <span data-ttu-id="78e11-118">String</span><span class="sxs-lookup"><span data-stu-id="78e11-118">String</span></span>  | <span data-ttu-id="78e11-119">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="78e11-119">The media type.</span></span> <span data-ttu-id="78e11-120">可能的值为 `unknown` 、、、 `audio` `video` `videoBasedScreenSharing` `data` 。</span><span class="sxs-lookup"><span data-stu-id="78e11-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="78e11-121">serverMuted</span><span class="sxs-lookup"><span data-stu-id="78e11-121">serverMuted</span></span> | <span data-ttu-id="78e11-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="78e11-122">Boolean</span></span> | <span data-ttu-id="78e11-123">指示服务器是否静音媒体。</span><span class="sxs-lookup"><span data-stu-id="78e11-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="78e11-124">sourceId</span><span class="sxs-lookup"><span data-stu-id="78e11-124">sourceId</span></span>    | <span data-ttu-id="78e11-125">String</span><span class="sxs-lookup"><span data-stu-id="78e11-125">String</span></span>  | <span data-ttu-id="78e11-126">源 ID。</span><span class="sxs-lookup"><span data-stu-id="78e11-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="78e11-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78e11-127">JSON representation</span></span>

<span data-ttu-id="78e11-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78e11-128">The following is a JSON representation of the resource.</span></span>

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


