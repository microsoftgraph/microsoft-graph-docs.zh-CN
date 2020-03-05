---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2d93bba585393b11cdb0adc573a8fed5b895ed6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500000"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="dddb2-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="dddb2-105">educationTerm resource type</span></span>

<span data-ttu-id="dddb2-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dddb2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dddb2-107">一个学期。</span><span class="sxs-lookup"><span data-stu-id="dddb2-107">A term.</span></span> <span data-ttu-id="dddb2-108">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="dddb2-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="dddb2-109">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="dddb2-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dddb2-110">属性</span><span class="sxs-lookup"><span data-stu-id="dddb2-110">Properties</span></span>
| <span data-ttu-id="dddb2-111">属性</span><span class="sxs-lookup"><span data-stu-id="dddb2-111">Property</span></span>     | <span data-ttu-id="dddb2-112">类型</span><span class="sxs-lookup"><span data-stu-id="dddb2-112">Type</span></span>   |<span data-ttu-id="dddb2-113">说明</span><span class="sxs-lookup"><span data-stu-id="dddb2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dddb2-114">displayName</span><span class="sxs-lookup"><span data-stu-id="dddb2-114">displayName</span></span>| <span data-ttu-id="dddb2-115">String</span><span class="sxs-lookup"><span data-stu-id="dddb2-115">String</span></span>| <span data-ttu-id="dddb2-116">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dddb2-116">Display name of the term.</span></span>| 
|<span data-ttu-id="dddb2-117">externalId</span><span class="sxs-lookup"><span data-stu-id="dddb2-117">externalId</span></span>|<span data-ttu-id="dddb2-118">String</span><span class="sxs-lookup"><span data-stu-id="dddb2-118">String</span></span>| <span data-ttu-id="dddb2-119">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="dddb2-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="dddb2-120">startDate</span><span class="sxs-lookup"><span data-stu-id="dddb2-120">startDate</span></span>|<span data-ttu-id="dddb2-121">日期</span><span class="sxs-lookup"><span data-stu-id="dddb2-121">Date</span></span>|<span data-ttu-id="dddb2-122">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="dddb2-122">Start of the term.</span></span>|
|<span data-ttu-id="dddb2-123">endDate</span><span class="sxs-lookup"><span data-stu-id="dddb2-123">endDate</span></span>|<span data-ttu-id="dddb2-124">Date</span><span class="sxs-lookup"><span data-stu-id="dddb2-124">Date</span></span>|<span data-ttu-id="dddb2-125">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="dddb2-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dddb2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dddb2-126">JSON representation</span></span>

<span data-ttu-id="dddb2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dddb2-127">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
