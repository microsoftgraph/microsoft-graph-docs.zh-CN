---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
ms.openlocfilehash: a74ea283f153a535008003e6875018eb12a35d15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007584"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="a5ba1-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5ba1-105">educationTerm resource type</span></span>

<span data-ttu-id="a5ba1-106">一个学期。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-106">A term.</span></span> <span data-ttu-id="a5ba1-107">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="a5ba1-108">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a5ba1-109">属性</span><span class="sxs-lookup"><span data-stu-id="a5ba1-109">Properties</span></span>
| <span data-ttu-id="a5ba1-110">属性</span><span class="sxs-lookup"><span data-stu-id="a5ba1-110">Property</span></span>     | <span data-ttu-id="a5ba1-111">类型</span><span class="sxs-lookup"><span data-stu-id="a5ba1-111">Type</span></span>   |<span data-ttu-id="a5ba1-112">说明</span><span class="sxs-lookup"><span data-stu-id="a5ba1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ba1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a5ba1-113">displayName</span></span>| <span data-ttu-id="a5ba1-114">String</span><span class="sxs-lookup"><span data-stu-id="a5ba1-114">String</span></span>| <span data-ttu-id="a5ba1-115">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-115">Display name of the term.</span></span>| 
|<span data-ttu-id="a5ba1-116">externalId</span><span class="sxs-lookup"><span data-stu-id="a5ba1-116">externalId</span></span>|<span data-ttu-id="a5ba1-117">String</span><span class="sxs-lookup"><span data-stu-id="a5ba1-117">String</span></span>| <span data-ttu-id="a5ba1-118">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="a5ba1-119">startDate</span><span class="sxs-lookup"><span data-stu-id="a5ba1-119">startDate</span></span>|<span data-ttu-id="a5ba1-120">Date</span><span class="sxs-lookup"><span data-stu-id="a5ba1-120">Date</span></span>|<span data-ttu-id="a5ba1-121">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-121">Start of the term.</span></span>|
|<span data-ttu-id="a5ba1-122">endDate</span><span class="sxs-lookup"><span data-stu-id="a5ba1-122">endDate</span></span>|<span data-ttu-id="a5ba1-123">Date</span><span class="sxs-lookup"><span data-stu-id="a5ba1-123">Date</span></span>|<span data-ttu-id="a5ba1-124">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ba1-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5ba1-125">JSON representation</span></span>

<span data-ttu-id="a5ba1-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-126">The following is a JSON representation of the resource.</span></span>

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