---
title: educationCategory 资源类型
description: 可应用于工作分配的类别。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 18ddcd32a2ab4a8d44505adbc92445a0feeae8b6
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911317"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="f4a9c-103">educationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4a9c-103">educationCategory resource type</span></span>

<span data-ttu-id="f4a9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4a9c-105">可应用于工作分配的类别。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="f4a9c-106">方法</span><span class="sxs-lookup"><span data-stu-id="f4a9c-106">Methods</span></span>

| <span data-ttu-id="f4a9c-107">方法</span><span class="sxs-lookup"><span data-stu-id="f4a9c-107">Method</span></span>           | <span data-ttu-id="f4a9c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4a9c-108">Return Type</span></span>    |<span data-ttu-id="f4a9c-109">说明</span><span class="sxs-lookup"><span data-stu-id="f4a9c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4a9c-110">Create category</span><span class="sxs-lookup"><span data-stu-id="f4a9c-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="f4a9c-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="f4a9c-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="f4a9c-112">创建新的 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="f4a9c-113">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="f4a9c-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="f4a9c-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="f4a9c-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="f4a9c-115">获取现有的 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="f4a9c-116">删除类别</span><span class="sxs-lookup"><span data-stu-id="f4a9c-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="f4a9c-117">无</span><span class="sxs-lookup"><span data-stu-id="f4a9c-117">None</span></span> | <span data-ttu-id="f4a9c-118">删除 **educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="f4a9c-119">属性</span><span class="sxs-lookup"><span data-stu-id="f4a9c-119">Properties</span></span>
| <span data-ttu-id="f4a9c-120">属性</span><span class="sxs-lookup"><span data-stu-id="f4a9c-120">Property</span></span>     | <span data-ttu-id="f4a9c-121">类型</span><span class="sxs-lookup"><span data-stu-id="f4a9c-121">Type</span></span>   |<span data-ttu-id="f4a9c-122">说明</span><span class="sxs-lookup"><span data-stu-id="f4a9c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4a9c-123">id</span><span class="sxs-lookup"><span data-stu-id="f4a9c-123">id</span></span>|<span data-ttu-id="f4a9c-124">String</span><span class="sxs-lookup"><span data-stu-id="f4a9c-124">String</span></span>|<span data-ttu-id="f4a9c-125">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="f4a9c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f4a9c-126">displayName</span></span>|<span data-ttu-id="f4a9c-127">String</span><span class="sxs-lookup"><span data-stu-id="f4a9c-127">String</span></span>|<span data-ttu-id="f4a9c-128">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4a9c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4a9c-129">JSON representation</span></span>

<span data-ttu-id="f4a9c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4a9c-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
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


