---
title: customerPayments 资源类型
description: Dynamics 365 Business Central 中的客户付款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543097"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="3f768-103">customerPayments 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f768-103">customerPayments resource type</span></span>
<span data-ttu-id="3f768-104">代表 Dynamics 365 Business Central 中的客户付款。</span><span class="sxs-lookup"><span data-stu-id="3f768-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="3f768-105">客户付款作为客户付款日志中的一条线路输入。</span><span class="sxs-lookup"><span data-stu-id="3f768-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="3f768-106">方法</span><span class="sxs-lookup"><span data-stu-id="3f768-106">Methods</span></span>

| <span data-ttu-id="3f768-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f768-107">Method</span></span>         | <span data-ttu-id="3f768-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f768-108">Return Type</span></span>  |<span data-ttu-id="3f768-109">说明</span><span class="sxs-lookup"><span data-stu-id="3f768-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="3f768-110">获取 customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="3f768-111">customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-111">customerPayments</span></span>|<span data-ttu-id="3f768-112">获取客户付款。</span><span class="sxs-lookup"><span data-stu-id="3f768-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="3f768-113">Post customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="3f768-114">customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-114">customerPayments</span></span>|<span data-ttu-id="3f768-115">创建客户付款。</span><span class="sxs-lookup"><span data-stu-id="3f768-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="3f768-116">修补程序 customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="3f768-117">customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-117">customerPayments</span></span>|<span data-ttu-id="3f768-118">更新客户付款。</span><span class="sxs-lookup"><span data-stu-id="3f768-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="3f768-119">删除 customerPayments</span><span class="sxs-lookup"><span data-stu-id="3f768-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="3f768-120">无</span><span class="sxs-lookup"><span data-stu-id="3f768-120">none</span></span>|<span data-ttu-id="3f768-121">删除客户付款。</span><span class="sxs-lookup"><span data-stu-id="3f768-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f768-122">属性</span><span class="sxs-lookup"><span data-stu-id="3f768-122">Properties</span></span>
| <span data-ttu-id="3f768-123">属性</span><span class="sxs-lookup"><span data-stu-id="3f768-123">Property</span></span>     | <span data-ttu-id="3f768-124">类型</span><span class="sxs-lookup"><span data-stu-id="3f768-124">Type</span></span>    |<span data-ttu-id="3f768-125">说明</span><span class="sxs-lookup"><span data-stu-id="3f768-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="3f768-126">id</span><span class="sxs-lookup"><span data-stu-id="3f768-126">id</span></span>|<span data-ttu-id="3f768-127">GUID</span><span class="sxs-lookup"><span data-stu-id="3f768-127">GUID</span></span>|<span data-ttu-id="3f768-128">客户付款的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3f768-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="3f768-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="3f768-129">Non-editable.</span></span>|
|<span data-ttu-id="3f768-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="3f768-130">journalDisplayName</span></span>|<span data-ttu-id="3f768-131">string</span><span class="sxs-lookup"><span data-stu-id="3f768-131">string</span></span>|<span data-ttu-id="3f768-132">付款记录所在的行的客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="3f768-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="3f768-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="3f768-133">lineNumber</span></span>|<span data-ttu-id="3f768-134">integer</span><span class="sxs-lookup"><span data-stu-id="3f768-134">integer</span></span>|<span data-ttu-id="3f768-135">客户付款的编号。</span><span class="sxs-lookup"><span data-stu-id="3f768-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="3f768-136">customerId</span><span class="sxs-lookup"><span data-stu-id="3f768-136">customerId</span></span>|<span data-ttu-id="3f768-137">GUID</span><span class="sxs-lookup"><span data-stu-id="3f768-137">GUID</span></span>|<span data-ttu-id="3f768-138">与付款相关的客户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3f768-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="3f768-139">customerNumber</span><span class="sxs-lookup"><span data-stu-id="3f768-139">customerNumber</span></span>|<span data-ttu-id="3f768-140">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3f768-140">string, maximum size 20</span></span>|<span data-ttu-id="3f768-141">与付款相关的客户的编号。</span><span class="sxs-lookup"><span data-stu-id="3f768-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="3f768-142">contactId</span><span class="sxs-lookup"><span data-stu-id="3f768-142">contactId</span></span>|<span data-ttu-id="3f768-143">字符串, 最大大小为250</span><span class="sxs-lookup"><span data-stu-id="3f768-143">string, maximum size 250</span></span>|<span data-ttu-id="3f768-144">给定客户的 exchange 联系人 id。</span><span class="sxs-lookup"><span data-stu-id="3f768-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="3f768-145">如果未指定客户 id, 我们将使用联系人 id 来查找它。</span><span class="sxs-lookup"><span data-stu-id="3f768-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="3f768-146">postingDate</span><span class="sxs-lookup"><span data-stu-id="3f768-146">postingDate</span></span>|<span data-ttu-id="3f768-147">date</span><span class="sxs-lookup"><span data-stu-id="3f768-147">date</span></span>|<span data-ttu-id="3f768-148">客户付款的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="3f768-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="3f768-149">documentNumber</span><span class="sxs-lookup"><span data-stu-id="3f768-149">documentNumber</span></span>|<span data-ttu-id="3f768-150">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3f768-150">string, maximum size 20</span></span>|<span data-ttu-id="3f768-151">指定客户付款的文档编号。</span><span class="sxs-lookup"><span data-stu-id="3f768-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="3f768-152">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="3f768-152">externalDocumentNumber</span></span>|<span data-ttu-id="3f768-153">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3f768-153">string, maximum size 20</span></span>|<span data-ttu-id="3f768-154">指定客户付款的外部文档编号。</span><span class="sxs-lookup"><span data-stu-id="3f768-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="3f768-155">量</span><span class="sxs-lookup"><span data-stu-id="3f768-155">amount</span></span>|<span data-ttu-id="3f768-156">数位</span><span class="sxs-lookup"><span data-stu-id="3f768-156">decimal</span></span>|<span data-ttu-id="3f768-157">指定客户付款包含的总金额 (包括 VAT)。</span><span class="sxs-lookup"><span data-stu-id="3f768-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="3f768-158">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="3f768-158">appliesToInvoiceId</span></span>|<span data-ttu-id="3f768-159">GUID</span><span class="sxs-lookup"><span data-stu-id="3f768-159">GUID</span></span>|<span data-ttu-id="3f768-160">与付款相关的发票的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="3f768-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="3f768-161">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="3f768-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="3f768-162">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="3f768-162">string, maximum size 20</span></span>|<span data-ttu-id="3f768-163">与付款相关的发票的编号。</span><span class="sxs-lookup"><span data-stu-id="3f768-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="3f768-164">description</span><span class="sxs-lookup"><span data-stu-id="3f768-164">description</span></span>|<span data-ttu-id="3f768-165">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="3f768-165">string, maximum size 50</span></span>|<span data-ttu-id="3f768-166">客户付款的说明, 由用户或 autocreated 提供。</span><span class="sxs-lookup"><span data-stu-id="3f768-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="3f768-167">注释</span><span class="sxs-lookup"><span data-stu-id="3f768-167">comment</span></span>|<span data-ttu-id="3f768-168">字符串, 最大大小为250</span><span class="sxs-lookup"><span data-stu-id="3f768-168">string, maximum size 250</span></span>|<span data-ttu-id="3f768-169">用户在客户付款上指定的注释。</span><span class="sxs-lookup"><span data-stu-id="3f768-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="3f768-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f768-170">lastModifiedDateTime</span></span>|<span data-ttu-id="3f768-171">datetime</span><span class="sxs-lookup"><span data-stu-id="3f768-171">datetime</span></span>|<span data-ttu-id="3f768-172">客户付款修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3f768-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="3f768-173">只读。</span><span class="sxs-lookup"><span data-stu-id="3f768-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3f768-174">关系</span><span class="sxs-lookup"><span data-stu-id="3f768-174">Relationships</span></span>
<span data-ttu-id="3f768-175">客户付款是客户付款日志的子页面。</span><span class="sxs-lookup"><span data-stu-id="3f768-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="3f768-176">不能直接访问它。</span><span class="sxs-lookup"><span data-stu-id="3f768-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="3f768-177">客户付款可以是维行的 "父实体"。</span><span class="sxs-lookup"><span data-stu-id="3f768-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="3f768-178">客户 (customerId) 必须存在于 Customers 表中。</span><span class="sxs-lookup"><span data-stu-id="3f768-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="3f768-179">发票 (appliesToInvoiceId) 必须存在于 "销售发票" 表中。</span><span class="sxs-lookup"><span data-stu-id="3f768-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f768-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f768-180">JSON representation</span></span>

<span data-ttu-id="3f768-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f768-181">Here is a JSON representation of the resource.</span></span>

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

