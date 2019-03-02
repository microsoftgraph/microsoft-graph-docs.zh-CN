---
title: paymentTerms 资源类型
description: Dynamics 365 Business Central 中的付款条款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365638"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="a0b16-103">paymentTerms 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0b16-103">paymentTerms resource type</span></span>
<span data-ttu-id="a0b16-104">表示 Dynamics 365 Business Central 中的付款期限。</span><span class="sxs-lookup"><span data-stu-id="a0b16-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a0b16-105">方法</span><span class="sxs-lookup"><span data-stu-id="a0b16-105">Methods</span></span>

| <span data-ttu-id="a0b16-106">方法</span><span class="sxs-lookup"><span data-stu-id="a0b16-106">Method</span></span>                                                      | <span data-ttu-id="a0b16-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0b16-107">Return Type</span></span>|<span data-ttu-id="a0b16-108">说明</span><span class="sxs-lookup"><span data-stu-id="a0b16-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="a0b16-109">获取 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="a0b16-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-110">paymentTerms</span></span>|<span data-ttu-id="a0b16-111">获取付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="a0b16-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="a0b16-112">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="a0b16-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-113">paymentTerms</span></span>|<span data-ttu-id="a0b16-114">创建付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="a0b16-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="a0b16-115">修补程序 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="a0b16-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-116">paymentTerms</span></span>|<span data-ttu-id="a0b16-117">更新付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="a0b16-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="a0b16-118">删除 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="a0b16-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="a0b16-119">无</span><span class="sxs-lookup"><span data-stu-id="a0b16-119">none</span></span>        |<span data-ttu-id="a0b16-120">删除付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="a0b16-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0b16-121">属性</span><span class="sxs-lookup"><span data-stu-id="a0b16-121">Properties</span></span>
| <span data-ttu-id="a0b16-122">属性</span><span class="sxs-lookup"><span data-stu-id="a0b16-122">Property</span></span>                     | <span data-ttu-id="a0b16-123">类型</span><span class="sxs-lookup"><span data-stu-id="a0b16-123">Type</span></span>     |<span data-ttu-id="a0b16-124">说明</span><span class="sxs-lookup"><span data-stu-id="a0b16-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="a0b16-125">id</span><span class="sxs-lookup"><span data-stu-id="a0b16-125">id</span></span>                            |<span data-ttu-id="a0b16-126">GUID</span><span class="sxs-lookup"><span data-stu-id="a0b16-126">GUID</span></span>    |<span data-ttu-id="a0b16-127">paymentTerms 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a0b16-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="a0b16-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="a0b16-128">Non-editable.</span></span>           |
|<span data-ttu-id="a0b16-129">code</span><span class="sxs-lookup"><span data-stu-id="a0b16-129">code</span></span>                          |<span data-ttu-id="a0b16-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a0b16-130">string</span></span>  |<span data-ttu-id="a0b16-131">指定付款期限代码。</span><span class="sxs-lookup"><span data-stu-id="a0b16-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="a0b16-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a0b16-132">displayName</span></span>                   |<span data-ttu-id="a0b16-133">string</span><span class="sxs-lookup"><span data-stu-id="a0b16-133">string</span></span>  |<span data-ttu-id="a0b16-134">指定付款期限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a0b16-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="a0b16-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="a0b16-135">dueDateCalculation</span></span>            |<span data-ttu-id="a0b16-136">string</span><span class="sxs-lookup"><span data-stu-id="a0b16-136">string</span></span>  |<span data-ttu-id="a0b16-137">指定用于计算必须进行付款的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="a0b16-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="a0b16-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="a0b16-138">discountDateCalculation</span></span>       |<span data-ttu-id="a0b16-139">string</span><span class="sxs-lookup"><span data-stu-id="a0b16-139">string</span></span>  |<span data-ttu-id="a0b16-140">指定用于计算要获取折扣付款所必须进行的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="a0b16-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="a0b16-141">discountPercent</span><span class="sxs-lookup"><span data-stu-id="a0b16-141">discountPercent</span></span>               |<span data-ttu-id="a0b16-142">decimal</span><span class="sxs-lookup"><span data-stu-id="a0b16-142">decimal</span></span> |<span data-ttu-id="a0b16-143">指定针对发票金额的提前付款应用的折扣百分比。</span><span class="sxs-lookup"><span data-stu-id="a0b16-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="a0b16-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="a0b16-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="a0b16-145">boolean</span><span class="sxs-lookup"><span data-stu-id="a0b16-145">boolean</span></span> |<span data-ttu-id="a0b16-146">指定是否应将折扣应用于贷方通知单。</span><span class="sxs-lookup"><span data-stu-id="a0b16-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="a0b16-147">**如果为 True** , 则表示将提供折扣, **false**表示不会给出折扣。</span><span class="sxs-lookup"><span data-stu-id="a0b16-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="a0b16-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b16-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="a0b16-149">datetime</span><span class="sxs-lookup"><span data-stu-id="a0b16-149">datetime</span></span>|<span data-ttu-id="a0b16-150">上次修改 paymentTerms 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a0b16-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="a0b16-151">只读。</span><span class="sxs-lookup"><span data-stu-id="a0b16-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="a0b16-152">关系</span><span class="sxs-lookup"><span data-stu-id="a0b16-152">Relationships</span></span>
<span data-ttu-id="a0b16-153">无</span><span class="sxs-lookup"><span data-stu-id="a0b16-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0b16-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0b16-154">JSON representation</span></span>

<span data-ttu-id="a0b16-155">下面是 paymentTerms 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0b16-155">Here is a JSON representation of the paymentTerms.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
