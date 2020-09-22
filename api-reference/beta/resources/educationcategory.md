---
title: educationCategory 资源类型
description: 可应用于工作分配的类别。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82ad4f009ca76625c148e8a42e58385195466fbb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095539"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="02e8a-103">educationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="02e8a-103">educationCategory resource type</span></span>

<span data-ttu-id="02e8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02e8a-105">可应用于工作分配的类别。</span><span class="sxs-lookup"><span data-stu-id="02e8a-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="02e8a-106">方法</span><span class="sxs-lookup"><span data-stu-id="02e8a-106">Methods</span></span>

| <span data-ttu-id="02e8a-107">方法</span><span class="sxs-lookup"><span data-stu-id="02e8a-107">Method</span></span>           | <span data-ttu-id="02e8a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="02e8a-108">Return Type</span></span>    |<span data-ttu-id="02e8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="02e8a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02e8a-110">Create category</span><span class="sxs-lookup"><span data-stu-id="02e8a-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="02e8a-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="02e8a-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="02e8a-112">创建新的 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="02e8a-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="02e8a-113">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="02e8a-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="02e8a-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="02e8a-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="02e8a-115">获取现有的 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="02e8a-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="02e8a-116">删除类别</span><span class="sxs-lookup"><span data-stu-id="02e8a-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="02e8a-117">无</span><span class="sxs-lookup"><span data-stu-id="02e8a-117">None</span></span> | <span data-ttu-id="02e8a-118">删除 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="02e8a-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="02e8a-119">属性</span><span class="sxs-lookup"><span data-stu-id="02e8a-119">Properties</span></span>
| <span data-ttu-id="02e8a-120">属性</span><span class="sxs-lookup"><span data-stu-id="02e8a-120">Property</span></span>     | <span data-ttu-id="02e8a-121">类型</span><span class="sxs-lookup"><span data-stu-id="02e8a-121">Type</span></span>   |<span data-ttu-id="02e8a-122">说明</span><span class="sxs-lookup"><span data-stu-id="02e8a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02e8a-123">id</span><span class="sxs-lookup"><span data-stu-id="02e8a-123">id</span></span>|<span data-ttu-id="02e8a-124">字符串</span><span class="sxs-lookup"><span data-stu-id="02e8a-124">String</span></span>|<span data-ttu-id="02e8a-125">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="02e8a-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="02e8a-126">displayName</span><span class="sxs-lookup"><span data-stu-id="02e8a-126">displayName</span></span>|<span data-ttu-id="02e8a-127">字符串</span><span class="sxs-lookup"><span data-stu-id="02e8a-127">String</span></span>|<span data-ttu-id="02e8a-128">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="02e8a-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02e8a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02e8a-129">JSON representation</span></span>

<span data-ttu-id="02e8a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02e8a-130">The following is a JSON representation of the resource.</span></span>

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


