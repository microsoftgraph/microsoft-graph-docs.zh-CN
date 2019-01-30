---
title: usageDetails 资源类型
description: 包含使用项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4df15bf635785aba054d52beb89b5ac04d48d3d3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641524"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="359c0-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="359c0-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="359c0-105">包含[用于](insights-used.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="359c0-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="359c0-106">上次访问该资源的信息 （查看） 和修改用户 （编辑）。</span><span class="sxs-lookup"><span data-stu-id="359c0-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="359c0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="359c0-107">JSON representation</span></span>

<span data-ttu-id="359c0-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="359c0-108">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="359c0-109">属性</span><span class="sxs-lookup"><span data-stu-id="359c0-109">Properties</span></span>

| <span data-ttu-id="359c0-110">属性</span><span class="sxs-lookup"><span data-stu-id="359c0-110">Property</span></span>              | <span data-ttu-id="359c0-111">类型</span><span class="sxs-lookup"><span data-stu-id="359c0-111">Type</span></span>          | <span data-ttu-id="359c0-112">说明</span><span class="sxs-lookup"><span data-stu-id="359c0-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="359c0-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="359c0-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="359c0-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359c0-114">DateTimeOffset</span></span>        | <span data-ttu-id="359c0-115">日期和时间用户上次访问资源。</span><span class="sxs-lookup"><span data-stu-id="359c0-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="359c0-116">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="359c0-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="359c0-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="359c0-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="359c0-118">只读。</span><span class="sxs-lookup"><span data-stu-id="359c0-118">Read-only.</span></span>                      |
| <span data-ttu-id="359c0-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="359c0-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="359c0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359c0-120">DateTimeOffset</span></span>        | <span data-ttu-id="359c0-121">日期和时间用户上次修改资源。</span><span class="sxs-lookup"><span data-stu-id="359c0-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="359c0-122">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="359c0-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="359c0-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="359c0-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="359c0-124">只读。</span><span class="sxs-lookup"><span data-stu-id="359c0-124">Read-only.</span></span>       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
