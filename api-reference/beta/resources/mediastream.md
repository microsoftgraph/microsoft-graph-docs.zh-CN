---
title: mediaStream 资源类型
description: mediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69d8088ba161bdf4dbf0482fdab8ad757347126d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342616"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="c29cb-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="c29cb-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c29cb-104">mediaStream 类型。</span><span class="sxs-lookup"><span data-stu-id="c29cb-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="c29cb-105">属性</span><span class="sxs-lookup"><span data-stu-id="c29cb-105">Properties</span></span>

| <span data-ttu-id="c29cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="c29cb-106">Property</span></span>    | <span data-ttu-id="c29cb-107">类型</span><span class="sxs-lookup"><span data-stu-id="c29cb-107">Type</span></span>    | <span data-ttu-id="c29cb-108">说明</span><span class="sxs-lookup"><span data-stu-id="c29cb-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c29cb-109">direction</span><span class="sxs-lookup"><span data-stu-id="c29cb-109">direction</span></span>   | <span data-ttu-id="c29cb-110">String</span><span class="sxs-lookup"><span data-stu-id="c29cb-110">String</span></span>  | <span data-ttu-id="c29cb-111">方向。</span><span class="sxs-lookup"><span data-stu-id="c29cb-111">The direction.</span></span> <span data-ttu-id="c29cb-112">可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="c29cb-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="c29cb-113">label</span><span class="sxs-lookup"><span data-stu-id="c29cb-113">label</span></span>       | <span data-ttu-id="c29cb-114">String</span><span class="sxs-lookup"><span data-stu-id="c29cb-114">String</span></span>  | <span data-ttu-id="c29cb-115">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="c29cb-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="c29cb-116">群组</span><span class="sxs-lookup"><span data-stu-id="c29cb-116">mediaType</span></span>   | <span data-ttu-id="c29cb-117">String</span><span class="sxs-lookup"><span data-stu-id="c29cb-117">String</span></span>  | <span data-ttu-id="c29cb-118">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="c29cb-118">The media type.</span></span> <span data-ttu-id="c29cb-119">可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。</span><span class="sxs-lookup"><span data-stu-id="c29cb-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="c29cb-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="c29cb-120">serverMuted</span></span> | <span data-ttu-id="c29cb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c29cb-121">Boolean</span></span> | <span data-ttu-id="c29cb-122">如果服务器已将媒体设为静音。</span><span class="sxs-lookup"><span data-stu-id="c29cb-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="c29cb-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="c29cb-123">sourceId</span></span>    | <span data-ttu-id="c29cb-124">String</span><span class="sxs-lookup"><span data-stu-id="c29cb-124">String</span></span>  | <span data-ttu-id="c29cb-125">源 ID。</span><span class="sxs-lookup"><span data-stu-id="c29cb-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="c29cb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c29cb-126">JSON representation</span></span>

<span data-ttu-id="c29cb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c29cb-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
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

## <a name="example"></a><span data-ttu-id="c29cb-128">示例</span><span class="sxs-lookup"><span data-stu-id="c29cb-128">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
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
