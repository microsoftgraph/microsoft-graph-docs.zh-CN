---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c15720ac3f2bda673d495fbe32dc6bae8d5898d7
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844496"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="eb69d-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb69d-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb69d-104">包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="eb69d-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb69d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb69d-105">JSON representation</span></span>

<span data-ttu-id="eb69d-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb69d-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="eb69d-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb69d-107">Properties</span></span>

| <span data-ttu-id="eb69d-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb69d-108">Property</span></span>      | <span data-ttu-id="eb69d-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb69d-109">Type</span></span>      | <span data-ttu-id="eb69d-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb69d-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="eb69d-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="eb69d-111">webUrl</span></span>        | <span data-ttu-id="eb69d-112">String</span><span class="sxs-lookup"><span data-stu-id="eb69d-112">String</span></span>    | <span data-ttu-id="eb69d-113">指向引用项的 URL。</span><span class="sxs-lookup"><span data-stu-id="eb69d-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="eb69d-114">id</span><span class="sxs-lookup"><span data-stu-id="eb69d-114">id</span></span>            | <span data-ttu-id="eb69d-115">String</span><span class="sxs-lookup"><span data-stu-id="eb69d-115">String</span></span>    | <span data-ttu-id="eb69d-116">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eb69d-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="eb69d-117">type</span><span class="sxs-lookup"><span data-stu-id="eb69d-117">type</span></span>          | <span data-ttu-id="eb69d-118">String</span><span class="sxs-lookup"><span data-stu-id="eb69d-118">String</span></span>    | <span data-ttu-id="eb69d-119">一个可用于对项目进行分类的字符串值，例如 "driveItem"</span><span class="sxs-lookup"><span data-stu-id="eb69d-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
