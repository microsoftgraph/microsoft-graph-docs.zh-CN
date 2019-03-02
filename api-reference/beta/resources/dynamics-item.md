---
title: items 资源类型
description: Dynamics 365 Business Central 中的 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365960"
---
# <a name="items-resource-type"></a><span data-ttu-id="1577e-103">items 资源类型</span><span class="sxs-lookup"><span data-stu-id="1577e-103">items resource type</span></span>
<span data-ttu-id="1577e-104">表示 Dynamics 365 Business Central 中的项。</span><span class="sxs-lookup"><span data-stu-id="1577e-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1577e-105">方法</span><span class="sxs-lookup"><span data-stu-id="1577e-105">Methods</span></span>

| <span data-ttu-id="1577e-106">方法</span><span class="sxs-lookup"><span data-stu-id="1577e-106">Method</span></span>                                      |<span data-ttu-id="1577e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1577e-107">Return Type</span></span>|<span data-ttu-id="1577e-108">说明</span><span class="sxs-lookup"><span data-stu-id="1577e-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="1577e-109">获取项目</span><span class="sxs-lookup"><span data-stu-id="1577e-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="1577e-110">项目</span><span class="sxs-lookup"><span data-stu-id="1577e-110">items</span></span>     |<span data-ttu-id="1577e-111">获取一个项目对象。</span><span class="sxs-lookup"><span data-stu-id="1577e-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="1577e-112">发布项目</span><span class="sxs-lookup"><span data-stu-id="1577e-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="1577e-113">项目</span><span class="sxs-lookup"><span data-stu-id="1577e-113">items</span></span>     |<span data-ttu-id="1577e-114">创建一个 item 对象。</span><span class="sxs-lookup"><span data-stu-id="1577e-114">Creates an item object.</span></span>|
|[<span data-ttu-id="1577e-115">修补程序项</span><span class="sxs-lookup"><span data-stu-id="1577e-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="1577e-116">项目</span><span class="sxs-lookup"><span data-stu-id="1577e-116">items</span></span>     |<span data-ttu-id="1577e-117">更新项目对象。</span><span class="sxs-lookup"><span data-stu-id="1577e-117">Updates an item object.</span></span>|
|[<span data-ttu-id="1577e-118">删除项目</span><span class="sxs-lookup"><span data-stu-id="1577e-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="1577e-119">无</span><span class="sxs-lookup"><span data-stu-id="1577e-119">none</span></span>      |<span data-ttu-id="1577e-120">删除 item 对象。</span><span class="sxs-lookup"><span data-stu-id="1577e-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1577e-121">属性</span><span class="sxs-lookup"><span data-stu-id="1577e-121">Properties</span></span>
| <span data-ttu-id="1577e-122">属性</span><span class="sxs-lookup"><span data-stu-id="1577e-122">Property</span></span>           | <span data-ttu-id="1577e-123">类型</span><span class="sxs-lookup"><span data-stu-id="1577e-123">Type</span></span> |<span data-ttu-id="1577e-124">说明</span><span class="sxs-lookup"><span data-stu-id="1577e-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="1577e-125">id</span><span class="sxs-lookup"><span data-stu-id="1577e-125">id</span></span>                  |<span data-ttu-id="1577e-126">GUID</span><span class="sxs-lookup"><span data-stu-id="1577e-126">GUID</span></span>    |<span data-ttu-id="1577e-127">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1577e-127">The unique ID of the item.</span></span> <span data-ttu-id="1577e-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="1577e-128">Non-editable.</span></span>             |
|<span data-ttu-id="1577e-129">number</span><span class="sxs-lookup"><span data-stu-id="1577e-129">number</span></span>              |<span data-ttu-id="1577e-130">string</span><span class="sxs-lookup"><span data-stu-id="1577e-130">string</span></span>  |<span data-ttu-id="1577e-131">物料编号。</span><span class="sxs-lookup"><span data-stu-id="1577e-131">The item number.</span></span>                                     |
|<span data-ttu-id="1577e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1577e-132">displayName</span></span>         |<span data-ttu-id="1577e-133">string</span><span class="sxs-lookup"><span data-stu-id="1577e-133">string</span></span>  |<span data-ttu-id="1577e-134">指定项的说明。</span><span class="sxs-lookup"><span data-stu-id="1577e-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="1577e-135">type</span><span class="sxs-lookup"><span data-stu-id="1577e-135">type</span></span>                |<span data-ttu-id="1577e-136">位数</span><span class="sxs-lookup"><span data-stu-id="1577e-136">numeric</span></span> |<span data-ttu-id="1577e-137">项目的库存类型。</span><span class="sxs-lookup"><span data-stu-id="1577e-137">The inventory type for the item.</span></span> <span data-ttu-id="1577e-138">1 = 库存项, 2 = 服务项。</span><span class="sxs-lookup"><span data-stu-id="1577e-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="1577e-139">此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="1577e-139">This is a required property.</span></span>|
|<span data-ttu-id="1577e-140">已阻止</span><span class="sxs-lookup"><span data-stu-id="1577e-140">blocked</span></span>             |<span data-ttu-id="1577e-141">boolean</span><span class="sxs-lookup"><span data-stu-id="1577e-141">boolean</span></span> |<span data-ttu-id="1577e-142">指定无法发布项目的事务, 例如, 由于该项目处于隔离中。</span><span class="sxs-lookup"><span data-stu-id="1577e-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="1577e-143">如果项目被阻止, 则设置为**true**。</span><span class="sxs-lookup"><span data-stu-id="1577e-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="1577e-144">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="1577e-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="1577e-145">GUID</span><span class="sxs-lookup"><span data-stu-id="1577e-145">GUID</span></span>    |<span data-ttu-id="1577e-146">指定度量单位的 ID。</span><span class="sxs-lookup"><span data-stu-id="1577e-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="1577e-147">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="1577e-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="1577e-148">翻.UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="1577e-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="1577e-149">指定项在库存中保留的单位。</span><span class="sxs-lookup"><span data-stu-id="1577e-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="1577e-150">gtin</span><span class="sxs-lookup"><span data-stu-id="1577e-150">gtin</span></span>                |<span data-ttu-id="1577e-151">位数</span><span class="sxs-lookup"><span data-stu-id="1577e-151">numeric</span></span> |<span data-ttu-id="1577e-152">这是全局贸易项目编号。</span><span class="sxs-lookup"><span data-stu-id="1577e-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="1577e-153">itemCategoryId</span><span class="sxs-lookup"><span data-stu-id="1577e-153">itemCategoryId</span></span>      |<span data-ttu-id="1577e-154">GUID</span><span class="sxs-lookup"><span data-stu-id="1577e-154">GUID</span></span> |<span data-ttu-id="1577e-155">指定项所属的类别。</span><span class="sxs-lookup"><span data-stu-id="1577e-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="1577e-156">项类别还包含任何已分配的项属性。</span><span class="sxs-lookup"><span data-stu-id="1577e-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="1577e-157">inventory</span><span class="sxs-lookup"><span data-stu-id="1577e-157">inventory</span></span>           |<span data-ttu-id="1577e-158">decimal</span><span class="sxs-lookup"><span data-stu-id="1577e-158">decimal</span></span> |<span data-ttu-id="1577e-159">指定项目在库存中的单位 (例如, 棋子、方框或箱) 的数量。</span><span class="sxs-lookup"><span data-stu-id="1577e-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="1577e-160">只读。</span><span class="sxs-lookup"><span data-stu-id="1577e-160">Read-Only.</span></span>|
|<span data-ttu-id="1577e-161">价格</span><span class="sxs-lookup"><span data-stu-id="1577e-161">unitPrice</span></span>           |<span data-ttu-id="1577e-162">decimal</span><span class="sxs-lookup"><span data-stu-id="1577e-162">decimal</span></span> |<span data-ttu-id="1577e-163">以指定货币指定项目的一个单位的价格。</span><span class="sxs-lookup"><span data-stu-id="1577e-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="1577e-164">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="1577e-164">priceIncludesTax</span></span>    |<span data-ttu-id="1577e-165">boolean</span><span class="sxs-lookup"><span data-stu-id="1577e-165">boolean</span></span> |<span data-ttu-id="1577e-166">指定单价包含税。</span><span class="sxs-lookup"><span data-stu-id="1577e-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="1577e-167">如果单价包含税, 则设置为**true**。</span><span class="sxs-lookup"><span data-stu-id="1577e-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="1577e-168">unitCost</span><span class="sxs-lookup"><span data-stu-id="1577e-168">unitCost</span></span>            |<span data-ttu-id="1577e-169">decimal</span><span class="sxs-lookup"><span data-stu-id="1577e-169">decimal</span></span> |<span data-ttu-id="1577e-170">指定项目的每单位成本。</span><span class="sxs-lookup"><span data-stu-id="1577e-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="1577e-171">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="1577e-171">taxGroupId</span></span>          |<span data-ttu-id="1577e-172">GUID</span><span class="sxs-lookup"><span data-stu-id="1577e-172">GUID</span></span>    |<span data-ttu-id="1577e-173">指定项目的税务组的 ID。</span><span class="sxs-lookup"><span data-stu-id="1577e-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="1577e-174">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="1577e-174">taxGroupCode</span></span>        |<span data-ttu-id="1577e-175">位数</span><span class="sxs-lookup"><span data-stu-id="1577e-175">numeric</span></span> |<span data-ttu-id="1577e-176">税组表示符合相同税条款的一组库存物料或资源。</span><span class="sxs-lookup"><span data-stu-id="1577e-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="1577e-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1577e-177">lastModifiedDateTime</span></span>|<span data-ttu-id="1577e-178">datetime</span><span class="sxs-lookup"><span data-stu-id="1577e-178">datetime</span></span>|<span data-ttu-id="1577e-179">项目修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1577e-179">The last datetime the item was modified.</span></span> <span data-ttu-id="1577e-180">只读。</span><span class="sxs-lookup"><span data-stu-id="1577e-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="1577e-181">关系</span><span class="sxs-lookup"><span data-stu-id="1577e-181">Relationships</span></span>
<span data-ttu-id="1577e-182">税组 (taxGroupCode) 必须存在于税务组表中。</span><span class="sxs-lookup"><span data-stu-id="1577e-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1577e-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1577e-183">JSON representation</span></span>

<span data-ttu-id="1577e-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1577e-184">Here is a JSON representation of the resource.</span></span>


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


