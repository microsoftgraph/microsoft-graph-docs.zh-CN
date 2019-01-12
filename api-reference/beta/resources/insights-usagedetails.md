---
title: usageDetails 资源类型
description: 包含使用项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 466308ad1b6290c2b96335f94c586eb35c6cac28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950016"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="8fd9e-104">usageDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fd9e-104">usageDetails resource type</span></span>

> <span data-ttu-id="8fd9e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fd9e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fd9e-107">包含[用于](insights-used.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="8fd9e-108">上次访问该资源的信息 （查看） 和修改用户 （编辑）。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fd9e-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fd9e-109">JSON representation</span></span>

<span data-ttu-id="8fd9e-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="8fd9e-111">属性</span><span class="sxs-lookup"><span data-stu-id="8fd9e-111">Properties</span></span>

| <span data-ttu-id="8fd9e-112">属性</span><span class="sxs-lookup"><span data-stu-id="8fd9e-112">Property</span></span>              | <span data-ttu-id="8fd9e-113">类型</span><span class="sxs-lookup"><span data-stu-id="8fd9e-113">Type</span></span>          | <span data-ttu-id="8fd9e-114">说明</span><span class="sxs-lookup"><span data-stu-id="8fd9e-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="8fd9e-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fd9e-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="8fd9e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fd9e-116">DateTimeOffset</span></span>        | <span data-ttu-id="8fd9e-117">日期和时间用户上次访问资源。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="8fd9e-118">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fd9e-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8fd9e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-120">Read-only.</span></span>                      |
| <span data-ttu-id="8fd9e-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fd9e-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="8fd9e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fd9e-122">DateTimeOffset</span></span>        | <span data-ttu-id="8fd9e-123">日期和时间用户上次修改资源。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="8fd9e-124">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fd9e-125">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8fd9e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8fd9e-126">Read-only.</span></span>       |
