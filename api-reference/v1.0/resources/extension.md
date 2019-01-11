---
title: 扩展资源类型
description: 用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。
localization_priority: Normal
ms.openlocfilehash: 2633c8a28c1be1a670a80834ce869b5156fc1de9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834669"
---
# <a name="extension-resource-type"></a><span data-ttu-id="0c28d-103">扩展资源类型</span><span class="sxs-lookup"><span data-stu-id="0c28d-103">extension resource type</span></span>

<span data-ttu-id="0c28d-104">用以支持 OData v4 开放类型 [openTypeExtension](opentypeextension.md) 的抽象类型。</span><span class="sxs-lookup"><span data-stu-id="0c28d-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c28d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c28d-105">JSON representation</span></span>

<span data-ttu-id="0c28d-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c28d-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="0c28d-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c28d-107">Properties</span></span>
| <span data-ttu-id="0c28d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c28d-108">Property</span></span>     | <span data-ttu-id="0c28d-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c28d-109">Type</span></span>   |<span data-ttu-id="0c28d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c28d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c28d-111">id</span><span class="sxs-lookup"><span data-stu-id="0c28d-111">id</span></span>|<span data-ttu-id="0c28d-112">String</span><span class="sxs-lookup"><span data-stu-id="0c28d-112">String</span></span>| <span data-ttu-id="0c28d-113">只读。</span><span class="sxs-lookup"><span data-stu-id="0c28d-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c28d-114">Relationships</span><span class="sxs-lookup"><span data-stu-id="0c28d-114">Relationships</span></span>
<span data-ttu-id="0c28d-115">无</span><span class="sxs-lookup"><span data-stu-id="0c28d-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="0c28d-116">方法</span><span class="sxs-lookup"><span data-stu-id="0c28d-116">Methods</span></span>

<span data-ttu-id="0c28d-117">请参阅派生类型 [openTypeExtension](opentypeextension.md) 的方法以了解实际支持的方法。</span><span class="sxs-lookup"><span data-stu-id="0c28d-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
