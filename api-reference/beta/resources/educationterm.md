---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc068df7a31c1b3903e8735ba1255cc3a6f0ae73
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962756"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="77131-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="77131-105">educationTerm resource type</span></span>

> <span data-ttu-id="77131-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="77131-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77131-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77131-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77131-108">一个学期。</span><span class="sxs-lookup"><span data-stu-id="77131-108">A term.</span></span> <span data-ttu-id="77131-109">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="77131-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="77131-110">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="77131-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="77131-111">属性</span><span class="sxs-lookup"><span data-stu-id="77131-111">Properties</span></span>
| <span data-ttu-id="77131-112">属性</span><span class="sxs-lookup"><span data-stu-id="77131-112">Property</span></span>     | <span data-ttu-id="77131-113">类型</span><span class="sxs-lookup"><span data-stu-id="77131-113">Type</span></span>   |<span data-ttu-id="77131-114">说明</span><span class="sxs-lookup"><span data-stu-id="77131-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77131-115">displayName</span><span class="sxs-lookup"><span data-stu-id="77131-115">displayName</span></span>| <span data-ttu-id="77131-116">String</span><span class="sxs-lookup"><span data-stu-id="77131-116">String</span></span>| <span data-ttu-id="77131-117">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="77131-117">Display name of the term.</span></span>| 
|<span data-ttu-id="77131-118">externalId</span><span class="sxs-lookup"><span data-stu-id="77131-118">externalId</span></span>|<span data-ttu-id="77131-119">String</span><span class="sxs-lookup"><span data-stu-id="77131-119">String</span></span>| <span data-ttu-id="77131-120">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="77131-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="77131-121">startDate</span><span class="sxs-lookup"><span data-stu-id="77131-121">startDate</span></span>|<span data-ttu-id="77131-122">Date</span><span class="sxs-lookup"><span data-stu-id="77131-122">Date</span></span>|<span data-ttu-id="77131-123">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="77131-123">Start of the term.</span></span>|
|<span data-ttu-id="77131-124">endDate</span><span class="sxs-lookup"><span data-stu-id="77131-124">endDate</span></span>|<span data-ttu-id="77131-125">Date</span><span class="sxs-lookup"><span data-stu-id="77131-125">Date</span></span>|<span data-ttu-id="77131-126">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="77131-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77131-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77131-127">JSON representation</span></span>

<span data-ttu-id="77131-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77131-128">The following is a JSON representation of the resource.</span></span>

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
