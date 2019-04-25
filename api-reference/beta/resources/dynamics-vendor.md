---
title: 供应商资源类型
description: Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534855"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="c0306-103">供应商资源类型</span><span class="sxs-lookup"><span data-stu-id="c0306-103">vendors resource type</span></span>
<span data-ttu-id="c0306-104">表示 Dynamics 365 Business Central 中的供应商。</span><span class="sxs-lookup"><span data-stu-id="c0306-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c0306-105">方法</span><span class="sxs-lookup"><span data-stu-id="c0306-105">Methods</span></span>

| <span data-ttu-id="c0306-106">方法</span><span class="sxs-lookup"><span data-stu-id="c0306-106">Method</span></span>       | <span data-ttu-id="c0306-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0306-107">Return Type</span></span>  |<span data-ttu-id="c0306-108">说明</span><span class="sxs-lookup"><span data-stu-id="c0306-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0306-109">获取供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="c0306-110">供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-110">vendors</span></span>|<span data-ttu-id="c0306-111">获取一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="c0306-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="c0306-112">供应商后</span><span class="sxs-lookup"><span data-stu-id="c0306-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="c0306-113">供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-113">vendors</span></span>|<span data-ttu-id="c0306-114">创建一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="c0306-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="c0306-115">修补程序供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="c0306-116">供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-116">vendors</span></span>|<span data-ttu-id="c0306-117">更新供应商对象。</span><span class="sxs-lookup"><span data-stu-id="c0306-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="c0306-118">删除供应商</span><span class="sxs-lookup"><span data-stu-id="c0306-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="c0306-119">无</span><span class="sxs-lookup"><span data-stu-id="c0306-119">none</span></span>|<span data-ttu-id="c0306-120">删除 "供应商" 对象。</span><span class="sxs-lookup"><span data-stu-id="c0306-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0306-121">属性</span><span class="sxs-lookup"><span data-stu-id="c0306-121">Properties</span></span>
| <span data-ttu-id="c0306-122">属性</span><span class="sxs-lookup"><span data-stu-id="c0306-122">Property</span></span>     | <span data-ttu-id="c0306-123">类型</span><span class="sxs-lookup"><span data-stu-id="c0306-123">Type</span></span>   |<span data-ttu-id="c0306-124">说明</span><span class="sxs-lookup"><span data-stu-id="c0306-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0306-125">id</span><span class="sxs-lookup"><span data-stu-id="c0306-125">id</span></span>|<span data-ttu-id="c0306-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c0306-126">GUID</span></span>|<span data-ttu-id="c0306-127">供应商的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c0306-127">The unique ID of the vendor.</span></span> <span data-ttu-id="c0306-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="c0306-128">Non-editable.</span></span>|
|<span data-ttu-id="c0306-129">数字</span><span class="sxs-lookup"><span data-stu-id="c0306-129">number</span></span>|<span data-ttu-id="c0306-130">string</span><span class="sxs-lookup"><span data-stu-id="c0306-130">string</span></span>|<span data-ttu-id="c0306-131">供应商编号。</span><span class="sxs-lookup"><span data-stu-id="c0306-131">The vendor number.</span></span>|
|<span data-ttu-id="c0306-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c0306-132">displayName</span></span>|<span data-ttu-id="c0306-133">string</span><span class="sxs-lookup"><span data-stu-id="c0306-133">string</span></span>|<span data-ttu-id="c0306-134">供应商的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c0306-134">The vendor's display name.</span></span>|
|<span data-ttu-id="c0306-135">address</span><span class="sxs-lookup"><span data-stu-id="c0306-135">address</span></span>|[<span data-ttu-id="c0306-136">翻.省略</span><span class="sxs-lookup"><span data-stu-id="c0306-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c0306-137">供应商的地址。</span><span class="sxs-lookup"><span data-stu-id="c0306-137">The vendor's address.</span></span>|
|<span data-ttu-id="c0306-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c0306-138">phoneNumber</span></span>|<span data-ttu-id="c0306-139">string</span><span class="sxs-lookup"><span data-stu-id="c0306-139">string</span></span>|<span data-ttu-id="c0306-140">供应商的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c0306-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="c0306-141">email</span><span class="sxs-lookup"><span data-stu-id="c0306-141">email</span></span>|<span data-ttu-id="c0306-142">string</span><span class="sxs-lookup"><span data-stu-id="c0306-142">string</span></span>|<span data-ttu-id="c0306-143">供应商的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c0306-143">The vendor's email address.</span></span>|
|<span data-ttu-id="c0306-144">website</span><span class="sxs-lookup"><span data-stu-id="c0306-144">website</span></span>|<span data-ttu-id="c0306-145">string</span><span class="sxs-lookup"><span data-stu-id="c0306-145">string</span></span>|<span data-ttu-id="c0306-146">供应商的网站地址。</span><span class="sxs-lookup"><span data-stu-id="c0306-146">The vendor's website address.</span></span>|
|<span data-ttu-id="c0306-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="c0306-147">taxRegistrationNumber</span></span>|<span data-ttu-id="c0306-148">string</span><span class="sxs-lookup"><span data-stu-id="c0306-148">string</span></span>|<span data-ttu-id="c0306-149">供应商的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="c0306-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="c0306-150">currencyId</span><span class="sxs-lookup"><span data-stu-id="c0306-150">currencyId</span></span>|<span data-ttu-id="c0306-151">GUID</span><span class="sxs-lookup"><span data-stu-id="c0306-151">GUID</span></span>|<span data-ttu-id="c0306-152">供应商的默认币种代码 ID。</span><span class="sxs-lookup"><span data-stu-id="c0306-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="c0306-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="c0306-153">currencyCode</span></span>|<span data-ttu-id="c0306-154">string</span><span class="sxs-lookup"><span data-stu-id="c0306-154">string</span></span>|<span data-ttu-id="c0306-155">供应商的默认币种代码。</span><span class="sxs-lookup"><span data-stu-id="c0306-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="c0306-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="c0306-156">irs1099Code</span></span>|<span data-ttu-id="c0306-157">string</span><span class="sxs-lookup"><span data-stu-id="c0306-157">string</span></span>|<span data-ttu-id="c0306-158">指定供应商的1099代码。</span><span class="sxs-lookup"><span data-stu-id="c0306-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="c0306-159">仅限美国。</span><span class="sxs-lookup"><span data-stu-id="c0306-159">US only.</span></span>|
|<span data-ttu-id="c0306-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="c0306-160">paymentTermsId</span></span>|<span data-ttu-id="c0306-161">GUID</span><span class="sxs-lookup"><span data-stu-id="c0306-161">GUID</span></span>|<span data-ttu-id="c0306-162">供应商的默认付款条款 ID。</span><span class="sxs-lookup"><span data-stu-id="c0306-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="c0306-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="c0306-163">paymentMethodId</span></span>|<span data-ttu-id="c0306-164">GUID</span><span class="sxs-lookup"><span data-stu-id="c0306-164">GUID</span></span>|<span data-ttu-id="c0306-165">供应商的默认付款方法 ID。</span><span class="sxs-lookup"><span data-stu-id="c0306-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="c0306-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="c0306-166">taxLiable</span></span>|<span data-ttu-id="c0306-167">布尔</span><span class="sxs-lookup"><span data-stu-id="c0306-167">boolean</span></span>|<span data-ttu-id="c0306-168">指定供应商是否对税负有责任。</span><span class="sxs-lookup"><span data-stu-id="c0306-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="c0306-169">堵塞</span><span class="sxs-lookup"><span data-stu-id="c0306-169">blocked</span></span>|<span data-ttu-id="c0306-170">string</span><span class="sxs-lookup"><span data-stu-id="c0306-170">string</span></span>|<span data-ttu-id="c0306-171">指定哪些交易记录与供应商不能过帐。</span><span class="sxs-lookup"><span data-stu-id="c0306-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="c0306-172">接受的值为空、付款或全部</span><span class="sxs-lookup"><span data-stu-id="c0306-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="c0306-173">恰好</span><span class="sxs-lookup"><span data-stu-id="c0306-173">balance</span></span>|<span data-ttu-id="c0306-174">数位</span><span class="sxs-lookup"><span data-stu-id="c0306-174">decimal</span></span>|<span data-ttu-id="c0306-175">供应商的余额。</span><span class="sxs-lookup"><span data-stu-id="c0306-175">The vendor's balance.</span></span> <span data-ttu-id="c0306-176">只读。</span><span class="sxs-lookup"><span data-stu-id="c0306-176">Read-Only.</span></span>|
|<span data-ttu-id="c0306-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0306-177">lastModifiedDateTime</span></span>|<span data-ttu-id="c0306-178">datetime</span><span class="sxs-lookup"><span data-stu-id="c0306-178">datetime</span></span>|<span data-ttu-id="c0306-179">上次修改供应商的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0306-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="c0306-180">只读。</span><span class="sxs-lookup"><span data-stu-id="c0306-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c0306-181">关系</span><span class="sxs-lookup"><span data-stu-id="c0306-181">Relationships</span></span>
<span data-ttu-id="c0306-182">无</span><span class="sxs-lookup"><span data-stu-id="c0306-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0306-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0306-183">JSON representation</span></span>

<span data-ttu-id="c0306-184">下面是供应商的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0306-184">Here is a JSON representation of the vendor.</span></span>

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

