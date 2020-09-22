---
title: items 资源类型
description: Dynamics 365 Business Central 中的 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 89ccee3123fc3f0fc04b620e5b3528f4a253d1fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058448"
---
# <a name="items-resource-type"></a><span data-ttu-id="6342b-103">items 资源类型</span><span class="sxs-lookup"><span data-stu-id="6342b-103">items resource type</span></span>

<span data-ttu-id="6342b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6342b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6342b-105">表示 Dynamics 365 Business Central 中的项。</span><span class="sxs-lookup"><span data-stu-id="6342b-105">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="6342b-106">方法</span><span class="sxs-lookup"><span data-stu-id="6342b-106">Methods</span></span>

| <span data-ttu-id="6342b-107">方法</span><span class="sxs-lookup"><span data-stu-id="6342b-107">Method</span></span>                                      |<span data-ttu-id="6342b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6342b-108">Return Type</span></span>|<span data-ttu-id="6342b-109">说明</span><span class="sxs-lookup"><span data-stu-id="6342b-109">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="6342b-110">获取项目</span><span class="sxs-lookup"><span data-stu-id="6342b-110">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="6342b-111">items</span><span class="sxs-lookup"><span data-stu-id="6342b-111">items</span></span>     |<span data-ttu-id="6342b-112">获取一个项目对象。</span><span class="sxs-lookup"><span data-stu-id="6342b-112">Gets an item object.</span></span>   |
|[<span data-ttu-id="6342b-113">发布项目</span><span class="sxs-lookup"><span data-stu-id="6342b-113">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="6342b-114">items</span><span class="sxs-lookup"><span data-stu-id="6342b-114">items</span></span>     |<span data-ttu-id="6342b-115">创建一个 item 对象。</span><span class="sxs-lookup"><span data-stu-id="6342b-115">Creates an item object.</span></span>|
|[<span data-ttu-id="6342b-116">修补程序项</span><span class="sxs-lookup"><span data-stu-id="6342b-116">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="6342b-117">items</span><span class="sxs-lookup"><span data-stu-id="6342b-117">items</span></span>     |<span data-ttu-id="6342b-118">更新项目对象。</span><span class="sxs-lookup"><span data-stu-id="6342b-118">Updates an item object.</span></span>|
|[<span data-ttu-id="6342b-119">删除项目</span><span class="sxs-lookup"><span data-stu-id="6342b-119">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="6342b-120">无</span><span class="sxs-lookup"><span data-stu-id="6342b-120">none</span></span>      |<span data-ttu-id="6342b-121">删除 item 对象。</span><span class="sxs-lookup"><span data-stu-id="6342b-121">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6342b-122">属性</span><span class="sxs-lookup"><span data-stu-id="6342b-122">Properties</span></span>
| <span data-ttu-id="6342b-123">属性</span><span class="sxs-lookup"><span data-stu-id="6342b-123">Property</span></span>           | <span data-ttu-id="6342b-124">类型</span><span class="sxs-lookup"><span data-stu-id="6342b-124">Type</span></span> |<span data-ttu-id="6342b-125">说明</span><span class="sxs-lookup"><span data-stu-id="6342b-125">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="6342b-126">id</span><span class="sxs-lookup"><span data-stu-id="6342b-126">id</span></span>                  |<span data-ttu-id="6342b-127">GUID</span><span class="sxs-lookup"><span data-stu-id="6342b-127">GUID</span></span>    |<span data-ttu-id="6342b-128">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6342b-128">The unique ID of the item.</span></span> <span data-ttu-id="6342b-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="6342b-129">Non-editable.</span></span>             |
|<span data-ttu-id="6342b-130">数字</span><span class="sxs-lookup"><span data-stu-id="6342b-130">number</span></span>              |<span data-ttu-id="6342b-131">string</span><span class="sxs-lookup"><span data-stu-id="6342b-131">string</span></span>  |<span data-ttu-id="6342b-132">物料编号。</span><span class="sxs-lookup"><span data-stu-id="6342b-132">The item number.</span></span>                                     |
|<span data-ttu-id="6342b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6342b-133">displayName</span></span>         |<span data-ttu-id="6342b-134">string</span><span class="sxs-lookup"><span data-stu-id="6342b-134">string</span></span>  |<span data-ttu-id="6342b-135">指定项的说明。</span><span class="sxs-lookup"><span data-stu-id="6342b-135">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="6342b-136">type</span><span class="sxs-lookup"><span data-stu-id="6342b-136">type</span></span>                |<span data-ttu-id="6342b-137">位数</span><span class="sxs-lookup"><span data-stu-id="6342b-137">numeric</span></span> |<span data-ttu-id="6342b-138">项目的库存类型。</span><span class="sxs-lookup"><span data-stu-id="6342b-138">The inventory type for the item.</span></span> <span data-ttu-id="6342b-139">1 = 库存项，2 = 服务项。</span><span class="sxs-lookup"><span data-stu-id="6342b-139">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="6342b-140">此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="6342b-140">This is a required property.</span></span>|
|<span data-ttu-id="6342b-141">堵塞</span><span class="sxs-lookup"><span data-stu-id="6342b-141">blocked</span></span>             |<span data-ttu-id="6342b-142">boolean</span><span class="sxs-lookup"><span data-stu-id="6342b-142">boolean</span></span> |<span data-ttu-id="6342b-143">指定无法发布项目的事务，例如，由于该项目处于隔离中。</span><span class="sxs-lookup"><span data-stu-id="6342b-143">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="6342b-144">如果项目被阻止，则设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6342b-144">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="6342b-145">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="6342b-145">baseUnitOfMeasureId</span></span> |<span data-ttu-id="6342b-146">GUID</span><span class="sxs-lookup"><span data-stu-id="6342b-146">GUID</span></span>    |<span data-ttu-id="6342b-147">指定度量单位的 ID。</span><span class="sxs-lookup"><span data-stu-id="6342b-147">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="6342b-148">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6342b-148">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="6342b-149">翻.UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="6342b-149">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="6342b-150">指定项在库存中保留的单位。</span><span class="sxs-lookup"><span data-stu-id="6342b-150">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="6342b-151">gtin</span><span class="sxs-lookup"><span data-stu-id="6342b-151">gtin</span></span>                |<span data-ttu-id="6342b-152">位数</span><span class="sxs-lookup"><span data-stu-id="6342b-152">numeric</span></span> |<span data-ttu-id="6342b-153">这是全局贸易项目编号。</span><span class="sxs-lookup"><span data-stu-id="6342b-153">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="6342b-154">itemCategoryId</span><span class="sxs-lookup"><span data-stu-id="6342b-154">itemCategoryId</span></span>      |<span data-ttu-id="6342b-155">GUID</span><span class="sxs-lookup"><span data-stu-id="6342b-155">GUID</span></span> |<span data-ttu-id="6342b-156">指定项所属的类别。</span><span class="sxs-lookup"><span data-stu-id="6342b-156">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="6342b-157">项类别还包含任何已分配的项属性。</span><span class="sxs-lookup"><span data-stu-id="6342b-157">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="6342b-158">inventory</span><span class="sxs-lookup"><span data-stu-id="6342b-158">inventory</span></span>           |<span data-ttu-id="6342b-159">数位</span><span class="sxs-lookup"><span data-stu-id="6342b-159">decimal</span></span> |<span data-ttu-id="6342b-160">指定项目在库存中的单位（例如，棋子、方框或箱）的数量。</span><span class="sxs-lookup"><span data-stu-id="6342b-160">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="6342b-161">只读。</span><span class="sxs-lookup"><span data-stu-id="6342b-161">Read-Only.</span></span>|
|<span data-ttu-id="6342b-162">价格</span><span class="sxs-lookup"><span data-stu-id="6342b-162">unitPrice</span></span>           |<span data-ttu-id="6342b-163">数位</span><span class="sxs-lookup"><span data-stu-id="6342b-163">decimal</span></span> |<span data-ttu-id="6342b-164">以指定货币指定项目的一个单位的价格。</span><span class="sxs-lookup"><span data-stu-id="6342b-164">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="6342b-165">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="6342b-165">priceIncludesTax</span></span>    |<span data-ttu-id="6342b-166">boolean</span><span class="sxs-lookup"><span data-stu-id="6342b-166">boolean</span></span> |<span data-ttu-id="6342b-167">指定单价包含税。</span><span class="sxs-lookup"><span data-stu-id="6342b-167">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="6342b-168">如果单价包含税，则设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6342b-168">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="6342b-169">unitCost</span><span class="sxs-lookup"><span data-stu-id="6342b-169">unitCost</span></span>            |<span data-ttu-id="6342b-170">数位</span><span class="sxs-lookup"><span data-stu-id="6342b-170">decimal</span></span> |<span data-ttu-id="6342b-171">指定项目的每单位成本。</span><span class="sxs-lookup"><span data-stu-id="6342b-171">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="6342b-172">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="6342b-172">taxGroupId</span></span>          |<span data-ttu-id="6342b-173">GUID</span><span class="sxs-lookup"><span data-stu-id="6342b-173">GUID</span></span>    |<span data-ttu-id="6342b-174">指定项目的税务组的 ID。</span><span class="sxs-lookup"><span data-stu-id="6342b-174">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="6342b-175">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="6342b-175">taxGroupCode</span></span>        |<span data-ttu-id="6342b-176">位数</span><span class="sxs-lookup"><span data-stu-id="6342b-176">numeric</span></span> |<span data-ttu-id="6342b-177">税组表示符合相同税条款的一组库存物料或资源。</span><span class="sxs-lookup"><span data-stu-id="6342b-177">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="6342b-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6342b-178">lastModifiedDateTime</span></span>|<span data-ttu-id="6342b-179">datetime</span><span class="sxs-lookup"><span data-stu-id="6342b-179">datetime</span></span>|<span data-ttu-id="6342b-180">项目修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6342b-180">The last datetime the item was modified.</span></span> <span data-ttu-id="6342b-181">只读。</span><span class="sxs-lookup"><span data-stu-id="6342b-181">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="6342b-182">关系</span><span class="sxs-lookup"><span data-stu-id="6342b-182">Relationships</span></span>
<span data-ttu-id="6342b-183">税组 (taxGroupCode) 必须存在于税务组表中。</span><span class="sxs-lookup"><span data-stu-id="6342b-183">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6342b-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6342b-184">JSON representation</span></span>

<span data-ttu-id="6342b-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6342b-185">Here is a JSON representation of the resource.</span></span>


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




