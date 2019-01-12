---
title: commsNotification 资源类型
description: 通信，请通知发布 Communications 服务器以更改通知的基类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e5b929997cf17d13043264d42421418321aae84e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977694"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="fdf23-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdf23-103">commsNotification resource type</span></span>

> <span data-ttu-id="fdf23-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fdf23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf23-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fdf23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdf23-106">通信，请通知发布 Communications 服务器以更改通知的基类型。</span><span class="sxs-lookup"><span data-stu-id="fdf23-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="fdf23-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdf23-107">Properties</span></span>
| <span data-ttu-id="fdf23-108">属性</span><span class="sxs-lookup"><span data-stu-id="fdf23-108">Property</span></span>       | <span data-ttu-id="fdf23-109">类型</span><span class="sxs-lookup"><span data-stu-id="fdf23-109">Type</span></span>    | <span data-ttu-id="fdf23-110">说明</span><span class="sxs-lookup"><span data-stu-id="fdf23-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="fdf23-111">changeType</span><span class="sxs-lookup"><span data-stu-id="fdf23-111">changeType</span></span>     | <span data-ttu-id="fdf23-112">字符串</span><span class="sxs-lookup"><span data-stu-id="fdf23-112">String</span></span>  | <span data-ttu-id="fdf23-113">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="fdf23-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="fdf23-114">resource</span><span class="sxs-lookup"><span data-stu-id="fdf23-114">resource</span></span>       | <span data-ttu-id="fdf23-115">字符串</span><span class="sxs-lookup"><span data-stu-id="fdf23-115">String</span></span>  | <span data-ttu-id="fdf23-116">已更改的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="fdf23-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="fdf23-117">**注意：**`resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="fdf23-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="fdf23-118">它是一个实体或 Collection(entity) 根据打包通知中的更改的次数。</span><span class="sxs-lookup"><span data-stu-id="fdf23-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdf23-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdf23-119">JSON representation</span></span>

<span data-ttu-id="fdf23-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdf23-120">The following is a JSON representation of the resource.</span></span>

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
