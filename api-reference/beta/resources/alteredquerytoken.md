---
title: alteredQueryToken 资源类型
description: 表示与原始用户查询有关更改的线段。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 03e6f010fdcd77e07fc6ce3cc7e8c8c285fde73f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067993"
---
# <a name="alteredquerytoken-resource-type"></a><span data-ttu-id="84cb5-103">alteredQueryToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="84cb5-103">alteredQueryToken resource type</span></span>

<span data-ttu-id="84cb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84cb5-105">表示与原始用户查询有关更改的线段。</span><span class="sxs-lookup"><span data-stu-id="84cb5-105">Represents changed segments with respect to original user query.</span></span>

## <a name="properties"></a><span data-ttu-id="84cb5-106">属性</span><span class="sxs-lookup"><span data-stu-id="84cb5-106">Properties</span></span>

| <span data-ttu-id="84cb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="84cb5-107">Property</span></span>     | <span data-ttu-id="84cb5-108">类型</span><span class="sxs-lookup"><span data-stu-id="84cb5-108">Type</span></span>        | <span data-ttu-id="84cb5-109">说明</span><span class="sxs-lookup"><span data-stu-id="84cb5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84cb5-110">offset</span><span class="sxs-lookup"><span data-stu-id="84cb5-110">offset</span></span>|<span data-ttu-id="84cb5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="84cb5-111">Int32</span></span>| <span data-ttu-id="84cb5-112">定义更改的线段的偏移量。</span><span class="sxs-lookup"><span data-stu-id="84cb5-112">Defines the offset of a changed segment.</span></span>|
|<span data-ttu-id="84cb5-113">length</span><span class="sxs-lookup"><span data-stu-id="84cb5-113">length</span></span>|<span data-ttu-id="84cb5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="84cb5-114">Int32</span></span>| <span data-ttu-id="84cb5-115">定义已更改的线段的长度。</span><span class="sxs-lookup"><span data-stu-id="84cb5-115">Defines the length of a changed segment.</span></span>|
|<span data-ttu-id="84cb5-116">suggestion</span><span class="sxs-lookup"><span data-stu-id="84cb5-116">suggestion</span></span>|<span data-ttu-id="84cb5-117">String</span><span class="sxs-lookup"><span data-stu-id="84cb5-117">String</span></span>| <span data-ttu-id="84cb5-118">表示更正的线段字符串。</span><span class="sxs-lookup"><span data-stu-id="84cb5-118">Represents the corrected segment string.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84cb5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84cb5-119">JSON representation</span></span>

<span data-ttu-id="84cb5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84cb5-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "offset": 0,
  "length": 6,
  "suggestion": "String"
}
```
