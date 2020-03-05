---
title: commsNotification 资源类型
description: 通信服务器发布的用于通知更改的通信通知基类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ec3df8bc56e6164af3b7752333d28bd10665d67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507602"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="9ac7a-103">commsNotification 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ac7a-103">commsNotification resource type</span></span>

<span data-ttu-id="9ac7a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9ac7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac7a-105">通信服务器发布的用于通知更改的通信通知基类型。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-105">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="9ac7a-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ac7a-106">Properties</span></span>
| <span data-ttu-id="9ac7a-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ac7a-107">Property</span></span>       | <span data-ttu-id="9ac7a-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ac7a-108">Type</span></span>    | <span data-ttu-id="9ac7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ac7a-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="9ac7a-110">changeType</span><span class="sxs-lookup"><span data-stu-id="9ac7a-110">changeType</span></span>     | <span data-ttu-id="9ac7a-111">String</span><span class="sxs-lookup"><span data-stu-id="9ac7a-111">String</span></span>  | <span data-ttu-id="9ac7a-112">可取值为：`created`、`updated`、`deleted`。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="9ac7a-113">resourceUrl</span><span class="sxs-lookup"><span data-stu-id="9ac7a-113">resourceUrl</span></span>       | <span data-ttu-id="9ac7a-114">String</span><span class="sxs-lookup"><span data-stu-id="9ac7a-114">String</span></span>  | <span data-ttu-id="9ac7a-115">已更改的资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="9ac7a-116">**注意：** `resourceData`可用作其他数据。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="9ac7a-117">它可以是实体，也可以是实体集合，具体取决于通知中打包的更改数。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-117">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ac7a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ac7a-118">JSON representation</span></span>

<span data-ttu-id="9ac7a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ac7a-119">The following is a JSON representation of the resource.</span></span>

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
