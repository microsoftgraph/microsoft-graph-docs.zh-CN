---
title: averageComparativeScore 资源类型
description: 包含基于不同范围的各种不同分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ed82e040121f49bdef29009f6ac387ed4c79cbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532029"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="91b5b-103">averageComparativeScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="91b5b-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="91b5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91b5b-105">包含基于不同范围的各种不同分数（例如，按行业垂直、按公司座位大小的平均值等）和控制类别（标识、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="91b5b-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="91b5b-106">属性</span><span class="sxs-lookup"><span data-stu-id="91b5b-106">Properties</span></span>

|<span data-ttu-id="91b5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="91b5b-107">Property</span></span> |<span data-ttu-id="91b5b-108">类型</span><span class="sxs-lookup"><span data-stu-id="91b5b-108">Type</span></span> |<span data-ttu-id="91b5b-109">说明</span><span class="sxs-lookup"><span data-stu-id="91b5b-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="91b5b-110">基本</span><span class="sxs-lookup"><span data-stu-id="91b5b-110">basis</span></span>|<span data-ttu-id="91b5b-111">字符串</span><span class="sxs-lookup"><span data-stu-id="91b5b-111">String</span></span>|<span data-ttu-id="91b5b-112">范围类型。</span><span class="sxs-lookup"><span data-stu-id="91b5b-112">Scope type.</span></span> <span data-ttu-id="91b5b-113">可能的值包括 `AllTenants`、`TotalSeats`、`IndustryTypes`。</span><span class="sxs-lookup"><span data-stu-id="91b5b-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="91b5b-114">averageScore</span><span class="sxs-lookup"><span data-stu-id="91b5b-114">averageScore</span></span>|<span data-ttu-id="91b5b-115">双精度</span><span class="sxs-lookup"><span data-stu-id="91b5b-115">Double</span></span>|<span data-ttu-id="91b5b-116">指定基准中的平均分数。</span><span class="sxs-lookup"><span data-stu-id="91b5b-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91b5b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91b5b-117">JSON representation</span></span>

<span data-ttu-id="91b5b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91b5b-118">The following is a JSON representation of the resource.</span></span>

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
