---
title: commsNotifications 资源类型
description: Communications server 用于在单一批次中发送多个通知的通知的列表。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9ce629e17c85806d7e05bce99d6a62f9fa9cbff8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851497"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="61643-103">commsNotifications 资源类型</span><span class="sxs-lookup"><span data-stu-id="61643-103">commsNotifications resource type</span></span>

> <span data-ttu-id="61643-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="61643-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61643-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61643-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61643-106">Communications server 用于在单一批次中发送多个通知的通知的列表。</span><span class="sxs-lookup"><span data-stu-id="61643-106">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="61643-107">属性</span><span class="sxs-lookup"><span data-stu-id="61643-107">Properties</span></span>

| <span data-ttu-id="61643-108">属性</span><span class="sxs-lookup"><span data-stu-id="61643-108">Property</span></span>       | <span data-ttu-id="61643-109">类型</span><span class="sxs-lookup"><span data-stu-id="61643-109">Type</span></span>                                                 | <span data-ttu-id="61643-110">说明</span><span class="sxs-lookup"><span data-stu-id="61643-110">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="61643-111">value</span><span class="sxs-lookup"><span data-stu-id="61643-111">value</span></span>          | <span data-ttu-id="61643-112">[commsNotification](commsnotification.md)集合</span><span class="sxs-lookup"><span data-stu-id="61643-112">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="61643-113">资源中更改的通知。</span><span class="sxs-lookup"><span data-stu-id="61643-113">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61643-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61643-114">JSON representation</span></span>

<span data-ttu-id="61643-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61643-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
