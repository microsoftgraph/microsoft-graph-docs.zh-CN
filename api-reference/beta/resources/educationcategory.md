---
title: educationCategory 资源类型
description: 可应用于工作分配的类别。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4732bab700ab23869e0463437288b1aa8897aa0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972785"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="f51e8-103">educationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="f51e8-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f51e8-104">可应用于工作分配的类别。</span><span class="sxs-lookup"><span data-stu-id="f51e8-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="f51e8-105">方法</span><span class="sxs-lookup"><span data-stu-id="f51e8-105">Methods</span></span>

| <span data-ttu-id="f51e8-106">方法</span><span class="sxs-lookup"><span data-stu-id="f51e8-106">Method</span></span>           | <span data-ttu-id="f51e8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f51e8-107">Return Type</span></span>    |<span data-ttu-id="f51e8-108">说明</span><span class="sxs-lookup"><span data-stu-id="f51e8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f51e8-109">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="f51e8-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="f51e8-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="f51e8-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="f51e8-111">获取现有的**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="f51e8-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="f51e8-112">删除类别</span><span class="sxs-lookup"><span data-stu-id="f51e8-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="f51e8-113">无</span><span class="sxs-lookup"><span data-stu-id="f51e8-113">None</span></span> | <span data-ttu-id="f51e8-114">删除**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="f51e8-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="f51e8-115">属性</span><span class="sxs-lookup"><span data-stu-id="f51e8-115">Properties</span></span>
| <span data-ttu-id="f51e8-116">属性</span><span class="sxs-lookup"><span data-stu-id="f51e8-116">Property</span></span>     | <span data-ttu-id="f51e8-117">类型</span><span class="sxs-lookup"><span data-stu-id="f51e8-117">Type</span></span>   |<span data-ttu-id="f51e8-118">说明</span><span class="sxs-lookup"><span data-stu-id="f51e8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f51e8-119">id</span><span class="sxs-lookup"><span data-stu-id="f51e8-119">id</span></span>|<span data-ttu-id="f51e8-120">String</span><span class="sxs-lookup"><span data-stu-id="f51e8-120">String</span></span>|<span data-ttu-id="f51e8-121">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f51e8-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="f51e8-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f51e8-122">displayName</span></span>|<span data-ttu-id="f51e8-123">String</span><span class="sxs-lookup"><span data-stu-id="f51e8-123">String</span></span>|<span data-ttu-id="f51e8-124">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f51e8-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f51e8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f51e8-125">JSON representation</span></span>

<span data-ttu-id="f51e8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f51e8-126">The following is a JSON representation of the resource.</span></span>

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
