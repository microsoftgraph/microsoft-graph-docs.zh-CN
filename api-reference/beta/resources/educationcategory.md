---
title: educationCategory 资源类型
description: 可应用于工作分配的类别。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf5ee33ec7d217c0bc4c6e4d35666d6e9f34dadb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340594"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="d2dc9-103">educationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2dc9-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2dc9-104">可应用于工作分配的类别。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="d2dc9-105">方法</span><span class="sxs-lookup"><span data-stu-id="d2dc9-105">Methods</span></span>

| <span data-ttu-id="d2dc9-106">方法</span><span class="sxs-lookup"><span data-stu-id="d2dc9-106">Method</span></span>           | <span data-ttu-id="d2dc9-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2dc9-107">Return Type</span></span>    |<span data-ttu-id="d2dc9-108">说明</span><span class="sxs-lookup"><span data-stu-id="d2dc9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2dc9-109">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="d2dc9-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="d2dc9-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="d2dc9-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="d2dc9-111">获取现有的**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="d2dc9-112">删除类别</span><span class="sxs-lookup"><span data-stu-id="d2dc9-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="d2dc9-113">无</span><span class="sxs-lookup"><span data-stu-id="d2dc9-113">None</span></span> | <span data-ttu-id="d2dc9-114">删除**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="d2dc9-115">属性</span><span class="sxs-lookup"><span data-stu-id="d2dc9-115">Properties</span></span>
| <span data-ttu-id="d2dc9-116">属性</span><span class="sxs-lookup"><span data-stu-id="d2dc9-116">Property</span></span>     | <span data-ttu-id="d2dc9-117">类型</span><span class="sxs-lookup"><span data-stu-id="d2dc9-117">Type</span></span>   |<span data-ttu-id="d2dc9-118">说明</span><span class="sxs-lookup"><span data-stu-id="d2dc9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2dc9-119">id</span><span class="sxs-lookup"><span data-stu-id="d2dc9-119">id</span></span>|<span data-ttu-id="d2dc9-120">String</span><span class="sxs-lookup"><span data-stu-id="d2dc9-120">String</span></span>|<span data-ttu-id="d2dc9-121">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="d2dc9-122">displayName</span><span class="sxs-lookup"><span data-stu-id="d2dc9-122">displayName</span></span>|<span data-ttu-id="d2dc9-123">String</span><span class="sxs-lookup"><span data-stu-id="d2dc9-123">String</span></span>|<span data-ttu-id="d2dc9-124">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2dc9-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2dc9-125">JSON representation</span></span>

<span data-ttu-id="d2dc9-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2dc9-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
