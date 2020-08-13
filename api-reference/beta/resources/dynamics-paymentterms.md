---
title: paymentTerms 资源类型
description: Dynamics 365 Business Central 中的付款条款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cf6917b724f9e35735d63d1cda13c01d6f9003bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503598"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="0b1e1-103">paymentTerms 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b1e1-103">paymentTerms resource type</span></span>

<span data-ttu-id="0b1e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b1e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b1e1-105">表示 Dynamics 365 Business Central 中的付款期限。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-105">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0b1e1-106">方法</span><span class="sxs-lookup"><span data-stu-id="0b1e1-106">Methods</span></span>

| <span data-ttu-id="0b1e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="0b1e1-107">Method</span></span>                                                      | <span data-ttu-id="0b1e1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b1e1-108">Return Type</span></span>|<span data-ttu-id="0b1e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b1e1-109">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="0b1e1-110">获取 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-110">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="0b1e1-111">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-111">paymentTerms</span></span>|<span data-ttu-id="0b1e1-112">获取付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-112">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="0b1e1-113">Post paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-113">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="0b1e1-114">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-114">paymentTerms</span></span>|<span data-ttu-id="0b1e1-115">创建付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-115">Create a payment terms object.</span></span>|
|[<span data-ttu-id="0b1e1-116">修补程序 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-116">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="0b1e1-117">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-117">paymentTerms</span></span>|<span data-ttu-id="0b1e1-118">更新付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-118">Update a payment terms object.</span></span>|
|[<span data-ttu-id="0b1e1-119">删除 paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0b1e1-119">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="0b1e1-120">无</span><span class="sxs-lookup"><span data-stu-id="0b1e1-120">none</span></span>        |<span data-ttu-id="0b1e1-121">删除付款期限对象。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-121">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b1e1-122">属性</span><span class="sxs-lookup"><span data-stu-id="0b1e1-122">Properties</span></span>
| <span data-ttu-id="0b1e1-123">属性</span><span class="sxs-lookup"><span data-stu-id="0b1e1-123">Property</span></span>                     | <span data-ttu-id="0b1e1-124">类型</span><span class="sxs-lookup"><span data-stu-id="0b1e1-124">Type</span></span>     |<span data-ttu-id="0b1e1-125">说明</span><span class="sxs-lookup"><span data-stu-id="0b1e1-125">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="0b1e1-126">id</span><span class="sxs-lookup"><span data-stu-id="0b1e1-126">id</span></span>                            |<span data-ttu-id="0b1e1-127">GUID</span><span class="sxs-lookup"><span data-stu-id="0b1e1-127">GUID</span></span>    |<span data-ttu-id="0b1e1-128">PaymentTerms 的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-128">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="0b1e1-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-129">Non-editable.</span></span>           |
|<span data-ttu-id="0b1e1-130">code</span><span class="sxs-lookup"><span data-stu-id="0b1e1-130">code</span></span>                          |<span data-ttu-id="0b1e1-131">string</span><span class="sxs-lookup"><span data-stu-id="0b1e1-131">string</span></span>  |<span data-ttu-id="0b1e1-132">指定付款期限代码。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-132">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="0b1e1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b1e1-133">displayName</span></span>                   |<span data-ttu-id="0b1e1-134">string</span><span class="sxs-lookup"><span data-stu-id="0b1e1-134">string</span></span>  |<span data-ttu-id="0b1e1-135">指定付款期限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-135">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="0b1e1-136">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="0b1e1-136">dueDateCalculation</span></span>            |<span data-ttu-id="0b1e1-137">string</span><span class="sxs-lookup"><span data-stu-id="0b1e1-137">string</span></span>  |<span data-ttu-id="0b1e1-138">指定用于计算必须进行付款的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-138">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="0b1e1-139">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="0b1e1-139">discountDateCalculation</span></span>       |<span data-ttu-id="0b1e1-140">string</span><span class="sxs-lookup"><span data-stu-id="0b1e1-140">string</span></span>  |<span data-ttu-id="0b1e1-141">指定用于计算要获取折扣付款所必须进行的日期的公式。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-141">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="0b1e1-142">discountPercent</span><span class="sxs-lookup"><span data-stu-id="0b1e1-142">discountPercent</span></span>               |<span data-ttu-id="0b1e1-143">数位</span><span class="sxs-lookup"><span data-stu-id="0b1e1-143">decimal</span></span> |<span data-ttu-id="0b1e1-144">指定针对发票金额的提前付款应用的折扣百分比。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-144">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="0b1e1-145">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="0b1e1-145">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="0b1e1-146">boolean</span><span class="sxs-lookup"><span data-stu-id="0b1e1-146">boolean</span></span> |<span data-ttu-id="0b1e1-147">指定是否应将折扣应用于贷方通知单。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-147">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="0b1e1-148">**如果为 True** ，则表示将提供折扣， **false**表示不会给出折扣。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-148">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="0b1e1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b1e1-149">lastModifiedDateTime</span></span>          |<span data-ttu-id="0b1e1-150">datetime</span><span class="sxs-lookup"><span data-stu-id="0b1e1-150">datetime</span></span>|<span data-ttu-id="0b1e1-151">上次修改 paymentTerms 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-151">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="0b1e1-152">只读。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-152">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="0b1e1-153">关系</span><span class="sxs-lookup"><span data-stu-id="0b1e1-153">Relationships</span></span>
<span data-ttu-id="0b1e1-154">无</span><span class="sxs-lookup"><span data-stu-id="0b1e1-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b1e1-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b1e1-155">JSON representation</span></span>

<span data-ttu-id="0b1e1-156">下面是 paymentTerms 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b1e1-156">Here is a JSON representation of the paymentTerms.</span></span>


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
