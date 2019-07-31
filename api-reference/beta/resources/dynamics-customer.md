---
title: customers 资源类型
description: 代表 Dynamics 365 Business Central 中的客户。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2a3ad7bade33af9456e65e3c19b988b9d2f679b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973637"
---
# <a name="customers-resource-type"></a><span data-ttu-id="ca4ec-103">customers 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca4ec-103">customers resource type</span></span>
<span data-ttu-id="ca4ec-104">代表 Dynamics 365 Business Central 中的客户。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ca4ec-105">方法</span><span class="sxs-lookup"><span data-stu-id="ca4ec-105">Methods</span></span>

| <span data-ttu-id="ca4ec-106">方法</span><span class="sxs-lookup"><span data-stu-id="ca4ec-106">Method</span></span>                                              |<span data-ttu-id="ca4ec-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca4ec-107">Return Type</span></span>| <span data-ttu-id="ca4ec-108">说明</span><span class="sxs-lookup"><span data-stu-id="ca4ec-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="ca4ec-109">获取客户</span><span class="sxs-lookup"><span data-stu-id="ca4ec-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="ca4ec-110">各地</span><span class="sxs-lookup"><span data-stu-id="ca4ec-110">customers</span></span>   |<span data-ttu-id="ca4ec-111">获取客户。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="ca4ec-112">创建客户</span><span class="sxs-lookup"><span data-stu-id="ca4ec-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="ca4ec-113">各地</span><span class="sxs-lookup"><span data-stu-id="ca4ec-113">customers</span></span>   |<span data-ttu-id="ca4ec-114">创建客户。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-114">Creates a customer.</span></span>|
|[<span data-ttu-id="ca4ec-115">更新客户</span><span class="sxs-lookup"><span data-stu-id="ca4ec-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="ca4ec-116">各地</span><span class="sxs-lookup"><span data-stu-id="ca4ec-116">customers</span></span>   |<span data-ttu-id="ca4ec-117">更新客户。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-117">Updates a customer.</span></span>|
|[<span data-ttu-id="ca4ec-118">删除客户</span><span class="sxs-lookup"><span data-stu-id="ca4ec-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="ca4ec-119">无</span><span class="sxs-lookup"><span data-stu-id="ca4ec-119">none</span></span>        |<span data-ttu-id="ca4ec-120">删除客户。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca4ec-121">属性</span><span class="sxs-lookup"><span data-stu-id="ca4ec-121">Properties</span></span>
| <span data-ttu-id="ca4ec-122">属性</span><span class="sxs-lookup"><span data-stu-id="ca4ec-122">Property</span></span>    | <span data-ttu-id="ca4ec-123">类型</span><span class="sxs-lookup"><span data-stu-id="ca4ec-123">Type</span></span>     |<span data-ttu-id="ca4ec-124">说明</span><span class="sxs-lookup"><span data-stu-id="ca4ec-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="ca4ec-125">id</span><span class="sxs-lookup"><span data-stu-id="ca4ec-125">id</span></span>           |<span data-ttu-id="ca4ec-126">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-126">GUID</span></span>      |<span data-ttu-id="ca4ec-127">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-127">The unique ID of the item.</span></span> <span data-ttu-id="ca4ec-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-128">Non-editable.</span></span>|
|<span data-ttu-id="ca4ec-129">number</span><span class="sxs-lookup"><span data-stu-id="ca4ec-129">number</span></span>       |<span data-ttu-id="ca4ec-130">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-130">string</span></span>    |<span data-ttu-id="ca4ec-131">客户编号。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-131">The customer number.</span></span>|
|<span data-ttu-id="ca4ec-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ca4ec-132">displayName</span></span>  |<span data-ttu-id="ca4ec-133">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-133">string</span></span>    |<span data-ttu-id="ca4ec-134">指定客户的名称。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-134">Specifies the customer's name.</span></span> <span data-ttu-id="ca4ec-135">此名称将显示在客户的所有销售文档中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ca4ec-136">类型</span><span class="sxs-lookup"><span data-stu-id="ca4ec-136">type</span></span>         |<span data-ttu-id="ca4ec-137">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-137">string</span></span>    |<span data-ttu-id="ca4ec-138">指定客户类型, 可以是 "Company", 也可以是 "Person"。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="ca4ec-139">address</span><span class="sxs-lookup"><span data-stu-id="ca4ec-139">address</span></span>      |[<span data-ttu-id="ca4ec-140">翻.省略</span><span class="sxs-lookup"><span data-stu-id="ca4ec-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ca4ec-141">指定客户地址。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-141">Specifies the customer's address.</span></span> <span data-ttu-id="ca4ec-142">此地址将显示在客户的所有销售文档中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ca4ec-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ca4ec-143">phoneNumber</span></span>  |<span data-ttu-id="ca4ec-144">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-144">string</span></span>    |<span data-ttu-id="ca4ec-145">指定客户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="ca4ec-146">email</span><span class="sxs-lookup"><span data-stu-id="ca4ec-146">email</span></span>        |<span data-ttu-id="ca4ec-147">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-147">string</span></span>    |<span data-ttu-id="ca4ec-148">指定客户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="ca4ec-149">website</span><span class="sxs-lookup"><span data-stu-id="ca4ec-149">website</span></span>      |<span data-ttu-id="ca4ec-150">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-150">string</span></span>    |<span data-ttu-id="ca4ec-151">指定客户的主页地址。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="ca4ec-152">taxLiable</span><span class="sxs-lookup"><span data-stu-id="ca4ec-152">taxLiable</span></span>    |<span data-ttu-id="ca4ec-153">boolean</span><span class="sxs-lookup"><span data-stu-id="ca4ec-153">boolean</span></span>   |<span data-ttu-id="ca4ec-154">指定客户或供应商是否对销售税负有义务。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="ca4ec-155">如果客户有义务责任, 则设置为**true** 。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="ca4ec-156">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="ca4ec-156">taxAreaId</span></span>    |<span data-ttu-id="ca4ec-157">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-157">GUID</span></span>      |<span data-ttu-id="ca4ec-158">指定客户所属的税务区域。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ca4ec-159">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca4ec-159">taxAreaDisplayName</span></span>|<span data-ttu-id="ca4ec-160">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-160">string</span></span>|<span data-ttu-id="ca4ec-161">指定客户所属的税务区域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ca4ec-162">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="ca4ec-162">taxRegistrationNumber</span></span>|<span data-ttu-id="ca4ec-163">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="ca4ec-163">string, maximum size 20</span></span>|<span data-ttu-id="ca4ec-164">指定客户的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="ca4ec-165">currencyId</span><span class="sxs-lookup"><span data-stu-id="ca4ec-165">currencyId</span></span>   |<span data-ttu-id="ca4ec-166">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-166">GUID</span></span>      |<span data-ttu-id="ca4ec-167">指定客户使用的货币。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="ca4ec-168">currencyCode</span><span class="sxs-lookup"><span data-stu-id="ca4ec-168">currencyCode</span></span> |<span data-ttu-id="ca4ec-169">位数</span><span class="sxs-lookup"><span data-stu-id="ca4ec-169">numeric</span></span>   |<span data-ttu-id="ca4ec-170">客户的默认货币代码。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="ca4ec-171">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="ca4ec-171">paymentTermsId</span></span>|<span data-ttu-id="ca4ec-172">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-172">GUID</span></span>     |<span data-ttu-id="ca4ec-173">指定客户使用的付款期限。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="ca4ec-174">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="ca4ec-174">paymentMethodId</span></span>|<span data-ttu-id="ca4ec-175">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-175">GUID</span></span>    |<span data-ttu-id="ca4ec-176">指定客户使用的支付方式。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="ca4ec-177">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="ca4ec-177">shipmentMethodId</span></span>|<span data-ttu-id="ca4ec-178">GUID</span><span class="sxs-lookup"><span data-stu-id="ca4ec-178">GUID</span></span>   |<span data-ttu-id="ca4ec-179">指定客户使用的装运方法。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="ca4ec-180">堵塞</span><span class="sxs-lookup"><span data-stu-id="ca4ec-180">blocked</span></span>      |<span data-ttu-id="ca4ec-181">string</span><span class="sxs-lookup"><span data-stu-id="ca4ec-181">string</span></span>    |<span data-ttu-id="ca4ec-182">指定无法对客户的交易记录进行过帐。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="ca4ec-183">设置为**All**, 如果客户被阻止, 则设置为空 (如果未阻止)。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="ca4ec-184">恰好</span><span class="sxs-lookup"><span data-stu-id="ca4ec-184">balance</span></span>      |<span data-ttu-id="ca4ec-185">位数</span><span class="sxs-lookup"><span data-stu-id="ca4ec-185">numeric</span></span>   |<span data-ttu-id="ca4ec-186">指定客户为完成的销售而支付的付款金额。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="ca4ec-187">此值也称为客户余额。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="ca4ec-188">只读。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-188">Read-Only.</span></span>|
|<span data-ttu-id="ca4ec-189">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="ca4ec-189">overdueAmount</span></span>|<span data-ttu-id="ca4ec-190">位数</span><span class="sxs-lookup"><span data-stu-id="ca4ec-190">numeric</span></span>   |<span data-ttu-id="ca4ec-191">指定客户的逾期金额。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="ca4ec-192">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="ca4ec-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="ca4ec-193">位数</span><span class="sxs-lookup"><span data-stu-id="ca4ec-193">numeric</span></span>|<span data-ttu-id="ca4ec-194">指定不包括客户税的总销售额。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="ca4ec-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4ec-195">lastModifiedDateTime</span></span>|<span data-ttu-id="ca4ec-196">datetime</span><span class="sxs-lookup"><span data-stu-id="ca4ec-196">datetime</span></span>|<span data-ttu-id="ca4ec-197">客户修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="ca4ec-198">只读。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ca4ec-199">关系</span><span class="sxs-lookup"><span data-stu-id="ca4ec-199">Relationships</span></span>
<span data-ttu-id="ca4ec-200">货币 (currencyCode) 必须在货币表中存在。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="ca4ec-201">付款期限 (paymentTerms) 必须存在于付款条款表中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="ca4ec-202">装运方法 (shipmentMethod) 必须存在于装运方法表中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="ca4ec-203">付款方法 (paymentMethod) 必须存在于付款方法表中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="ca4ec-204">税务区域 (taxArea) 必须存在于税务区域表中。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca4ec-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca4ec-205">JSON representation</span></span>

<span data-ttu-id="ca4ec-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca4ec-206">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

