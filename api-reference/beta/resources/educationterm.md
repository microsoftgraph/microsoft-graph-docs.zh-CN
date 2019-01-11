---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 67e7cd6c9942b61bb6f9ba45f8f25952ae916c5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835147"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="a4959-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4959-105">educationTerm resource type</span></span>

> <span data-ttu-id="a4959-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4959-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4959-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4959-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4959-108">一个学期。</span><span class="sxs-lookup"><span data-stu-id="a4959-108">A term.</span></span> <span data-ttu-id="a4959-109">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="a4959-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="a4959-110">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="a4959-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a4959-111">属性</span><span class="sxs-lookup"><span data-stu-id="a4959-111">Properties</span></span>
| <span data-ttu-id="a4959-112">属性</span><span class="sxs-lookup"><span data-stu-id="a4959-112">Property</span></span>     | <span data-ttu-id="a4959-113">类型</span><span class="sxs-lookup"><span data-stu-id="a4959-113">Type</span></span>   |<span data-ttu-id="a4959-114">说明</span><span class="sxs-lookup"><span data-stu-id="a4959-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4959-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a4959-115">displayName</span></span>| <span data-ttu-id="a4959-116">String</span><span class="sxs-lookup"><span data-stu-id="a4959-116">String</span></span>| <span data-ttu-id="a4959-117">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a4959-117">Display name of the term.</span></span>| 
|<span data-ttu-id="a4959-118">externalId</span><span class="sxs-lookup"><span data-stu-id="a4959-118">externalId</span></span>|<span data-ttu-id="a4959-119">String</span><span class="sxs-lookup"><span data-stu-id="a4959-119">String</span></span>| <span data-ttu-id="a4959-120">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="a4959-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="a4959-121">startDate</span><span class="sxs-lookup"><span data-stu-id="a4959-121">startDate</span></span>|<span data-ttu-id="a4959-122">Date</span><span class="sxs-lookup"><span data-stu-id="a4959-122">Date</span></span>|<span data-ttu-id="a4959-123">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="a4959-123">Start of the term.</span></span>|
|<span data-ttu-id="a4959-124">endDate</span><span class="sxs-lookup"><span data-stu-id="a4959-124">endDate</span></span>|<span data-ttu-id="a4959-125">Date</span><span class="sxs-lookup"><span data-stu-id="a4959-125">Date</span></span>|<span data-ttu-id="a4959-126">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="a4959-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4959-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4959-127">JSON representation</span></span>

<span data-ttu-id="a4959-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4959-128">The following is a JSON representation of the resource.</span></span>

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
