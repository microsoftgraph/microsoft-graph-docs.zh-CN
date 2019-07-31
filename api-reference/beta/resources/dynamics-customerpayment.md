---
title: customerPayments 资源类型
description: Dynamics 365 Business Central 中的客户付款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4a1c777d51dd1ba706af85f431162cda16b5d25b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012602"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="db829-103">customerPayments 资源类型</span><span class="sxs-lookup"><span data-stu-id="db829-103">customerPayments resource type</span></span>
<span data-ttu-id="db829-104">代表 Dynamics 365 Business Central 中的客户付款。</span><span class="sxs-lookup"><span data-stu-id="db829-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="db829-105">客户付款作为客户付款日志中的一条线路输入。</span><span class="sxs-lookup"><span data-stu-id="db829-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="db829-106">方法</span><span class="sxs-lookup"><span data-stu-id="db829-106">Methods</span></span>

| <span data-ttu-id="db829-107">方法</span><span class="sxs-lookup"><span data-stu-id="db829-107">Method</span></span>         | <span data-ttu-id="db829-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="db829-108">Return Type</span></span>  |<span data-ttu-id="db829-109">说明</span><span class="sxs-lookup"><span data-stu-id="db829-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="db829-110">获取 customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="db829-111">customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-111">customerPayments</span></span>|<span data-ttu-id="db829-112">获取客户付款。</span><span class="sxs-lookup"><span data-stu-id="db829-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="db829-113">Post customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="db829-114">customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-114">customerPayments</span></span>|<span data-ttu-id="db829-115">创建客户付款。</span><span class="sxs-lookup"><span data-stu-id="db829-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="db829-116">修补程序 customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="db829-117">customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-117">customerPayments</span></span>|<span data-ttu-id="db829-118">更新客户付款。</span><span class="sxs-lookup"><span data-stu-id="db829-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="db829-119">删除 customerPayments</span><span class="sxs-lookup"><span data-stu-id="db829-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="db829-120">无</span><span class="sxs-lookup"><span data-stu-id="db829-120">none</span></span>|<span data-ttu-id="db829-121">删除客户付款。</span><span class="sxs-lookup"><span data-stu-id="db829-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="db829-122">属性</span><span class="sxs-lookup"><span data-stu-id="db829-122">Properties</span></span>
| <span data-ttu-id="db829-123">属性</span><span class="sxs-lookup"><span data-stu-id="db829-123">Property</span></span>     | <span data-ttu-id="db829-124">类型</span><span class="sxs-lookup"><span data-stu-id="db829-124">Type</span></span>    |<span data-ttu-id="db829-125">说明</span><span class="sxs-lookup"><span data-stu-id="db829-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="db829-126">id</span><span class="sxs-lookup"><span data-stu-id="db829-126">id</span></span>|<span data-ttu-id="db829-127">GUID</span><span class="sxs-lookup"><span data-stu-id="db829-127">GUID</span></span>|<span data-ttu-id="db829-128">客户付款的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="db829-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="db829-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="db829-129">Non-editable.</span></span>|
|<span data-ttu-id="db829-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="db829-130">journalDisplayName</span></span>|<span data-ttu-id="db829-131">string</span><span class="sxs-lookup"><span data-stu-id="db829-131">string</span></span>|<span data-ttu-id="db829-132">付款记录所在的行的客户付款日志。</span><span class="sxs-lookup"><span data-stu-id="db829-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="db829-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="db829-133">lineNumber</span></span>|<span data-ttu-id="db829-134">integer</span><span class="sxs-lookup"><span data-stu-id="db829-134">integer</span></span>|<span data-ttu-id="db829-135">客户付款的编号。</span><span class="sxs-lookup"><span data-stu-id="db829-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="db829-136">customerId</span><span class="sxs-lookup"><span data-stu-id="db829-136">customerId</span></span>|<span data-ttu-id="db829-137">GUID</span><span class="sxs-lookup"><span data-stu-id="db829-137">GUID</span></span>|<span data-ttu-id="db829-138">与付款相关的客户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="db829-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="db829-139">customerNumber</span><span class="sxs-lookup"><span data-stu-id="db829-139">customerNumber</span></span>|<span data-ttu-id="db829-140">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="db829-140">string, maximum size 20</span></span>|<span data-ttu-id="db829-141">与付款相关的客户的编号。</span><span class="sxs-lookup"><span data-stu-id="db829-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="db829-142">contactId</span><span class="sxs-lookup"><span data-stu-id="db829-142">contactId</span></span>|<span data-ttu-id="db829-143">字符串, 最大大小为250</span><span class="sxs-lookup"><span data-stu-id="db829-143">string, maximum size 250</span></span>|<span data-ttu-id="db829-144">给定客户的 exchange 联系人 id。</span><span class="sxs-lookup"><span data-stu-id="db829-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="db829-145">如果未指定客户 id, 我们将使用联系人 id 来查找它。</span><span class="sxs-lookup"><span data-stu-id="db829-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="db829-146">postingDate</span><span class="sxs-lookup"><span data-stu-id="db829-146">postingDate</span></span>|<span data-ttu-id="db829-147">date</span><span class="sxs-lookup"><span data-stu-id="db829-147">date</span></span>|<span data-ttu-id="db829-148">客户付款的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="db829-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="db829-149">documentNumber</span><span class="sxs-lookup"><span data-stu-id="db829-149">documentNumber</span></span>|<span data-ttu-id="db829-150">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="db829-150">string, maximum size 20</span></span>|<span data-ttu-id="db829-151">指定客户付款的文档编号。</span><span class="sxs-lookup"><span data-stu-id="db829-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="db829-152">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="db829-152">externalDocumentNumber</span></span>|<span data-ttu-id="db829-153">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="db829-153">string, maximum size 20</span></span>|<span data-ttu-id="db829-154">指定客户付款的外部文档编号。</span><span class="sxs-lookup"><span data-stu-id="db829-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="db829-155">量</span><span class="sxs-lookup"><span data-stu-id="db829-155">amount</span></span>|<span data-ttu-id="db829-156">数位</span><span class="sxs-lookup"><span data-stu-id="db829-156">decimal</span></span>|<span data-ttu-id="db829-157">指定客户付款包含的总金额 (包括 VAT)。</span><span class="sxs-lookup"><span data-stu-id="db829-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="db829-158">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="db829-158">appliesToInvoiceId</span></span>|<span data-ttu-id="db829-159">GUID</span><span class="sxs-lookup"><span data-stu-id="db829-159">GUID</span></span>|<span data-ttu-id="db829-160">与付款相关的发票的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="db829-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="db829-161">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="db829-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="db829-162">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="db829-162">string, maximum size 20</span></span>|<span data-ttu-id="db829-163">与付款相关的发票的编号。</span><span class="sxs-lookup"><span data-stu-id="db829-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="db829-164">说明</span><span class="sxs-lookup"><span data-stu-id="db829-164">description</span></span>|<span data-ttu-id="db829-165">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="db829-165">string, maximum size 50</span></span>|<span data-ttu-id="db829-166">客户付款的说明, 由用户或 autocreated 提供。</span><span class="sxs-lookup"><span data-stu-id="db829-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="db829-167">注释</span><span class="sxs-lookup"><span data-stu-id="db829-167">comment</span></span>|<span data-ttu-id="db829-168">字符串, 最大大小为250</span><span class="sxs-lookup"><span data-stu-id="db829-168">string, maximum size 250</span></span>|<span data-ttu-id="db829-169">用户在客户付款上指定的注释。</span><span class="sxs-lookup"><span data-stu-id="db829-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="db829-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db829-170">lastModifiedDateTime</span></span>|<span data-ttu-id="db829-171">datetime</span><span class="sxs-lookup"><span data-stu-id="db829-171">datetime</span></span>|<span data-ttu-id="db829-172">客户付款修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="db829-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="db829-173">只读。</span><span class="sxs-lookup"><span data-stu-id="db829-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="db829-174">关系</span><span class="sxs-lookup"><span data-stu-id="db829-174">Relationships</span></span>
<span data-ttu-id="db829-175">客户付款是客户付款日志的子页面。</span><span class="sxs-lookup"><span data-stu-id="db829-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="db829-176">不能直接访问它。</span><span class="sxs-lookup"><span data-stu-id="db829-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="db829-177">客户付款可以是维行的 "父实体"。</span><span class="sxs-lookup"><span data-stu-id="db829-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="db829-178">客户 (customerId) 必须存在于 Customers 表中。</span><span class="sxs-lookup"><span data-stu-id="db829-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="db829-179">发票 (appliesToInvoiceId) 必须存在于 "销售发票" 表中。</span><span class="sxs-lookup"><span data-stu-id="db829-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="db829-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db829-180">JSON representation</span></span>

<span data-ttu-id="db829-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db829-181">Here is a JSON representation of the resource.</span></span>

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

