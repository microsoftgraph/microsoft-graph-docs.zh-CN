---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bc104f3a9c19c38ef569d08d24da83d0e07d75f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091899"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="6b728-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b728-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="6b728-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b728-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b728-105">包含基于不同范围的不同分数 (例如，按行业垂直排列平均值、按公司座位大小分类的平均值等等) 和控制类别 (标识、数据、设备、应用程序、基础结构) 。</span><span class="sxs-lookup"><span data-stu-id="6b728-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="6b728-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b728-106">Properties</span></span>

|<span data-ttu-id="6b728-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b728-107">Property</span></span> |<span data-ttu-id="6b728-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b728-108">Type</span></span> |<span data-ttu-id="6b728-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b728-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6b728-110">基本</span><span class="sxs-lookup"><span data-stu-id="6b728-110">basis</span></span>|<span data-ttu-id="6b728-111">String</span><span class="sxs-lookup"><span data-stu-id="6b728-111">String</span></span>|<span data-ttu-id="6b728-112">范围类型。</span><span class="sxs-lookup"><span data-stu-id="6b728-112">Scope type.</span></span> <span data-ttu-id="6b728-113">可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。</span><span class="sxs-lookup"><span data-stu-id="6b728-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="6b728-114">averageScore</span><span class="sxs-lookup"><span data-stu-id="6b728-114">averageScore</span></span>|<span data-ttu-id="6b728-115">双精度</span><span class="sxs-lookup"><span data-stu-id="6b728-115">Double</span></span>|<span data-ttu-id="6b728-116">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="6b728-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b728-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b728-117">JSON representation</span></span>

<span data-ttu-id="6b728-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b728-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

