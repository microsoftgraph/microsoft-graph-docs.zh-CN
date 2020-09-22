---
title: itemCategories 资源类型
description: Dynamics 365 Business Central 中的项类别。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 866fda60aa8b0a357e8e587d105a7fa00e116d3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013839"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="ee7d0-103">itemCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee7d0-103">itemCategories resource type</span></span>

<span data-ttu-id="ee7d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee7d0-105">代表 Dynamics 365 Business Central 中的大量项目的类别。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-105">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ee7d0-106">方法</span><span class="sxs-lookup"><span data-stu-id="ee7d0-106">Methods</span></span>

| <span data-ttu-id="ee7d0-107">方法</span><span class="sxs-lookup"><span data-stu-id="ee7d0-107">Method</span></span>                                                          | <span data-ttu-id="ee7d0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee7d0-108">Return Type</span></span>  |<span data-ttu-id="ee7d0-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee7d0-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="ee7d0-110">获取 itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-110">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="ee7d0-111">itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-111">itemCategories</span></span>|<span data-ttu-id="ee7d0-112">获取项目类别。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-112">Get an item category.</span></span>   |
|[<span data-ttu-id="ee7d0-113">Post itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-113">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="ee7d0-114">itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-114">itemCategories</span></span>|<span data-ttu-id="ee7d0-115">创建项类别。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-115">Create an item category.</span></span>|
|[<span data-ttu-id="ee7d0-116">修补程序 itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-116">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="ee7d0-117">itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-117">itemCategories</span></span>|<span data-ttu-id="ee7d0-118">更新项目类别。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-118">Update an item category.</span></span>|
|[<span data-ttu-id="ee7d0-119">删除 itemCategories</span><span class="sxs-lookup"><span data-stu-id="ee7d0-119">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="ee7d0-120">无</span><span class="sxs-lookup"><span data-stu-id="ee7d0-120">none</span></span>          |<span data-ttu-id="ee7d0-121">删除项目类别。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-121">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee7d0-122">属性</span><span class="sxs-lookup"><span data-stu-id="ee7d0-122">Properties</span></span>
| <span data-ttu-id="ee7d0-123">属性</span><span class="sxs-lookup"><span data-stu-id="ee7d0-123">Property</span></span>           | <span data-ttu-id="ee7d0-124">类型</span><span class="sxs-lookup"><span data-stu-id="ee7d0-124">Type</span></span>   |<span data-ttu-id="ee7d0-125">说明</span><span class="sxs-lookup"><span data-stu-id="ee7d0-125">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="ee7d0-126">id</span><span class="sxs-lookup"><span data-stu-id="ee7d0-126">id</span></span>                  |<span data-ttu-id="ee7d0-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ee7d0-127">GUID</span></span>    |<span data-ttu-id="ee7d0-128">ItemCategory 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-128">The unique ID of the itemCategory.</span></span> <span data-ttu-id="ee7d0-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-129">Non-editable.</span></span>|
|<span data-ttu-id="ee7d0-130">code</span><span class="sxs-lookup"><span data-stu-id="ee7d0-130">code</span></span>                |<span data-ttu-id="ee7d0-131">string</span><span class="sxs-lookup"><span data-stu-id="ee7d0-131">string</span></span>  |<span data-ttu-id="ee7d0-132">ItemCategory 代码。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-132">The itemCategory code.</span></span>                          |
|<span data-ttu-id="ee7d0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7d0-133">displayName</span></span>         |<span data-ttu-id="ee7d0-134">string</span><span class="sxs-lookup"><span data-stu-id="ee7d0-134">string</span></span>  |<span data-ttu-id="ee7d0-135">ItemCategories 显示名称。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-135">The itemCategories display name.</span></span>                |
|<span data-ttu-id="ee7d0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee7d0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ee7d0-137">datetime</span><span class="sxs-lookup"><span data-stu-id="ee7d0-137">datetime</span></span>|<span data-ttu-id="ee7d0-138">上次修改 itemCategory 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-138">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="ee7d0-139">只读。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ee7d0-140">关系</span><span class="sxs-lookup"><span data-stu-id="ee7d0-140">Relationships</span></span>
<span data-ttu-id="ee7d0-141">无</span><span class="sxs-lookup"><span data-stu-id="ee7d0-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee7d0-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee7d0-142">JSON representation</span></span>

<span data-ttu-id="ee7d0-143">下面是 itemCategories 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee7d0-143">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```



