---
title: 通知资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: c09927cbe133c945b83a3bfc1b0eb74ef00bce2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047929"
---
# <a name="notification-resource-type"></a><span data-ttu-id="16094-103">通知资源类型</span><span class="sxs-lookup"><span data-stu-id="16094-103">notification resource type</span></span>

> <span data-ttu-id="16094-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16094-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16094-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16094-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="16094-106">属性</span><span class="sxs-lookup"><span data-stu-id="16094-106">Properties</span></span>
| <span data-ttu-id="16094-107">属性</span><span class="sxs-lookup"><span data-stu-id="16094-107">Property</span></span>       | <span data-ttu-id="16094-108">类型</span><span class="sxs-lookup"><span data-stu-id="16094-108">Type</span></span>    | <span data-ttu-id="16094-109">说明</span><span class="sxs-lookup"><span data-stu-id="16094-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="16094-110">changeType</span><span class="sxs-lookup"><span data-stu-id="16094-110">changeType</span></span>     | <span data-ttu-id="16094-111">字符串</span><span class="sxs-lookup"><span data-stu-id="16094-111">String</span></span>  | <span data-ttu-id="16094-112">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="16094-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="16094-113">resource</span><span class="sxs-lookup"><span data-stu-id="16094-113">resource</span></span>       | <span data-ttu-id="16094-114">字符串</span><span class="sxs-lookup"><span data-stu-id="16094-114">String</span></span>  | <span data-ttu-id="16094-115">已更改的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="16094-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="16094-116">**注意：**`resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="16094-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="16094-117">它是一个实体或 Collection(entity) 根据打包通知中的更改的次数。</span><span class="sxs-lookup"><span data-stu-id="16094-117">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16094-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16094-118">JSON representation</span></span>

<span data-ttu-id="16094-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16094-119">The following is a JSON representation of the resource.</span></span>

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
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->