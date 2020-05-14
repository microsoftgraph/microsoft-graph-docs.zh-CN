---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关用户上次访问（查看）或修改（编辑）资源的时间的信息。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: d73af15dc3578e9e6c0a568eebfd42480f7065e2
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227022"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="d3820-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3820-104">usageDetails resource type</span></span>

<span data-ttu-id="d3820-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3820-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3820-106">包含已[使用](insights-used.md)项的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="d3820-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="d3820-107">有关用户上次访问（查看）或修改（编辑）资源的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="d3820-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3820-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3820-108">JSON representation</span></span>

<span data-ttu-id="d3820-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3820-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d3820-110">属性</span><span class="sxs-lookup"><span data-stu-id="d3820-110">Properties</span></span>

| <span data-ttu-id="d3820-111">属性</span><span class="sxs-lookup"><span data-stu-id="d3820-111">Property</span></span>              | <span data-ttu-id="d3820-112">类型</span><span class="sxs-lookup"><span data-stu-id="d3820-112">Type</span></span>          | <span data-ttu-id="d3820-113">说明</span><span class="sxs-lookup"><span data-stu-id="d3820-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="d3820-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3820-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="d3820-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3820-115">DateTimeOffset</span></span>        | <span data-ttu-id="d3820-116">用户上次访问该资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3820-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="d3820-117">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d3820-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3820-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d3820-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d3820-119">只读。</span><span class="sxs-lookup"><span data-stu-id="d3820-119">Read-only.</span></span>                      |
| <span data-ttu-id="d3820-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3820-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="d3820-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3820-121">DateTimeOffset</span></span>        | <span data-ttu-id="d3820-122">用户上次修改资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d3820-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="d3820-123">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d3820-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3820-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d3820-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d3820-125">只读。</span><span class="sxs-lookup"><span data-stu-id="d3820-125">Read-only.</span></span>       |
