---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36426a7e3f1fb79264a788d8af7e7768f5bae26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032618"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="86a3b-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="86a3b-105">educationTerm resource type</span></span>

<span data-ttu-id="86a3b-106">一个学期。</span><span class="sxs-lookup"><span data-stu-id="86a3b-106">A term.</span></span> <span data-ttu-id="86a3b-107">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="86a3b-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="86a3b-108">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="86a3b-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="86a3b-109">属性</span><span class="sxs-lookup"><span data-stu-id="86a3b-109">Properties</span></span>
| <span data-ttu-id="86a3b-110">属性</span><span class="sxs-lookup"><span data-stu-id="86a3b-110">Property</span></span>     | <span data-ttu-id="86a3b-111">类型</span><span class="sxs-lookup"><span data-stu-id="86a3b-111">Type</span></span>   |<span data-ttu-id="86a3b-112">说明</span><span class="sxs-lookup"><span data-stu-id="86a3b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a3b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="86a3b-113">displayName</span></span>| <span data-ttu-id="86a3b-114">String</span><span class="sxs-lookup"><span data-stu-id="86a3b-114">String</span></span>| <span data-ttu-id="86a3b-115">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="86a3b-115">Display name of the term.</span></span>| 
|<span data-ttu-id="86a3b-116">externalId</span><span class="sxs-lookup"><span data-stu-id="86a3b-116">externalId</span></span>|<span data-ttu-id="86a3b-117">String</span><span class="sxs-lookup"><span data-stu-id="86a3b-117">String</span></span>| <span data-ttu-id="86a3b-118">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="86a3b-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="86a3b-119">startDate</span><span class="sxs-lookup"><span data-stu-id="86a3b-119">startDate</span></span>|<span data-ttu-id="86a3b-120">日期</span><span class="sxs-lookup"><span data-stu-id="86a3b-120">Date</span></span>|<span data-ttu-id="86a3b-121">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="86a3b-121">Start of the term.</span></span>|
|<span data-ttu-id="86a3b-122">endDate</span><span class="sxs-lookup"><span data-stu-id="86a3b-122">endDate</span></span>|<span data-ttu-id="86a3b-123">Date</span><span class="sxs-lookup"><span data-stu-id="86a3b-123">Date</span></span>|<span data-ttu-id="86a3b-124">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="86a3b-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86a3b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86a3b-125">JSON representation</span></span>

<span data-ttu-id="86a3b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86a3b-126">The following is a JSON representation of the resource.</span></span>

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
