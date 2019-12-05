---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关用户上次访问（查看）和修改（编辑）资源的时间的信息。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fb4c1c07d008c37475927d490b49bbb19c1e69d5
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844300"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="d68f4-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d68f4-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d68f4-105">包含已[使用](insights-used.md)项的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="d68f4-105">Complex type containing properties of [used](insights-used.md) items.</span></span> <span data-ttu-id="d68f4-106">有关用户上次访问（查看）和修改（编辑）资源的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="d68f4-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d68f4-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d68f4-107">JSON representation</span></span>

<span data-ttu-id="d68f4-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d68f4-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="d68f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="d68f4-109">Properties</span></span>

| <span data-ttu-id="d68f4-110">属性</span><span class="sxs-lookup"><span data-stu-id="d68f4-110">Property</span></span>              | <span data-ttu-id="d68f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="d68f4-111">Type</span></span>          | <span data-ttu-id="d68f4-112">说明</span><span class="sxs-lookup"><span data-stu-id="d68f4-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="d68f4-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="d68f4-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="d68f4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d68f4-114">DateTimeOffset</span></span>        | <span data-ttu-id="d68f4-115">用户上次访问该资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d68f4-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="d68f4-116">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d68f4-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d68f4-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d68f4-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d68f4-118">只读。</span><span class="sxs-lookup"><span data-stu-id="d68f4-118">Read-only.</span></span>                      |
| <span data-ttu-id="d68f4-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d68f4-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="d68f4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d68f4-120">DateTimeOffset</span></span>        | <span data-ttu-id="d68f4-121">用户上次修改资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d68f4-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="d68f4-122">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d68f4-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d68f4-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d68f4-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d68f4-124">只读。</span><span class="sxs-lookup"><span data-stu-id="d68f4-124">Read-only.</span></span>       |
