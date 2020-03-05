---
title: items 资源类型
description: Dynamics 365 Business Central 中的 item 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e5578cc2bc05aedd417230cc3e9d3b171e9ba577
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503899"
---
# <a name="items-resource-type"></a><span data-ttu-id="06021-103">items 资源类型</span><span class="sxs-lookup"><span data-stu-id="06021-103">items resource type</span></span>

<span data-ttu-id="06021-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="06021-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06021-105">表示 Dynamics 365 Business Central 中的项。</span><span class="sxs-lookup"><span data-stu-id="06021-105">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="06021-106">方法</span><span class="sxs-lookup"><span data-stu-id="06021-106">Methods</span></span>

| <span data-ttu-id="06021-107">方法</span><span class="sxs-lookup"><span data-stu-id="06021-107">Method</span></span>                                      |<span data-ttu-id="06021-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="06021-108">Return Type</span></span>|<span data-ttu-id="06021-109">说明</span><span class="sxs-lookup"><span data-stu-id="06021-109">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="06021-110">获取项目</span><span class="sxs-lookup"><span data-stu-id="06021-110">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="06021-111">items</span><span class="sxs-lookup"><span data-stu-id="06021-111">items</span></span>     |<span data-ttu-id="06021-112">获取一个项目对象。</span><span class="sxs-lookup"><span data-stu-id="06021-112">Gets an item object.</span></span>   |
|[<span data-ttu-id="06021-113">发布项目</span><span class="sxs-lookup"><span data-stu-id="06021-113">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="06021-114">items</span><span class="sxs-lookup"><span data-stu-id="06021-114">items</span></span>     |<span data-ttu-id="06021-115">创建一个 item 对象。</span><span class="sxs-lookup"><span data-stu-id="06021-115">Creates an item object.</span></span>|
|[<span data-ttu-id="06021-116">修补程序项</span><span class="sxs-lookup"><span data-stu-id="06021-116">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="06021-117">items</span><span class="sxs-lookup"><span data-stu-id="06021-117">items</span></span>     |<span data-ttu-id="06021-118">更新项目对象。</span><span class="sxs-lookup"><span data-stu-id="06021-118">Updates an item object.</span></span>|
|[<span data-ttu-id="06021-119">删除项目</span><span class="sxs-lookup"><span data-stu-id="06021-119">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="06021-120">无</span><span class="sxs-lookup"><span data-stu-id="06021-120">none</span></span>      |<span data-ttu-id="06021-121">删除 item 对象。</span><span class="sxs-lookup"><span data-stu-id="06021-121">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06021-122">属性</span><span class="sxs-lookup"><span data-stu-id="06021-122">Properties</span></span>
| <span data-ttu-id="06021-123">属性</span><span class="sxs-lookup"><span data-stu-id="06021-123">Property</span></span>           | <span data-ttu-id="06021-124">类型</span><span class="sxs-lookup"><span data-stu-id="06021-124">Type</span></span> |<span data-ttu-id="06021-125">说明</span><span class="sxs-lookup"><span data-stu-id="06021-125">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="06021-126">id</span><span class="sxs-lookup"><span data-stu-id="06021-126">id</span></span>                  |<span data-ttu-id="06021-127">GUID</span><span class="sxs-lookup"><span data-stu-id="06021-127">GUID</span></span>    |<span data-ttu-id="06021-128">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="06021-128">The unique ID of the item.</span></span> <span data-ttu-id="06021-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="06021-129">Non-editable.</span></span>             |
|<span data-ttu-id="06021-130">number</span><span class="sxs-lookup"><span data-stu-id="06021-130">number</span></span>              |<span data-ttu-id="06021-131">string</span><span class="sxs-lookup"><span data-stu-id="06021-131">string</span></span>  |<span data-ttu-id="06021-132">物料编号。</span><span class="sxs-lookup"><span data-stu-id="06021-132">The item number.</span></span>                                     |
|<span data-ttu-id="06021-133">displayName</span><span class="sxs-lookup"><span data-stu-id="06021-133">displayName</span></span>         |<span data-ttu-id="06021-134">string</span><span class="sxs-lookup"><span data-stu-id="06021-134">string</span></span>  |<span data-ttu-id="06021-135">指定项的说明。</span><span class="sxs-lookup"><span data-stu-id="06021-135">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="06021-136">type</span><span class="sxs-lookup"><span data-stu-id="06021-136">type</span></span>                |<span data-ttu-id="06021-137">位数</span><span class="sxs-lookup"><span data-stu-id="06021-137">numeric</span></span> |<span data-ttu-id="06021-138">项目的库存类型。</span><span class="sxs-lookup"><span data-stu-id="06021-138">The inventory type for the item.</span></span> <span data-ttu-id="06021-139">1 = 库存项，2 = 服务项。</span><span class="sxs-lookup"><span data-stu-id="06021-139">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="06021-140">此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="06021-140">This is a required property.</span></span>|
|<span data-ttu-id="06021-141">堵塞</span><span class="sxs-lookup"><span data-stu-id="06021-141">blocked</span></span>             |<span data-ttu-id="06021-142">boolean</span><span class="sxs-lookup"><span data-stu-id="06021-142">boolean</span></span> |<span data-ttu-id="06021-143">指定无法发布项目的事务，例如，由于该项目处于隔离中。</span><span class="sxs-lookup"><span data-stu-id="06021-143">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="06021-144">如果项目被阻止，则设置为**true**。</span><span class="sxs-lookup"><span data-stu-id="06021-144">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="06021-145">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="06021-145">baseUnitOfMeasureId</span></span> |<span data-ttu-id="06021-146">GUID</span><span class="sxs-lookup"><span data-stu-id="06021-146">GUID</span></span>    |<span data-ttu-id="06021-147">指定度量单位的 ID。</span><span class="sxs-lookup"><span data-stu-id="06021-147">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="06021-148">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="06021-148">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="06021-149">翻.UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="06021-149">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="06021-150">指定项在库存中保留的单位。</span><span class="sxs-lookup"><span data-stu-id="06021-150">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="06021-151">gtin</span><span class="sxs-lookup"><span data-stu-id="06021-151">gtin</span></span>                |<span data-ttu-id="06021-152">位数</span><span class="sxs-lookup"><span data-stu-id="06021-152">numeric</span></span> |<span data-ttu-id="06021-153">这是全局贸易项目编号。</span><span class="sxs-lookup"><span data-stu-id="06021-153">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="06021-154">itemCategoryId</span><span class="sxs-lookup"><span data-stu-id="06021-154">itemCategoryId</span></span>      |<span data-ttu-id="06021-155">GUID</span><span class="sxs-lookup"><span data-stu-id="06021-155">GUID</span></span> |<span data-ttu-id="06021-156">指定项所属的类别。</span><span class="sxs-lookup"><span data-stu-id="06021-156">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="06021-157">项类别还包含任何已分配的项属性。</span><span class="sxs-lookup"><span data-stu-id="06021-157">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="06021-158">inventory</span><span class="sxs-lookup"><span data-stu-id="06021-158">inventory</span></span>           |<span data-ttu-id="06021-159">数位</span><span class="sxs-lookup"><span data-stu-id="06021-159">decimal</span></span> |<span data-ttu-id="06021-160">指定项目在库存中的单位（例如，棋子、方框或箱）的数量。</span><span class="sxs-lookup"><span data-stu-id="06021-160">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="06021-161">只读。</span><span class="sxs-lookup"><span data-stu-id="06021-161">Read-Only.</span></span>|
|<span data-ttu-id="06021-162">价格</span><span class="sxs-lookup"><span data-stu-id="06021-162">unitPrice</span></span>           |<span data-ttu-id="06021-163">数位</span><span class="sxs-lookup"><span data-stu-id="06021-163">decimal</span></span> |<span data-ttu-id="06021-164">以指定货币指定项目的一个单位的价格。</span><span class="sxs-lookup"><span data-stu-id="06021-164">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="06021-165">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="06021-165">priceIncludesTax</span></span>    |<span data-ttu-id="06021-166">boolean</span><span class="sxs-lookup"><span data-stu-id="06021-166">boolean</span></span> |<span data-ttu-id="06021-167">指定单价包含税。</span><span class="sxs-lookup"><span data-stu-id="06021-167">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="06021-168">如果单价包含税，则设置为**true**。</span><span class="sxs-lookup"><span data-stu-id="06021-168">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="06021-169">unitCost</span><span class="sxs-lookup"><span data-stu-id="06021-169">unitCost</span></span>            |<span data-ttu-id="06021-170">数位</span><span class="sxs-lookup"><span data-stu-id="06021-170">decimal</span></span> |<span data-ttu-id="06021-171">指定项目的每单位成本。</span><span class="sxs-lookup"><span data-stu-id="06021-171">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="06021-172">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="06021-172">taxGroupId</span></span>          |<span data-ttu-id="06021-173">GUID</span><span class="sxs-lookup"><span data-stu-id="06021-173">GUID</span></span>    |<span data-ttu-id="06021-174">指定项目的税务组的 ID。</span><span class="sxs-lookup"><span data-stu-id="06021-174">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="06021-175">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="06021-175">taxGroupCode</span></span>        |<span data-ttu-id="06021-176">位数</span><span class="sxs-lookup"><span data-stu-id="06021-176">numeric</span></span> |<span data-ttu-id="06021-177">税组表示符合相同税条款的一组库存物料或资源。</span><span class="sxs-lookup"><span data-stu-id="06021-177">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="06021-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06021-178">lastModifiedDateTime</span></span>|<span data-ttu-id="06021-179">datetime</span><span class="sxs-lookup"><span data-stu-id="06021-179">datetime</span></span>|<span data-ttu-id="06021-180">项目修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06021-180">The last datetime the item was modified.</span></span> <span data-ttu-id="06021-181">只读。</span><span class="sxs-lookup"><span data-stu-id="06021-181">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="06021-182">关系</span><span class="sxs-lookup"><span data-stu-id="06021-182">Relationships</span></span>
<span data-ttu-id="06021-183">税组（taxGroupCode）必须存在于税务组表中。</span><span class="sxs-lookup"><span data-stu-id="06021-183">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06021-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06021-184">JSON representation</span></span>

<span data-ttu-id="06021-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06021-185">Here is a JSON representation of the resource.</span></span>


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


