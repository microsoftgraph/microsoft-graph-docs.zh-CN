---
title: commsNotification 资源类型
description: 通信，请通知发布 Communications 服务器以更改通知的基类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 526ed88f4b1c5983a06b1830f5c0b0bb97cc874e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837147"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="ac3b4-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac3b4-103">commsNotification resource type</span></span>

> <span data-ttu-id="ac3b4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac3b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac3b4-106">通信，请通知发布 Communications 服务器以更改通知的基类型。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="ac3b4-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac3b4-107">Properties</span></span>
| <span data-ttu-id="ac3b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac3b4-108">Property</span></span>       | <span data-ttu-id="ac3b4-109">类型</span><span class="sxs-lookup"><span data-stu-id="ac3b4-109">Type</span></span>    | <span data-ttu-id="ac3b4-110">说明</span><span class="sxs-lookup"><span data-stu-id="ac3b4-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="ac3b4-111">changeType</span><span class="sxs-lookup"><span data-stu-id="ac3b4-111">changeType</span></span>     | <span data-ttu-id="ac3b4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ac3b4-112">String</span></span>  | <span data-ttu-id="ac3b4-113">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="ac3b4-114">resource</span><span class="sxs-lookup"><span data-stu-id="ac3b4-114">resource</span></span>       | <span data-ttu-id="ac3b4-115">字符串</span><span class="sxs-lookup"><span data-stu-id="ac3b4-115">String</span></span>  | <span data-ttu-id="ac3b4-116">已更改的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="ac3b4-117">**注意：**`resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="ac3b4-118">它是一个实体或 Collection(entity) 根据打包通知中的更改的次数。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac3b4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac3b4-119">JSON representation</span></span>

<span data-ttu-id="ac3b4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac3b4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
