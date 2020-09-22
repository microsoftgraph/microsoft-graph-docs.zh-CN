---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a353eb07c1aeb2fd904b9f97c8307ed0b5190470
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021852"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d9fb6-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9fb6-103">resourceReference resource type</span></span>

<span data-ttu-id="d9fb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9fb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9fb6-105">包含[itemInsights](iteminsights.md)的属性的复杂类型</span><span class="sxs-lookup"><span data-stu-id="d9fb6-105">Complex type containing properties of [itemInsights](iteminsights.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9fb6-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9fb6-106">JSON representation</span></span>

<span data-ttu-id="d9fb6-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9fb6-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="d9fb6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9fb6-108">Properties</span></span>

| <span data-ttu-id="d9fb6-109">属性</span><span class="sxs-lookup"><span data-stu-id="d9fb6-109">Property</span></span>      | <span data-ttu-id="d9fb6-110">类型</span><span class="sxs-lookup"><span data-stu-id="d9fb6-110">Type</span></span>      | <span data-ttu-id="d9fb6-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9fb6-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d9fb6-112">WebUrl</span><span class="sxs-lookup"><span data-stu-id="d9fb6-112">webUrl</span></span>        | <span data-ttu-id="d9fb6-113">String</span><span class="sxs-lookup"><span data-stu-id="d9fb6-113">String</span></span>    | <span data-ttu-id="d9fb6-114">指向引用项的 URL。</span><span class="sxs-lookup"><span data-stu-id="d9fb6-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d9fb6-115">id</span><span class="sxs-lookup"><span data-stu-id="d9fb6-115">id</span></span>            | <span data-ttu-id="d9fb6-116">String</span><span class="sxs-lookup"><span data-stu-id="d9fb6-116">String</span></span>    | <span data-ttu-id="d9fb6-117">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d9fb6-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d9fb6-118">type</span><span class="sxs-lookup"><span data-stu-id="d9fb6-118">type</span></span>          | <span data-ttu-id="d9fb6-119">String</span><span class="sxs-lookup"><span data-stu-id="d9fb6-119">String</span></span>    | <span data-ttu-id="d9fb6-120">一个可用于对项目进行分类的字符串值，例如 "driveItem"</span><span class="sxs-lookup"><span data-stu-id="d9fb6-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |


