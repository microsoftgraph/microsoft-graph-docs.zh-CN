---
title: meetingInfo 资源类型
description: 会议指定要创建或加入会议的信息。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 24ac0247fd39569276f2cb288646eca578447e07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817750"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="d6eb2-103">meetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6eb2-103">meetingInfo resource type</span></span>

> <span data-ttu-id="d6eb2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6eb2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6eb2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6eb2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6eb2-106">会议指定要创建或加入会议的信息。</span><span class="sxs-lookup"><span data-stu-id="d6eb2-106">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d6eb2-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6eb2-107">Properties</span></span>

| <span data-ttu-id="d6eb2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6eb2-108">Property</span></span>       | <span data-ttu-id="d6eb2-109">类型</span><span class="sxs-lookup"><span data-stu-id="d6eb2-109">Type</span></span>    | <span data-ttu-id="d6eb2-110">Description</span><span class="sxs-lookup"><span data-stu-id="d6eb2-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6eb2-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="d6eb2-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="d6eb2-112">布尔</span><span class="sxs-lookup"><span data-stu-id="d6eb2-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="d6eb2-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6eb2-113">JSON representation</span></span>

<span data-ttu-id="d6eb2-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6eb2-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
