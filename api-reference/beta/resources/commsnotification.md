---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20b99493821cfb29898ff0c9517cceecba1d389c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341373"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="54d0c-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="54d0c-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54d0c-104">通信服务器发布的用于通知更改的通信通知基类型。</span><span class="sxs-lookup"><span data-stu-id="54d0c-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="54d0c-105">属性</span><span class="sxs-lookup"><span data-stu-id="54d0c-105">Properties</span></span>
| <span data-ttu-id="54d0c-106">属性</span><span class="sxs-lookup"><span data-stu-id="54d0c-106">Property</span></span>       | <span data-ttu-id="54d0c-107">类型</span><span class="sxs-lookup"><span data-stu-id="54d0c-107">Type</span></span>    | <span data-ttu-id="54d0c-108">说明</span><span class="sxs-lookup"><span data-stu-id="54d0c-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="54d0c-109">changeType</span><span class="sxs-lookup"><span data-stu-id="54d0c-109">changeType</span></span>     | <span data-ttu-id="54d0c-110">String</span><span class="sxs-lookup"><span data-stu-id="54d0c-110">String</span></span>  | <span data-ttu-id="54d0c-111">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="54d0c-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="54d0c-112">resource</span><span class="sxs-lookup"><span data-stu-id="54d0c-112">resource</span></span>       | <span data-ttu-id="54d0c-113">String</span><span class="sxs-lookup"><span data-stu-id="54d0c-113">String</span></span>  | <span data-ttu-id="54d0c-114">已更改的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="54d0c-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="54d0c-115">**注意:**`resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="54d0c-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="54d0c-116">它是一个实体或集合 (实体), 具体取决于通知中打包的更改的数量。</span><span class="sxs-lookup"><span data-stu-id="54d0c-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54d0c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54d0c-117">JSON representation</span></span>

<span data-ttu-id="54d0c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54d0c-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
