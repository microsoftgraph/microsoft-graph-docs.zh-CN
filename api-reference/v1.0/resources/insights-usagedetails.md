---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关上次访问资源的时间的信息 (查看由用户) 编辑的) 或修改的 (。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 79007d71ef44971bfab250c22abc6795a6b38dd4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054761"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="5104e-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="5104e-104">usageDetails resource type</span></span>

<span data-ttu-id="5104e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5104e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5104e-106">包含已 [使用](insights-used.md) 项的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="5104e-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="5104e-107">有关上次访问资源的时间的信息 (查看由用户) 编辑的) 或修改的 (。</span><span class="sxs-lookup"><span data-stu-id="5104e-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5104e-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5104e-108">JSON representation</span></span>

<span data-ttu-id="5104e-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5104e-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="5104e-110">属性</span><span class="sxs-lookup"><span data-stu-id="5104e-110">Properties</span></span>

| <span data-ttu-id="5104e-111">属性</span><span class="sxs-lookup"><span data-stu-id="5104e-111">Property</span></span>              | <span data-ttu-id="5104e-112">类型</span><span class="sxs-lookup"><span data-stu-id="5104e-112">Type</span></span>          | <span data-ttu-id="5104e-113">说明</span><span class="sxs-lookup"><span data-stu-id="5104e-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="5104e-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="5104e-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="5104e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5104e-115">DateTimeOffset</span></span>        | <span data-ttu-id="5104e-116">用户上次访问该资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5104e-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="5104e-117">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5104e-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5104e-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5104e-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5104e-119">只读。</span><span class="sxs-lookup"><span data-stu-id="5104e-119">Read-only.</span></span>                      |
| <span data-ttu-id="5104e-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5104e-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="5104e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5104e-121">DateTimeOffset</span></span>        | <span data-ttu-id="5104e-122">用户上次修改资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5104e-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="5104e-123">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5104e-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5104e-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5104e-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5104e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="5104e-125">Read-only.</span></span>       |

