---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关用户上次访问 (查看) 和修改 (编辑) 资源的时间的信息。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2b91275840546f0ff7486d8ecd5bdde2c1ff31e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005693"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="8cba2-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cba2-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cba2-105">包含已[使用](insights-used.md)项的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="8cba2-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="8cba2-106">有关用户上次访问 (查看) 和修改 (编辑) 资源的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="8cba2-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cba2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cba2-107">JSON representation</span></span>

<span data-ttu-id="8cba2-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cba2-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8cba2-109">属性</span><span class="sxs-lookup"><span data-stu-id="8cba2-109">Properties</span></span>

| <span data-ttu-id="8cba2-110">属性</span><span class="sxs-lookup"><span data-stu-id="8cba2-110">Property</span></span>              | <span data-ttu-id="8cba2-111">类型</span><span class="sxs-lookup"><span data-stu-id="8cba2-111">Type</span></span>          | <span data-ttu-id="8cba2-112">说明</span><span class="sxs-lookup"><span data-stu-id="8cba2-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="8cba2-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cba2-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="8cba2-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cba2-114">DateTimeOffset</span></span>        | <span data-ttu-id="8cba2-115">用户上次访问该资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8cba2-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="8cba2-116">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8cba2-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8cba2-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="8cba2-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8cba2-118">只读。</span><span class="sxs-lookup"><span data-stu-id="8cba2-118">Read-only.</span></span>                      |
| <span data-ttu-id="8cba2-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cba2-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="8cba2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cba2-120">DateTimeOffset</span></span>        | <span data-ttu-id="8cba2-121">用户上次修改资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8cba2-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="8cba2-122">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8cba2-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8cba2-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="8cba2-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8cba2-124">只读。</span><span class="sxs-lookup"><span data-stu-id="8cba2-124">Read-only.</span></span>       |
