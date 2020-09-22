---
title: 供应商资源类型
description: Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a2102a77748ebef8267792a887a522fa716619ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040038"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="d8d10-103">供应商资源类型</span><span class="sxs-lookup"><span data-stu-id="d8d10-103">vendors resource type</span></span>

<span data-ttu-id="d8d10-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d10-105">表示 Dynamics 365 Business Central 中的供应商。</span><span class="sxs-lookup"><span data-stu-id="d8d10-105">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d8d10-106">方法</span><span class="sxs-lookup"><span data-stu-id="d8d10-106">Methods</span></span>

| <span data-ttu-id="d8d10-107">方法</span><span class="sxs-lookup"><span data-stu-id="d8d10-107">Method</span></span>       | <span data-ttu-id="d8d10-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8d10-108">Return Type</span></span>  |<span data-ttu-id="d8d10-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8d10-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8d10-110">获取供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-110">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="d8d10-111">供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-111">vendors</span></span>|<span data-ttu-id="d8d10-112">获取一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="d8d10-112">Gets a vendor object.</span></span>|
|[<span data-ttu-id="d8d10-113">供应商后</span><span class="sxs-lookup"><span data-stu-id="d8d10-113">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="d8d10-114">供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-114">vendors</span></span>|<span data-ttu-id="d8d10-115">创建一个供应商对象。</span><span class="sxs-lookup"><span data-stu-id="d8d10-115">Creates a vendor object.</span></span>|
|[<span data-ttu-id="d8d10-116">修补程序供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-116">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="d8d10-117">供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-117">vendors</span></span>|<span data-ttu-id="d8d10-118">更新供应商对象。</span><span class="sxs-lookup"><span data-stu-id="d8d10-118">Updates a vendor object.</span></span>|
|[<span data-ttu-id="d8d10-119">删除供应商</span><span class="sxs-lookup"><span data-stu-id="d8d10-119">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="d8d10-120">无</span><span class="sxs-lookup"><span data-stu-id="d8d10-120">none</span></span>|<span data-ttu-id="d8d10-121">删除 "供应商" 对象。</span><span class="sxs-lookup"><span data-stu-id="d8d10-121">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8d10-122">属性</span><span class="sxs-lookup"><span data-stu-id="d8d10-122">Properties</span></span>
| <span data-ttu-id="d8d10-123">属性</span><span class="sxs-lookup"><span data-stu-id="d8d10-123">Property</span></span>     | <span data-ttu-id="d8d10-124">类型</span><span class="sxs-lookup"><span data-stu-id="d8d10-124">Type</span></span>   |<span data-ttu-id="d8d10-125">说明</span><span class="sxs-lookup"><span data-stu-id="d8d10-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d10-126">id</span><span class="sxs-lookup"><span data-stu-id="d8d10-126">id</span></span>|<span data-ttu-id="d8d10-127">GUID</span><span class="sxs-lookup"><span data-stu-id="d8d10-127">GUID</span></span>|<span data-ttu-id="d8d10-128">供应商的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d8d10-128">The unique ID of the vendor.</span></span> <span data-ttu-id="d8d10-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="d8d10-129">Non-editable.</span></span>|
|<span data-ttu-id="d8d10-130">数字</span><span class="sxs-lookup"><span data-stu-id="d8d10-130">number</span></span>|<span data-ttu-id="d8d10-131">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-131">string</span></span>|<span data-ttu-id="d8d10-132">供应商编号。</span><span class="sxs-lookup"><span data-stu-id="d8d10-132">The vendor number.</span></span>|
|<span data-ttu-id="d8d10-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d8d10-133">displayName</span></span>|<span data-ttu-id="d8d10-134">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-134">string</span></span>|<span data-ttu-id="d8d10-135">供应商的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d8d10-135">The vendor's display name.</span></span>|
|<span data-ttu-id="d8d10-136">address</span><span class="sxs-lookup"><span data-stu-id="d8d10-136">address</span></span>|[<span data-ttu-id="d8d10-137">翻.省略</span><span class="sxs-lookup"><span data-stu-id="d8d10-137">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="d8d10-138">供应商的地址。</span><span class="sxs-lookup"><span data-stu-id="d8d10-138">The vendor's address.</span></span>|
|<span data-ttu-id="d8d10-139">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d8d10-139">phoneNumber</span></span>|<span data-ttu-id="d8d10-140">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-140">string</span></span>|<span data-ttu-id="d8d10-141">供应商的电话号码。</span><span class="sxs-lookup"><span data-stu-id="d8d10-141">The vendor's telephone number.</span></span>|
|<span data-ttu-id="d8d10-142">email</span><span class="sxs-lookup"><span data-stu-id="d8d10-142">email</span></span>|<span data-ttu-id="d8d10-143">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-143">string</span></span>|<span data-ttu-id="d8d10-144">供应商的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d8d10-144">The vendor's email address.</span></span>|
|<span data-ttu-id="d8d10-145">website</span><span class="sxs-lookup"><span data-stu-id="d8d10-145">website</span></span>|<span data-ttu-id="d8d10-146">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-146">string</span></span>|<span data-ttu-id="d8d10-147">供应商的网站地址。</span><span class="sxs-lookup"><span data-stu-id="d8d10-147">The vendor's website address.</span></span>|
|<span data-ttu-id="d8d10-148">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="d8d10-148">taxRegistrationNumber</span></span>|<span data-ttu-id="d8d10-149">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-149">string</span></span>|<span data-ttu-id="d8d10-150">供应商的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="d8d10-150">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="d8d10-151">currencyId</span><span class="sxs-lookup"><span data-stu-id="d8d10-151">currencyId</span></span>|<span data-ttu-id="d8d10-152">GUID</span><span class="sxs-lookup"><span data-stu-id="d8d10-152">GUID</span></span>|<span data-ttu-id="d8d10-153">供应商的默认币种代码 ID。</span><span class="sxs-lookup"><span data-stu-id="d8d10-153">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="d8d10-154">currencyCode</span><span class="sxs-lookup"><span data-stu-id="d8d10-154">currencyCode</span></span>|<span data-ttu-id="d8d10-155">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-155">string</span></span>|<span data-ttu-id="d8d10-156">供应商的默认币种代码。</span><span class="sxs-lookup"><span data-stu-id="d8d10-156">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="d8d10-157">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="d8d10-157">irs1099Code</span></span>|<span data-ttu-id="d8d10-158">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-158">string</span></span>|<span data-ttu-id="d8d10-159">指定供应商的1099代码。</span><span class="sxs-lookup"><span data-stu-id="d8d10-159">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="d8d10-160">仅限美国。</span><span class="sxs-lookup"><span data-stu-id="d8d10-160">US only.</span></span>|
|<span data-ttu-id="d8d10-161">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="d8d10-161">paymentTermsId</span></span>|<span data-ttu-id="d8d10-162">GUID</span><span class="sxs-lookup"><span data-stu-id="d8d10-162">GUID</span></span>|<span data-ttu-id="d8d10-163">供应商的默认付款条款 ID。</span><span class="sxs-lookup"><span data-stu-id="d8d10-163">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="d8d10-164">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="d8d10-164">paymentMethodId</span></span>|<span data-ttu-id="d8d10-165">GUID</span><span class="sxs-lookup"><span data-stu-id="d8d10-165">GUID</span></span>|<span data-ttu-id="d8d10-166">供应商的默认付款方法 ID。</span><span class="sxs-lookup"><span data-stu-id="d8d10-166">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="d8d10-167">taxLiable</span><span class="sxs-lookup"><span data-stu-id="d8d10-167">taxLiable</span></span>|<span data-ttu-id="d8d10-168">boolean</span><span class="sxs-lookup"><span data-stu-id="d8d10-168">boolean</span></span>|<span data-ttu-id="d8d10-169">指定供应商是否对税负有责任。</span><span class="sxs-lookup"><span data-stu-id="d8d10-169">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="d8d10-170">堵塞</span><span class="sxs-lookup"><span data-stu-id="d8d10-170">blocked</span></span>|<span data-ttu-id="d8d10-171">string</span><span class="sxs-lookup"><span data-stu-id="d8d10-171">string</span></span>|<span data-ttu-id="d8d10-172">指定哪些交易记录与供应商不能过帐。</span><span class="sxs-lookup"><span data-stu-id="d8d10-172">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="d8d10-173">接受的值为空、付款或全部</span><span class="sxs-lookup"><span data-stu-id="d8d10-173">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="d8d10-174">恰好</span><span class="sxs-lookup"><span data-stu-id="d8d10-174">balance</span></span>|<span data-ttu-id="d8d10-175">数位</span><span class="sxs-lookup"><span data-stu-id="d8d10-175">decimal</span></span>|<span data-ttu-id="d8d10-176">供应商的余额。</span><span class="sxs-lookup"><span data-stu-id="d8d10-176">The vendor's balance.</span></span> <span data-ttu-id="d8d10-177">只读。</span><span class="sxs-lookup"><span data-stu-id="d8d10-177">Read-Only.</span></span>|
|<span data-ttu-id="d8d10-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d10-178">lastModifiedDateTime</span></span>|<span data-ttu-id="d8d10-179">datetime</span><span class="sxs-lookup"><span data-stu-id="d8d10-179">datetime</span></span>|<span data-ttu-id="d8d10-180">上次修改供应商的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d8d10-180">The last datetime the vendor was modified.</span></span> <span data-ttu-id="d8d10-181">只读。</span><span class="sxs-lookup"><span data-stu-id="d8d10-181">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="d8d10-182">关系</span><span class="sxs-lookup"><span data-stu-id="d8d10-182">Relationships</span></span>
<span data-ttu-id="d8d10-183">无</span><span class="sxs-lookup"><span data-stu-id="d8d10-183">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8d10-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8d10-184">JSON representation</span></span>

<span data-ttu-id="d8d10-185">下面是供应商的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8d10-185">Here is a JSON representation of the vendor.</span></span>

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



