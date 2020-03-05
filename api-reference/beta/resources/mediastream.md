---
title: mediaStream 资源类型
description: 包含媒体通道的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d6bce42c31e39f5b36e3beccdac2fc660f9cb30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522755"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="3bd37-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bd37-103">mediaStream resource type</span></span>

<span data-ttu-id="3bd37-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3bd37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd37-105">包含媒体通道的相关信息。</span><span class="sxs-lookup"><span data-stu-id="3bd37-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="3bd37-106">属性</span><span class="sxs-lookup"><span data-stu-id="3bd37-106">Properties</span></span>

| <span data-ttu-id="3bd37-107">属性</span><span class="sxs-lookup"><span data-stu-id="3bd37-107">Property</span></span>    | <span data-ttu-id="3bd37-108">类型</span><span class="sxs-lookup"><span data-stu-id="3bd37-108">Type</span></span>    | <span data-ttu-id="3bd37-109">说明</span><span class="sxs-lookup"><span data-stu-id="3bd37-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="3bd37-110">direction</span><span class="sxs-lookup"><span data-stu-id="3bd37-110">direction</span></span>   | <span data-ttu-id="3bd37-111">String</span><span class="sxs-lookup"><span data-stu-id="3bd37-111">String</span></span>  | <span data-ttu-id="3bd37-112">方向。</span><span class="sxs-lookup"><span data-stu-id="3bd37-112">The direction.</span></span> <span data-ttu-id="3bd37-113">可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="3bd37-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="3bd37-114">label</span><span class="sxs-lookup"><span data-stu-id="3bd37-114">label</span></span>       | <span data-ttu-id="3bd37-115">String</span><span class="sxs-lookup"><span data-stu-id="3bd37-115">String</span></span>  | <span data-ttu-id="3bd37-116">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="3bd37-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="3bd37-117">群组</span><span class="sxs-lookup"><span data-stu-id="3bd37-117">mediaType</span></span>   | <span data-ttu-id="3bd37-118">String</span><span class="sxs-lookup"><span data-stu-id="3bd37-118">String</span></span>  | <span data-ttu-id="3bd37-119">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="3bd37-119">The media type.</span></span> <span data-ttu-id="3bd37-120">可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。</span><span class="sxs-lookup"><span data-stu-id="3bd37-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="3bd37-121">serverMuted</span><span class="sxs-lookup"><span data-stu-id="3bd37-121">serverMuted</span></span> | <span data-ttu-id="3bd37-122">布尔</span><span class="sxs-lookup"><span data-stu-id="3bd37-122">Boolean</span></span> | <span data-ttu-id="3bd37-123">指示服务器是否静音媒体。</span><span class="sxs-lookup"><span data-stu-id="3bd37-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="3bd37-124">sourceId</span><span class="sxs-lookup"><span data-stu-id="3bd37-124">sourceId</span></span>    | <span data-ttu-id="3bd37-125">String</span><span class="sxs-lookup"><span data-stu-id="3bd37-125">String</span></span>  | <span data-ttu-id="3bd37-126">源 ID。</span><span class="sxs-lookup"><span data-stu-id="3bd37-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="3bd37-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bd37-127">JSON representation</span></span>

<span data-ttu-id="3bd37-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bd37-128">The following is a JSON representation of the resource.</span></span>

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
