---
title: sortProperty 资源类型
description: 提供用于对搜索结果进行排序的选项。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f1288b2dc9ec05fe8aaedb5871c3bda68714f90
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193864"
---
# <a name="sortproperty-resource-type"></a><span data-ttu-id="310dc-103">sortProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="310dc-103">sortProperty resource type</span></span>

<span data-ttu-id="310dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="310dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="310dc-105">表示对搜索结果进行排序的排序选项。</span><span class="sxs-lookup"><span data-stu-id="310dc-105">Represents the sort options to order search results.</span></span>

## <a name="properties"></a><span data-ttu-id="310dc-106">属性</span><span class="sxs-lookup"><span data-stu-id="310dc-106">Properties</span></span>

| <span data-ttu-id="310dc-107">属性</span><span class="sxs-lookup"><span data-stu-id="310dc-107">Property</span></span>     | <span data-ttu-id="310dc-108">类型</span><span class="sxs-lookup"><span data-stu-id="310dc-108">Type</span></span>        | <span data-ttu-id="310dc-109">描述</span><span class="sxs-lookup"><span data-stu-id="310dc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="310dc-110">name</span><span class="sxs-lookup"><span data-stu-id="310dc-110">name</span></span>|<span data-ttu-id="310dc-111">字符串</span><span class="sxs-lookup"><span data-stu-id="310dc-111">String</span></span>|<span data-ttu-id="310dc-112">要对其进行排序的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="310dc-112">The name of the property to sort on.</span></span> <span data-ttu-id="310dc-113">必需。</span><span class="sxs-lookup"><span data-stu-id="310dc-113">Required.</span></span>|
|<span data-ttu-id="310dc-114">isDescending</span><span class="sxs-lookup"><span data-stu-id="310dc-114">isDescending</span></span>|<span data-ttu-id="310dc-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="310dc-115">Boolean</span></span>|<span data-ttu-id="310dc-116">`True` 如果排序次序为降序。</span><span class="sxs-lookup"><span data-stu-id="310dc-116">`True` if the sort order is descending.</span></span> <span data-ttu-id="310dc-117">默认值为 `false` ，排序次序为升序。</span><span class="sxs-lookup"><span data-stu-id="310dc-117">Default is `false`, with the sort order as ascending.</span></span> <span data-ttu-id="310dc-118">可选。</span><span class="sxs-lookup"><span data-stu-id="310dc-118">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="310dc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="310dc-119">JSON representation</span></span>

<span data-ttu-id="310dc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="310dc-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortProperty",
  "baseType": null
}-->

```json
{
  "name": "String",
  "isDescending": "true"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->