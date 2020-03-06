---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59558512d27bb92c48fb5c0ac2dd0fb52f7c426d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531506"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="3d7b7-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d7b7-105">educationTerm resource type</span></span>

<span data-ttu-id="3d7b7-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d7b7-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d7b7-107">一个学期。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-107">A term.</span></span> <span data-ttu-id="3d7b7-108">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="3d7b7-109">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3d7b7-110">属性</span><span class="sxs-lookup"><span data-stu-id="3d7b7-110">Properties</span></span>
| <span data-ttu-id="3d7b7-111">属性</span><span class="sxs-lookup"><span data-stu-id="3d7b7-111">Property</span></span>     | <span data-ttu-id="3d7b7-112">类型</span><span class="sxs-lookup"><span data-stu-id="3d7b7-112">Type</span></span>   |<span data-ttu-id="3d7b7-113">说明</span><span class="sxs-lookup"><span data-stu-id="3d7b7-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d7b7-114">displayName</span><span class="sxs-lookup"><span data-stu-id="3d7b7-114">displayName</span></span>| <span data-ttu-id="3d7b7-115">String</span><span class="sxs-lookup"><span data-stu-id="3d7b7-115">String</span></span>| <span data-ttu-id="3d7b7-116">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-116">Display name of the term.</span></span>| 
|<span data-ttu-id="3d7b7-117">externalId</span><span class="sxs-lookup"><span data-stu-id="3d7b7-117">externalId</span></span>|<span data-ttu-id="3d7b7-118">String</span><span class="sxs-lookup"><span data-stu-id="3d7b7-118">String</span></span>| <span data-ttu-id="3d7b7-119">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="3d7b7-120">startDate</span><span class="sxs-lookup"><span data-stu-id="3d7b7-120">startDate</span></span>|<span data-ttu-id="3d7b7-121">日期</span><span class="sxs-lookup"><span data-stu-id="3d7b7-121">Date</span></span>|<span data-ttu-id="3d7b7-122">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-122">Start of the term.</span></span>|
|<span data-ttu-id="3d7b7-123">endDate</span><span class="sxs-lookup"><span data-stu-id="3d7b7-123">endDate</span></span>|<span data-ttu-id="3d7b7-124">Date</span><span class="sxs-lookup"><span data-stu-id="3d7b7-124">Date</span></span>|<span data-ttu-id="3d7b7-125">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d7b7-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d7b7-126">JSON representation</span></span>

<span data-ttu-id="3d7b7-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d7b7-127">The following is a JSON representation of the resource.</span></span>

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
