---
title: itemCategories 资源类型
description: Dynamics 365 Business Central 中的项类别。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972920"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="d2272-103">itemCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2272-103">itemCategories resource type</span></span>
<span data-ttu-id="d2272-104">代表 Dynamics 365 Business Central 中的大量项目的类别。</span><span class="sxs-lookup"><span data-stu-id="d2272-104">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d2272-105">方法</span><span class="sxs-lookup"><span data-stu-id="d2272-105">Methods</span></span>

| <span data-ttu-id="d2272-106">方法</span><span class="sxs-lookup"><span data-stu-id="d2272-106">Method</span></span>                                                          | <span data-ttu-id="d2272-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2272-107">Return Type</span></span>  |<span data-ttu-id="d2272-108">说明</span><span class="sxs-lookup"><span data-stu-id="d2272-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="d2272-109">获取 itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-109">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="d2272-110">itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-110">itemCategories</span></span>|<span data-ttu-id="d2272-111">获取项目类别。</span><span class="sxs-lookup"><span data-stu-id="d2272-111">Get an item category.</span></span>   |
|[<span data-ttu-id="d2272-112">Post itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-112">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="d2272-113">itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-113">itemCategories</span></span>|<span data-ttu-id="d2272-114">创建项类别。</span><span class="sxs-lookup"><span data-stu-id="d2272-114">Create an item category.</span></span>|
|[<span data-ttu-id="d2272-115">修补程序 itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-115">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="d2272-116">itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-116">itemCategories</span></span>|<span data-ttu-id="d2272-117">更新项目类别。</span><span class="sxs-lookup"><span data-stu-id="d2272-117">Update an item category.</span></span>|
|[<span data-ttu-id="d2272-118">删除 itemCategories</span><span class="sxs-lookup"><span data-stu-id="d2272-118">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="d2272-119">无</span><span class="sxs-lookup"><span data-stu-id="d2272-119">none</span></span>          |<span data-ttu-id="d2272-120">删除项目类别。</span><span class="sxs-lookup"><span data-stu-id="d2272-120">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2272-121">属性</span><span class="sxs-lookup"><span data-stu-id="d2272-121">Properties</span></span>
| <span data-ttu-id="d2272-122">属性</span><span class="sxs-lookup"><span data-stu-id="d2272-122">Property</span></span>           | <span data-ttu-id="d2272-123">类型</span><span class="sxs-lookup"><span data-stu-id="d2272-123">Type</span></span>   |<span data-ttu-id="d2272-124">说明</span><span class="sxs-lookup"><span data-stu-id="d2272-124">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="d2272-125">id</span><span class="sxs-lookup"><span data-stu-id="d2272-125">id</span></span>                  |<span data-ttu-id="d2272-126">GUID</span><span class="sxs-lookup"><span data-stu-id="d2272-126">GUID</span></span>    |<span data-ttu-id="d2272-127">ItemCategory 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d2272-127">The unique ID of the itemCategory.</span></span> <span data-ttu-id="d2272-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="d2272-128">Non-editable.</span></span>|
|<span data-ttu-id="d2272-129">code</span><span class="sxs-lookup"><span data-stu-id="d2272-129">code</span></span>                |<span data-ttu-id="d2272-130">string</span><span class="sxs-lookup"><span data-stu-id="d2272-130">string</span></span>  |<span data-ttu-id="d2272-131">ItemCategory 代码。</span><span class="sxs-lookup"><span data-stu-id="d2272-131">The itemCategory code.</span></span>                          |
|<span data-ttu-id="d2272-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d2272-132">displayName</span></span>         |<span data-ttu-id="d2272-133">string</span><span class="sxs-lookup"><span data-stu-id="d2272-133">string</span></span>  |<span data-ttu-id="d2272-134">ItemCategories 显示名称。</span><span class="sxs-lookup"><span data-stu-id="d2272-134">The itemCategories display name.</span></span>                |
|<span data-ttu-id="d2272-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2272-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d2272-136">datetime</span><span class="sxs-lookup"><span data-stu-id="d2272-136">datetime</span></span>|<span data-ttu-id="d2272-137">上次修改 itemCategory 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d2272-137">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="d2272-138">只读。</span><span class="sxs-lookup"><span data-stu-id="d2272-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="d2272-139">关系</span><span class="sxs-lookup"><span data-stu-id="d2272-139">Relationships</span></span>
<span data-ttu-id="d2272-140">无</span><span class="sxs-lookup"><span data-stu-id="d2272-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2272-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2272-141">JSON representation</span></span>

<span data-ttu-id="d2272-142">下面是 itemCategories 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2272-142">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

