---
title: itemCategories 资源类型
description: Dynamics 365 Business Central 中的项类别。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365743"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="5cc11-103">itemCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cc11-103">itemCategories resource type</span></span>
<span data-ttu-id="5cc11-104">代表 Dynamics 365 Business Central 中的大量项目的类别。</span><span class="sxs-lookup"><span data-stu-id="5cc11-104">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="5cc11-105">方法</span><span class="sxs-lookup"><span data-stu-id="5cc11-105">Methods</span></span>

| <span data-ttu-id="5cc11-106">方法</span><span class="sxs-lookup"><span data-stu-id="5cc11-106">Method</span></span>                                                          | <span data-ttu-id="5cc11-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cc11-107">Return Type</span></span>  |<span data-ttu-id="5cc11-108">说明</span><span class="sxs-lookup"><span data-stu-id="5cc11-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="5cc11-109">获取 itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-109">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="5cc11-110">itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-110">itemCategories</span></span>|<span data-ttu-id="5cc11-111">获取项目类别。</span><span class="sxs-lookup"><span data-stu-id="5cc11-111">Get an item category.</span></span>   |
|[<span data-ttu-id="5cc11-112">Post itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-112">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="5cc11-113">itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-113">itemCategories</span></span>|<span data-ttu-id="5cc11-114">创建项类别。</span><span class="sxs-lookup"><span data-stu-id="5cc11-114">Create an item category.</span></span>|
|[<span data-ttu-id="5cc11-115">修补程序 itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-115">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="5cc11-116">itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-116">itemCategories</span></span>|<span data-ttu-id="5cc11-117">更新项目类别。</span><span class="sxs-lookup"><span data-stu-id="5cc11-117">Update an item category.</span></span>|
|[<span data-ttu-id="5cc11-118">删除 itemCategories</span><span class="sxs-lookup"><span data-stu-id="5cc11-118">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="5cc11-119">无</span><span class="sxs-lookup"><span data-stu-id="5cc11-119">none</span></span>          |<span data-ttu-id="5cc11-120">删除项目类别。</span><span class="sxs-lookup"><span data-stu-id="5cc11-120">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="5cc11-121">属性</span><span class="sxs-lookup"><span data-stu-id="5cc11-121">Properties</span></span>
| <span data-ttu-id="5cc11-122">属性</span><span class="sxs-lookup"><span data-stu-id="5cc11-122">Property</span></span>           | <span data-ttu-id="5cc11-123">类型</span><span class="sxs-lookup"><span data-stu-id="5cc11-123">Type</span></span>   |<span data-ttu-id="5cc11-124">说明</span><span class="sxs-lookup"><span data-stu-id="5cc11-124">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="5cc11-125">id</span><span class="sxs-lookup"><span data-stu-id="5cc11-125">id</span></span>                  |<span data-ttu-id="5cc11-126">GUID</span><span class="sxs-lookup"><span data-stu-id="5cc11-126">GUID</span></span>    |<span data-ttu-id="5cc11-127">itemCategory 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5cc11-127">The unique ID of the itemCategory.</span></span> <span data-ttu-id="5cc11-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="5cc11-128">Non-editable.</span></span>|
|<span data-ttu-id="5cc11-129">code</span><span class="sxs-lookup"><span data-stu-id="5cc11-129">code</span></span>                |<span data-ttu-id="5cc11-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5cc11-130">string</span></span>  |<span data-ttu-id="5cc11-131">itemCategory 代码。</span><span class="sxs-lookup"><span data-stu-id="5cc11-131">The itemCategory code.</span></span>                          |
|<span data-ttu-id="5cc11-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5cc11-132">displayName</span></span>         |<span data-ttu-id="5cc11-133">string</span><span class="sxs-lookup"><span data-stu-id="5cc11-133">string</span></span>  |<span data-ttu-id="5cc11-134">itemCategories 显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cc11-134">The itemCategories display name.</span></span>                |
|<span data-ttu-id="5cc11-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc11-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5cc11-136">datetime</span><span class="sxs-lookup"><span data-stu-id="5cc11-136">datetime</span></span>|<span data-ttu-id="5cc11-137">上次修改 itemCategory 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5cc11-137">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="5cc11-138">只读。</span><span class="sxs-lookup"><span data-stu-id="5cc11-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="5cc11-139">关系</span><span class="sxs-lookup"><span data-stu-id="5cc11-139">Relationships</span></span>
<span data-ttu-id="5cc11-140">无</span><span class="sxs-lookup"><span data-stu-id="5cc11-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cc11-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cc11-141">JSON representation</span></span>

<span data-ttu-id="5cc11-142">下面是 itemCategories 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc11-142">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

