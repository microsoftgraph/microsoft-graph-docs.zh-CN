---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e98bb1dc059439dfad927db033759ea54d240716
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340585"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="b8a5c-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8a5c-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8a5c-106">一个学期。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-106">A term.</span></span> <span data-ttu-id="b8a5c-107">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="b8a5c-108">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8a5c-109">属性</span><span class="sxs-lookup"><span data-stu-id="b8a5c-109">Properties</span></span>
| <span data-ttu-id="b8a5c-110">属性</span><span class="sxs-lookup"><span data-stu-id="b8a5c-110">Property</span></span>     | <span data-ttu-id="b8a5c-111">类型</span><span class="sxs-lookup"><span data-stu-id="b8a5c-111">Type</span></span>   |<span data-ttu-id="b8a5c-112">说明</span><span class="sxs-lookup"><span data-stu-id="b8a5c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8a5c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b8a5c-113">displayName</span></span>| <span data-ttu-id="b8a5c-114">String</span><span class="sxs-lookup"><span data-stu-id="b8a5c-114">String</span></span>| <span data-ttu-id="b8a5c-115">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-115">Display name of the term.</span></span>| 
|<span data-ttu-id="b8a5c-116">externalId</span><span class="sxs-lookup"><span data-stu-id="b8a5c-116">externalId</span></span>|<span data-ttu-id="b8a5c-117">String</span><span class="sxs-lookup"><span data-stu-id="b8a5c-117">String</span></span>| <span data-ttu-id="b8a5c-118">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="b8a5c-119">startDate</span><span class="sxs-lookup"><span data-stu-id="b8a5c-119">startDate</span></span>|<span data-ttu-id="b8a5c-120">日期</span><span class="sxs-lookup"><span data-stu-id="b8a5c-120">Date</span></span>|<span data-ttu-id="b8a5c-121">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-121">Start of the term.</span></span>|
|<span data-ttu-id="b8a5c-122">endDate</span><span class="sxs-lookup"><span data-stu-id="b8a5c-122">endDate</span></span>|<span data-ttu-id="b8a5c-123">Date</span><span class="sxs-lookup"><span data-stu-id="b8a5c-123">Date</span></span>|<span data-ttu-id="b8a5c-124">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8a5c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8a5c-125">JSON representation</span></span>

<span data-ttu-id="b8a5c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8a5c-126">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
