---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947580"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="47d4b-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="47d4b-105">educationTerm resource type</span></span>

<span data-ttu-id="47d4b-106">一个学期。</span><span class="sxs-lookup"><span data-stu-id="47d4b-106">A term.</span></span> <span data-ttu-id="47d4b-107">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="47d4b-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="47d4b-108">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="47d4b-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="47d4b-109">属性</span><span class="sxs-lookup"><span data-stu-id="47d4b-109">Properties</span></span>
| <span data-ttu-id="47d4b-110">属性</span><span class="sxs-lookup"><span data-stu-id="47d4b-110">Property</span></span>     | <span data-ttu-id="47d4b-111">类型</span><span class="sxs-lookup"><span data-stu-id="47d4b-111">Type</span></span>   |<span data-ttu-id="47d4b-112">说明</span><span class="sxs-lookup"><span data-stu-id="47d4b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d4b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="47d4b-113">displayName</span></span>| <span data-ttu-id="47d4b-114">String</span><span class="sxs-lookup"><span data-stu-id="47d4b-114">String</span></span>| <span data-ttu-id="47d4b-115">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="47d4b-115">Display name of the term.</span></span>| 
|<span data-ttu-id="47d4b-116">externalId</span><span class="sxs-lookup"><span data-stu-id="47d4b-116">externalId</span></span>|<span data-ttu-id="47d4b-117">String</span><span class="sxs-lookup"><span data-stu-id="47d4b-117">String</span></span>| <span data-ttu-id="47d4b-118">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="47d4b-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="47d4b-119">startDate</span><span class="sxs-lookup"><span data-stu-id="47d4b-119">startDate</span></span>|<span data-ttu-id="47d4b-120">Date</span><span class="sxs-lookup"><span data-stu-id="47d4b-120">Date</span></span>|<span data-ttu-id="47d4b-121">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="47d4b-121">Start of the term.</span></span>|
|<span data-ttu-id="47d4b-122">endDate</span><span class="sxs-lookup"><span data-stu-id="47d4b-122">endDate</span></span>|<span data-ttu-id="47d4b-123">Date</span><span class="sxs-lookup"><span data-stu-id="47d4b-123">Date</span></span>|<span data-ttu-id="47d4b-124">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="47d4b-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47d4b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47d4b-125">JSON representation</span></span>

<span data-ttu-id="47d4b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47d4b-126">The following is a JSON representation of the resource.</span></span>

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
