---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5060120cdbf2a8b6f6497c6bb22efc5d5d084cd1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032571"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="18adc-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="18adc-105">educationTerm resource type</span></span>

<span data-ttu-id="18adc-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18adc-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18adc-107">一个学期。</span><span class="sxs-lookup"><span data-stu-id="18adc-107">A term.</span></span> <span data-ttu-id="18adc-108">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="18adc-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="18adc-109">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="18adc-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18adc-110">属性</span><span class="sxs-lookup"><span data-stu-id="18adc-110">Properties</span></span>
| <span data-ttu-id="18adc-111">属性</span><span class="sxs-lookup"><span data-stu-id="18adc-111">Property</span></span>     | <span data-ttu-id="18adc-112">类型</span><span class="sxs-lookup"><span data-stu-id="18adc-112">Type</span></span>   |<span data-ttu-id="18adc-113">说明</span><span class="sxs-lookup"><span data-stu-id="18adc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18adc-114">displayName</span><span class="sxs-lookup"><span data-stu-id="18adc-114">displayName</span></span>| <span data-ttu-id="18adc-115">String</span><span class="sxs-lookup"><span data-stu-id="18adc-115">String</span></span>| <span data-ttu-id="18adc-116">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="18adc-116">Display name of the term.</span></span>| 
|<span data-ttu-id="18adc-117">externalId</span><span class="sxs-lookup"><span data-stu-id="18adc-117">externalId</span></span>|<span data-ttu-id="18adc-118">String</span><span class="sxs-lookup"><span data-stu-id="18adc-118">String</span></span>| <span data-ttu-id="18adc-119">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="18adc-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="18adc-120">startDate</span><span class="sxs-lookup"><span data-stu-id="18adc-120">startDate</span></span>|<span data-ttu-id="18adc-121">Date</span><span class="sxs-lookup"><span data-stu-id="18adc-121">Date</span></span>|<span data-ttu-id="18adc-122">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="18adc-122">Start of the term.</span></span>|
|<span data-ttu-id="18adc-123">endDate</span><span class="sxs-lookup"><span data-stu-id="18adc-123">endDate</span></span>|<span data-ttu-id="18adc-124">Date</span><span class="sxs-lookup"><span data-stu-id="18adc-124">Date</span></span>|<span data-ttu-id="18adc-125">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="18adc-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18adc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18adc-126">JSON representation</span></span>

<span data-ttu-id="18adc-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18adc-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

