---
title: mediaStream 资源类型
description: MediaStream 类型。
author: VinodRavichandran
ms.openlocfilehash: f870611700289f0254272b78e18e344d02dd123e
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380294"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="6ca58-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ca58-103">mediaStream resource type</span></span>

> <span data-ttu-id="6ca58-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ca58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ca58-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ca58-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ca58-106">MediaStream 类型。</span><span class="sxs-lookup"><span data-stu-id="6ca58-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="6ca58-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ca58-107">Properties</span></span>

| <span data-ttu-id="6ca58-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ca58-108">Property</span></span>    | <span data-ttu-id="6ca58-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ca58-109">Type</span></span>    | <span data-ttu-id="6ca58-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ca58-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="6ca58-111">方向</span><span class="sxs-lookup"><span data-stu-id="6ca58-111">direction</span></span>   | <span data-ttu-id="6ca58-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca58-112">String</span></span>  | <span data-ttu-id="6ca58-113">方向。</span><span class="sxs-lookup"><span data-stu-id="6ca58-113">The direction.</span></span> <span data-ttu-id="6ca58-114">可能的值为`inactive`， `sendOnly`， `receiveOnly`， `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="6ca58-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="6ca58-115">标签</span><span class="sxs-lookup"><span data-stu-id="6ca58-115">label</span></span>       | <span data-ttu-id="6ca58-116">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca58-116">String</span></span>  | <span data-ttu-id="6ca58-117">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="6ca58-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="6ca58-118">媒体类型</span><span class="sxs-lookup"><span data-stu-id="6ca58-118">mediaType</span></span>   | <span data-ttu-id="6ca58-119">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca58-119">String</span></span>  | <span data-ttu-id="6ca58-120">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="6ca58-120">The media type.</span></span> <span data-ttu-id="6ca58-121">可能的值是`unknown`， `audio`， `video`， `videoBasedScreenSharing`， `data`。</span><span class="sxs-lookup"><span data-stu-id="6ca58-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="6ca58-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="6ca58-122">serverMuted</span></span> | <span data-ttu-id="6ca58-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ca58-123">Boolean</span></span> | <span data-ttu-id="6ca58-124">如果媒体服务器将设为静音。</span><span class="sxs-lookup"><span data-stu-id="6ca58-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="6ca58-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="6ca58-125">sourceId</span></span>    | <span data-ttu-id="6ca58-126">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca58-126">String</span></span>  | <span data-ttu-id="6ca58-127">源 id。</span><span class="sxs-lookup"><span data-stu-id="6ca58-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="6ca58-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ca58-128">JSON representation</span></span>

<span data-ttu-id="6ca58-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ca58-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="6ca58-130">示例</span><span class="sxs-lookup"><span data-stu-id="6ca58-130">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
