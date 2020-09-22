---
title: customerPayments 资源类型
description: Dynamics 365 Business Central 中的客户付款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bf5536181f965765615a7e2d707d6503813cfb76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040040"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="7efd8-103">customerPayments 资源类型</span><span class="sxs-lookup"><span data-stu-id="7efd8-103">customerPayments resource type</span></span>

<span data-ttu-id="7efd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7efd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7efd8-105">代表 Dynamics 365 Business Central 中的客户付款。</span><span class="sxs-lookup"><span data-stu-id="7efd8-105">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="7efd8-106">客户付款作为客户付款日志中的一条线路输入。</span><span class="sxs-lookup"><span data-stu-id="7efd8-106">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="7efd8-107">方法</span><span class="sxs-lookup"><span data-stu-id="7efd8-107">Methods</span></span>

| <span data-ttu-id="7efd8-108">方法</span><span class="sxs-lookup"><span data-stu-id="7efd8-108">Method</span></span>         | <span data-ttu-id="7efd8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7efd8-109">Return Type</span></span>  |<span data-ttu-id="7efd8-110">说明</span><span class="sxs-lookup"><span data-stu-id="7efd8-110">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="7efd8-111">获取 customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-111">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="7efd8-112">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-112">customerPayments</span></span>|<span data-ttu-id="7efd8-113">获取客户付款。</span><span class="sxs-lookup"><span data-stu-id="7efd8-113">Gets a customer payment.</span></span>|
|[<span data-ttu-id="7efd8-114">Post customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-114">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="7efd8-115">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-115">customerPayments</span></span>|<span data-ttu-id="7efd8-116">创建客户付款。</span><span class="sxs-lookup"><span data-stu-id="7efd8-116">Creates a customer payment.</span></span>|
|[<span data-ttu-id="7efd8-117">修补程序 customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-117">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="7efd8-118">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-118">customerPayments</span></span>|<span data-ttu-id="7efd8-119">更新客户付款。</span><span class="sxs-lookup"><span data-stu-id="7efd8-119">Updates a customer payment.</span></span>|
|[<span data-ttu-id="7efd8-120">删除 customerPayments</span><span class="sxs-lookup"><span data-stu-id="7efd8-120">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="7efd8-121">无</span><span class="sxs-lookup"><span data-stu-id="7efd8-121">none</span></span>|<span data-ttu-id="7efd8-122">删除客户付款。</span><span class="sxs-lookup"><span data-stu-id="7efd8-122">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="7efd8-123">属性</span><span class="sxs-lookup"><span data-stu-id="7efd8-123">Properties</span></span>
| <span data-ttu-id="7efd8-124">属性</span><span class="sxs-lookup"><span data-stu-id="7efd8-124">Property</span></span>     | <span data-ttu-id="7efd8-125">类型</span><span class="sxs-lookup"><span data-stu-id="7efd8-125">Type</span></span>    |<span data-ttu-id="7efd8-126">说明</span><span class="sxs-lookup"><span data-stu-id="7efd8-126">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="7efd8-127">id</span><span class="sxs-lookup"><span data-stu-id="7efd8-127">id</span></span>|<span data-ttu-id="7efd8-128">GUID</span><span class="sxs-lookup"><span data-stu-id="7efd8-128">GUID</span></span>|<span data-ttu-id="7efd8-129">客户付款的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="7efd8-129">The unique ID of the customer payment.</span></span> <span data-ttu-id="7efd8-130">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="7efd8-130">Non-editable.</span></span>|
|<span data-ttu-id="7efd8-131">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="7efd8-131">journalDisplayName</span></span>|<span data-ttu-id="7efd8-132">string</span><span class="sxs-lookup"><span data-stu-id="7efd8-132">string</span></span>|<span data-ttu-id="7efd8-133">付款记录所在的行的客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="7efd8-133">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="7efd8-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="7efd8-134">lineNumber</span></span>|<span data-ttu-id="7efd8-135">integer</span><span class="sxs-lookup"><span data-stu-id="7efd8-135">integer</span></span>|<span data-ttu-id="7efd8-136">客户付款的编号。</span><span class="sxs-lookup"><span data-stu-id="7efd8-136">The number of the customer payment.</span></span>|
|<span data-ttu-id="7efd8-137">customerId</span><span class="sxs-lookup"><span data-stu-id="7efd8-137">customerId</span></span>|<span data-ttu-id="7efd8-138">GUID</span><span class="sxs-lookup"><span data-stu-id="7efd8-138">GUID</span></span>|<span data-ttu-id="7efd8-139">与付款相关的客户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="7efd8-139">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="7efd8-140">customerNumber</span><span class="sxs-lookup"><span data-stu-id="7efd8-140">customerNumber</span></span>|<span data-ttu-id="7efd8-141">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="7efd8-141">string, maximum size 20</span></span>|<span data-ttu-id="7efd8-142">与付款相关的客户的编号。</span><span class="sxs-lookup"><span data-stu-id="7efd8-142">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="7efd8-143">contactId</span><span class="sxs-lookup"><span data-stu-id="7efd8-143">contactId</span></span>|<span data-ttu-id="7efd8-144">字符串，最大大小为250</span><span class="sxs-lookup"><span data-stu-id="7efd8-144">string, maximum size 250</span></span>|<span data-ttu-id="7efd8-145">给定客户的 exchange 联系人 id。</span><span class="sxs-lookup"><span data-stu-id="7efd8-145">The exchange contact id for the given customer.</span></span> <span data-ttu-id="7efd8-146">如果未指定客户 id，我们将使用联系人 id 来查找它。</span><span class="sxs-lookup"><span data-stu-id="7efd8-146">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="7efd8-147">postingDate</span><span class="sxs-lookup"><span data-stu-id="7efd8-147">postingDate</span></span>|<span data-ttu-id="7efd8-148">date</span><span class="sxs-lookup"><span data-stu-id="7efd8-148">date</span></span>|<span data-ttu-id="7efd8-149">客户付款的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="7efd8-149">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="7efd8-150">documentNumber</span><span class="sxs-lookup"><span data-stu-id="7efd8-150">documentNumber</span></span>|<span data-ttu-id="7efd8-151">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="7efd8-151">string, maximum size 20</span></span>|<span data-ttu-id="7efd8-152">指定客户付款的文档编号。</span><span class="sxs-lookup"><span data-stu-id="7efd8-152">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="7efd8-153">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="7efd8-153">externalDocumentNumber</span></span>|<span data-ttu-id="7efd8-154">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="7efd8-154">string, maximum size 20</span></span>|<span data-ttu-id="7efd8-155">指定客户付款的外部文档编号。</span><span class="sxs-lookup"><span data-stu-id="7efd8-155">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="7efd8-156">量</span><span class="sxs-lookup"><span data-stu-id="7efd8-156">amount</span></span>|<span data-ttu-id="7efd8-157">数位</span><span class="sxs-lookup"><span data-stu-id="7efd8-157">decimal</span></span>|<span data-ttu-id="7efd8-158">指定客户付款包含的增值税)  (总金额。</span><span class="sxs-lookup"><span data-stu-id="7efd8-158">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="7efd8-159">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="7efd8-159">appliesToInvoiceId</span></span>|<span data-ttu-id="7efd8-160">GUID</span><span class="sxs-lookup"><span data-stu-id="7efd8-160">GUID</span></span>|<span data-ttu-id="7efd8-161">与付款相关的发票的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="7efd8-161">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="7efd8-162">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="7efd8-162">appliesToInvoiceNumber</span></span>|<span data-ttu-id="7efd8-163">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="7efd8-163">string, maximum size 20</span></span>|<span data-ttu-id="7efd8-164">与付款相关的发票的编号。</span><span class="sxs-lookup"><span data-stu-id="7efd8-164">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="7efd8-165">description</span><span class="sxs-lookup"><span data-stu-id="7efd8-165">description</span></span>|<span data-ttu-id="7efd8-166">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="7efd8-166">string, maximum size 50</span></span>|<span data-ttu-id="7efd8-167">客户付款的说明，由用户或 autocreated 提供。</span><span class="sxs-lookup"><span data-stu-id="7efd8-167">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="7efd8-168">comment</span><span class="sxs-lookup"><span data-stu-id="7efd8-168">comment</span></span>|<span data-ttu-id="7efd8-169">字符串，最大大小为250</span><span class="sxs-lookup"><span data-stu-id="7efd8-169">string, maximum size 250</span></span>|<span data-ttu-id="7efd8-170">用户在客户付款上指定的注释。</span><span class="sxs-lookup"><span data-stu-id="7efd8-170">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="7efd8-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7efd8-171">lastModifiedDateTime</span></span>|<span data-ttu-id="7efd8-172">datetime</span><span class="sxs-lookup"><span data-stu-id="7efd8-172">datetime</span></span>|<span data-ttu-id="7efd8-173">客户付款修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7efd8-173">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="7efd8-174">只读。</span><span class="sxs-lookup"><span data-stu-id="7efd8-174">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7efd8-175">关系</span><span class="sxs-lookup"><span data-stu-id="7efd8-175">Relationships</span></span>
<span data-ttu-id="7efd8-176">客户付款是客户付款日志的子页面。</span><span class="sxs-lookup"><span data-stu-id="7efd8-176">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="7efd8-177">不能直接访问它。</span><span class="sxs-lookup"><span data-stu-id="7efd8-177">It cannot be accessed directly.</span></span>

<span data-ttu-id="7efd8-178">客户付款可以是维行的 "父实体"。</span><span class="sxs-lookup"><span data-stu-id="7efd8-178">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="7efd8-179">客户 (customerId) 必须存在于 Customers 表中。</span><span class="sxs-lookup"><span data-stu-id="7efd8-179">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="7efd8-180">发票 (appliesToInvoiceId) 必须存在于销售发票表中。</span><span class="sxs-lookup"><span data-stu-id="7efd8-180">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7efd8-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7efd8-181">JSON representation</span></span>

<span data-ttu-id="7efd8-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7efd8-182">Here is a JSON representation of the resource.</span></span>

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



