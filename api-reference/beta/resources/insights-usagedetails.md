---
title: usageDetails 资源类型
description: 包含已使用项的属性的复杂类型。 有关用户上次访问 (查看) 和修改 (编辑) 资源的时间的信息。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551289"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="122cb-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="122cb-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="122cb-105">包含已[使用](insights-used.md)项的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="122cb-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="122cb-106">有关用户上次访问 (查看) 和修改 (编辑) 资源的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="122cb-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="122cb-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="122cb-107">JSON representation</span></span>

<span data-ttu-id="122cb-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="122cb-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="122cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="122cb-109">Properties</span></span>

| <span data-ttu-id="122cb-110">属性</span><span class="sxs-lookup"><span data-stu-id="122cb-110">Property</span></span>              | <span data-ttu-id="122cb-111">类型</span><span class="sxs-lookup"><span data-stu-id="122cb-111">Type</span></span>          | <span data-ttu-id="122cb-112">说明</span><span class="sxs-lookup"><span data-stu-id="122cb-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="122cb-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="122cb-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="122cb-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="122cb-114">DateTimeOffset</span></span>        | <span data-ttu-id="122cb-115">用户上次访问该资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="122cb-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="122cb-116">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="122cb-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="122cb-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="122cb-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="122cb-118">只读。</span><span class="sxs-lookup"><span data-stu-id="122cb-118">Read-only.</span></span>                      |
| <span data-ttu-id="122cb-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="122cb-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="122cb-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="122cb-120">DateTimeOffset</span></span>        | <span data-ttu-id="122cb-121">用户上次修改资源的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="122cb-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="122cb-122">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="122cb-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="122cb-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="122cb-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="122cb-124">只读。</span><span class="sxs-lookup"><span data-stu-id="122cb-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
