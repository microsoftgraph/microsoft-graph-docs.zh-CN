---
title: paymentTerms 资源类型
description: Dynamics 365 Business Central 中的付款条款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 1e9e7951da79d524002f004410ef6939d7be5b99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027077"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="43295-103">paymentTerms 资源类型</span><span class="sxs-lookup"><span data-stu-id="43295-103">paymentTerms resource type</span></span>

<span data-ttu-id="43295-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43295-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43295-105">表示 Dynamics 365 Business Central 中的付款期限。</span><span class="sxs-lookup"><span data-stu-id="43295-105">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="43295-106">方法</span><span class="sxs-lookup"><span data-stu-id="43295-106">Methods</span></span>

| <span data-ttu-id="43295-107">方法</span><span class="sxs-lookup"><span data-stu-id="43295-107">Method</span></span>                                                      | <span data-ttu-id="43295-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="43295-108">Return Type</span></span>|<span data-ttu-id="43295-109">说明</span><span class="sxs-lookup"><span data-stu-id="43295-109">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="43295-110">获取 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-110">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="43295-111">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-111">paymentTerms</span></span>|<span data-ttu-id="43295-112">获取付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="43295-112">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="43295-113">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-113">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="43295-114">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-114">paymentTerms</span></span>|<span data-ttu-id="43295-115">创建付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="43295-115">Create a payment terms object.</span></span>|
|[<span data-ttu-id="43295-116">修补程序 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-116">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="43295-117">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-117">paymentTerms</span></span>|<span data-ttu-id="43295-118">更新付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="43295-118">Update a payment terms object.</span></span>|
|[<span data-ttu-id="43295-119">删除 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="43295-119">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="43295-120">无</span><span class="sxs-lookup"><span data-stu-id="43295-120">none</span></span>        |<span data-ttu-id="43295-121">删除付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="43295-121">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43295-122">属性</span><span class="sxs-lookup"><span data-stu-id="43295-122">Properties</span></span>
| <span data-ttu-id="43295-123">属性</span><span class="sxs-lookup"><span data-stu-id="43295-123">Property</span></span>                     | <span data-ttu-id="43295-124">类型</span><span class="sxs-lookup"><span data-stu-id="43295-124">Type</span></span>     |<span data-ttu-id="43295-125">说明</span><span class="sxs-lookup"><span data-stu-id="43295-125">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="43295-126">id</span><span class="sxs-lookup"><span data-stu-id="43295-126">id</span></span>                            |<span data-ttu-id="43295-127">GUID</span><span class="sxs-lookup"><span data-stu-id="43295-127">GUID</span></span>    |<span data-ttu-id="43295-128">PaymentTerms 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="43295-128">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="43295-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="43295-129">Non-editable.</span></span>           |
|<span data-ttu-id="43295-130">code</span><span class="sxs-lookup"><span data-stu-id="43295-130">code</span></span>                          |<span data-ttu-id="43295-131">string</span><span class="sxs-lookup"><span data-stu-id="43295-131">string</span></span>  |<span data-ttu-id="43295-132">指定付款期限代码。</span><span class="sxs-lookup"><span data-stu-id="43295-132">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="43295-133">displayName</span><span class="sxs-lookup"><span data-stu-id="43295-133">displayName</span></span>                   |<span data-ttu-id="43295-134">string</span><span class="sxs-lookup"><span data-stu-id="43295-134">string</span></span>  |<span data-ttu-id="43295-135">指定付款期限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="43295-135">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="43295-136">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="43295-136">dueDateCalculation</span></span>            |<span data-ttu-id="43295-137">string</span><span class="sxs-lookup"><span data-stu-id="43295-137">string</span></span>  |<span data-ttu-id="43295-138">指定用于计算必须进行付款的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="43295-138">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="43295-139">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="43295-139">discountDateCalculation</span></span>       |<span data-ttu-id="43295-140">string</span><span class="sxs-lookup"><span data-stu-id="43295-140">string</span></span>  |<span data-ttu-id="43295-141">指定用于计算要获取折扣付款所必须进行的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="43295-141">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="43295-142">discountPercent</span><span class="sxs-lookup"><span data-stu-id="43295-142">discountPercent</span></span>               |<span data-ttu-id="43295-143">数位</span><span class="sxs-lookup"><span data-stu-id="43295-143">decimal</span></span> |<span data-ttu-id="43295-144">指定针对发票金额的提前付款应用的折扣百分比。</span><span class="sxs-lookup"><span data-stu-id="43295-144">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="43295-145">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="43295-145">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="43295-146">boolean</span><span class="sxs-lookup"><span data-stu-id="43295-146">boolean</span></span> |<span data-ttu-id="43295-147">指定是否应将折扣应用于贷方通知单。</span><span class="sxs-lookup"><span data-stu-id="43295-147">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="43295-148">**如果为 True** ，则表示将提供折扣， **false** 表示不会给出折扣。</span><span class="sxs-lookup"><span data-stu-id="43295-148">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="43295-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43295-149">lastModifiedDateTime</span></span>          |<span data-ttu-id="43295-150">datetime</span><span class="sxs-lookup"><span data-stu-id="43295-150">datetime</span></span>|<span data-ttu-id="43295-151">上次修改 paymentTerms 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="43295-151">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="43295-152">只读。</span><span class="sxs-lookup"><span data-stu-id="43295-152">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="43295-153">关系</span><span class="sxs-lookup"><span data-stu-id="43295-153">Relationships</span></span>
<span data-ttu-id="43295-154">无</span><span class="sxs-lookup"><span data-stu-id="43295-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43295-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43295-155">JSON representation</span></span>

<span data-ttu-id="43295-156">下面是 paymentTerms 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43295-156">Here is a JSON representation of the paymentTerms.</span></span>


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


