---
title: paymentTerms 资源类型
description: Dynamics 365 Business Central 中的付款条款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507327"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="328a2-103">paymentTerms 资源类型</span><span class="sxs-lookup"><span data-stu-id="328a2-103">paymentTerms resource type</span></span>
<span data-ttu-id="328a2-104">表示 Dynamics 365 Business Central 中的付款期限。</span><span class="sxs-lookup"><span data-stu-id="328a2-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="328a2-105">方法</span><span class="sxs-lookup"><span data-stu-id="328a2-105">Methods</span></span>

| <span data-ttu-id="328a2-106">方法</span><span class="sxs-lookup"><span data-stu-id="328a2-106">Method</span></span>                                                      | <span data-ttu-id="328a2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="328a2-107">Return Type</span></span>|<span data-ttu-id="328a2-108">说明</span><span class="sxs-lookup"><span data-stu-id="328a2-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="328a2-109">获取 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="328a2-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-110">paymentTerms</span></span>|<span data-ttu-id="328a2-111">获取付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="328a2-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="328a2-112">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="328a2-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-113">paymentTerms</span></span>|<span data-ttu-id="328a2-114">创建付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="328a2-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="328a2-115">修补程序 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="328a2-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-116">paymentTerms</span></span>|<span data-ttu-id="328a2-117">更新付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="328a2-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="328a2-118">删除 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="328a2-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="328a2-119">无</span><span class="sxs-lookup"><span data-stu-id="328a2-119">none</span></span>        |<span data-ttu-id="328a2-120">删除付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="328a2-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="328a2-121">属性</span><span class="sxs-lookup"><span data-stu-id="328a2-121">Properties</span></span>
| <span data-ttu-id="328a2-122">属性</span><span class="sxs-lookup"><span data-stu-id="328a2-122">Property</span></span>                     | <span data-ttu-id="328a2-123">类型</span><span class="sxs-lookup"><span data-stu-id="328a2-123">Type</span></span>     |<span data-ttu-id="328a2-124">说明</span><span class="sxs-lookup"><span data-stu-id="328a2-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="328a2-125">id</span><span class="sxs-lookup"><span data-stu-id="328a2-125">id</span></span>                            |<span data-ttu-id="328a2-126">GUID</span><span class="sxs-lookup"><span data-stu-id="328a2-126">GUID</span></span>    |<span data-ttu-id="328a2-127">paymentTerms 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="328a2-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="328a2-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="328a2-128">Non-editable.</span></span>           |
|<span data-ttu-id="328a2-129">code</span><span class="sxs-lookup"><span data-stu-id="328a2-129">code</span></span>                          |<span data-ttu-id="328a2-130">string</span><span class="sxs-lookup"><span data-stu-id="328a2-130">string</span></span>  |<span data-ttu-id="328a2-131">指定付款期限代码。</span><span class="sxs-lookup"><span data-stu-id="328a2-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="328a2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="328a2-132">displayName</span></span>                   |<span data-ttu-id="328a2-133">string</span><span class="sxs-lookup"><span data-stu-id="328a2-133">string</span></span>  |<span data-ttu-id="328a2-134">指定付款期限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="328a2-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="328a2-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="328a2-135">dueDateCalculation</span></span>            |<span data-ttu-id="328a2-136">字符串</span><span class="sxs-lookup"><span data-stu-id="328a2-136">string</span></span>  |<span data-ttu-id="328a2-137">指定用于计算必须进行付款的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="328a2-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="328a2-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="328a2-138">discountDateCalculation</span></span>       |<span data-ttu-id="328a2-139">字符串</span><span class="sxs-lookup"><span data-stu-id="328a2-139">string</span></span>  |<span data-ttu-id="328a2-140">指定用于计算要获取折扣付款所必须进行的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="328a2-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="328a2-141">discountPercent</span><span class="sxs-lookup"><span data-stu-id="328a2-141">discountPercent</span></span>               |<span data-ttu-id="328a2-142">数位</span><span class="sxs-lookup"><span data-stu-id="328a2-142">decimal</span></span> |<span data-ttu-id="328a2-143">指定针对发票金额的提前付款应用的折扣百分比。</span><span class="sxs-lookup"><span data-stu-id="328a2-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="328a2-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="328a2-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="328a2-145">布尔</span><span class="sxs-lookup"><span data-stu-id="328a2-145">boolean</span></span> |<span data-ttu-id="328a2-146">指定是否应将折扣应用于贷方通知单。</span><span class="sxs-lookup"><span data-stu-id="328a2-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="328a2-147">**如果为 True** , 则表示将提供折扣, **false**表示不会给出折扣。</span><span class="sxs-lookup"><span data-stu-id="328a2-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="328a2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="328a2-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="328a2-149">datetime</span><span class="sxs-lookup"><span data-stu-id="328a2-149">datetime</span></span>|<span data-ttu-id="328a2-150">上次修改 paymentTerms 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="328a2-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="328a2-151">只读。</span><span class="sxs-lookup"><span data-stu-id="328a2-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="328a2-152">关系</span><span class="sxs-lookup"><span data-stu-id="328a2-152">Relationships</span></span>
<span data-ttu-id="328a2-153">无</span><span class="sxs-lookup"><span data-stu-id="328a2-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="328a2-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="328a2-154">JSON representation</span></span>

<span data-ttu-id="328a2-155">下面是 paymentTerms 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="328a2-155">Here is a JSON representation of the paymentTerms.</span></span>


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
