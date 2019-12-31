---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7d94b7462c50ca5a9304a2c4c320f6e244815373
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913245"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="e22fe-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="e22fe-103">commsNotification resource type</span></span>

<span data-ttu-id="e22fe-104">通信服务器发布的用于通知更改的通信通知基类型。</span><span class="sxs-lookup"><span data-stu-id="e22fe-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="e22fe-105">属性</span><span class="sxs-lookup"><span data-stu-id="e22fe-105">Properties</span></span>
| <span data-ttu-id="e22fe-106">属性</span><span class="sxs-lookup"><span data-stu-id="e22fe-106">Property</span></span>       | <span data-ttu-id="e22fe-107">类型</span><span class="sxs-lookup"><span data-stu-id="e22fe-107">Type</span></span>    | <span data-ttu-id="e22fe-108">说明</span><span class="sxs-lookup"><span data-stu-id="e22fe-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="e22fe-109">changeType</span><span class="sxs-lookup"><span data-stu-id="e22fe-109">changeType</span></span>     | <span data-ttu-id="e22fe-110">String</span><span class="sxs-lookup"><span data-stu-id="e22fe-110">String</span></span>  | <span data-ttu-id="e22fe-111">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="e22fe-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="e22fe-112">resourceUrl</span><span class="sxs-lookup"><span data-stu-id="e22fe-112">resourceUrl</span></span>       | <span data-ttu-id="e22fe-113">String</span><span class="sxs-lookup"><span data-stu-id="e22fe-113">String</span></span>  | <span data-ttu-id="e22fe-114">已更改的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="e22fe-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="e22fe-115">**注意：** `resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="e22fe-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="e22fe-116">它可以是实体，也可以是实体集合，具体取决于通知中打包的更改数。</span><span class="sxs-lookup"><span data-stu-id="e22fe-116">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e22fe-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e22fe-117">JSON representation</span></span>

<span data-ttu-id="e22fe-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e22fe-118">The following is a JSON representation of the resource.</span></span>

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
