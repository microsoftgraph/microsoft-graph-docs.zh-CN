---
title: 通知资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049164"
---
# <a name="notifications-resource-type"></a><span data-ttu-id="a6e09-103">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="a6e09-103">notifications resource type</span></span>

> <span data-ttu-id="a6e09-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6e09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6e09-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6e09-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="a6e09-106">属性</span><span class="sxs-lookup"><span data-stu-id="a6e09-106">Properties</span></span>

| <span data-ttu-id="a6e09-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6e09-107">Property</span></span>       | <span data-ttu-id="a6e09-108">类型</span><span class="sxs-lookup"><span data-stu-id="a6e09-108">Type</span></span>                                       | <span data-ttu-id="a6e09-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6e09-109">Description</span></span> |
|:---------------|:-------------------------------------------|:------------|
| <span data-ttu-id="a6e09-110">value</span><span class="sxs-lookup"><span data-stu-id="a6e09-110">value</span></span>          | <span data-ttu-id="a6e09-111">[通知](commsnotification.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6e09-111">[notification](commsnotification.md) collection</span></span> | <span data-ttu-id="a6e09-112">资源中更改的通知。</span><span class="sxs-lookup"><span data-stu-id="a6e09-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6e09-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6e09-113">JSON representation</span></span>

<span data-ttu-id="a6e09-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6e09-114">The following is a JSON representation of the resource.</span></span>

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
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->