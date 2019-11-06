---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9901c1390d1813413cdd95949debea95d54c286b
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006703"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="4f4c5-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f4c5-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4c5-104">通信服务器发布的用于通知更改的通信通知基类型。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="4f4c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="4f4c5-105">Properties</span></span>
| <span data-ttu-id="4f4c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f4c5-106">Property</span></span>       | <span data-ttu-id="4f4c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="4f4c5-107">Type</span></span>    | <span data-ttu-id="4f4c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="4f4c5-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="4f4c5-109">changeType</span><span class="sxs-lookup"><span data-stu-id="4f4c5-109">changeType</span></span>     | <span data-ttu-id="4f4c5-110">String</span><span class="sxs-lookup"><span data-stu-id="4f4c5-110">String</span></span>  | <span data-ttu-id="4f4c5-111">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="4f4c5-112">resourceUrl</span><span class="sxs-lookup"><span data-stu-id="4f4c5-112">resourceUrl</span></span>       | <span data-ttu-id="4f4c5-113">String</span><span class="sxs-lookup"><span data-stu-id="4f4c5-113">String</span></span>  | <span data-ttu-id="4f4c5-114">已更改的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="4f4c5-115">**注意：** `resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="4f4c5-116">它是一个实体或集合（实体），具体取决于通知中打包的更改的数量。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f4c5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f4c5-117">JSON representation</span></span>

<span data-ttu-id="4f4c5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f4c5-118">The following is a JSON representation of the resource.</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
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
