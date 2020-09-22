---
title: companyInformation 资源类型
description: Dynamics 365 Business Central 中的公司信息。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 05a42bfb00cb56cd560151976bc8b7c7d6ed59ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081765"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="0daaf-103">companyInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0daaf-103">companyInformation resource type</span></span>

<span data-ttu-id="0daaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0daaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0daaf-105">表示为 Dynamics 365 Business Central 中的当前公司指定的信息，例如名称、地址、电子邮件地址和网站地址。</span><span class="sxs-lookup"><span data-stu-id="0daaf-105">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="0daaf-106">方法</span><span class="sxs-lookup"><span data-stu-id="0daaf-106">Methods</span></span>

| <span data-ttu-id="0daaf-107">方法</span><span class="sxs-lookup"><span data-stu-id="0daaf-107">Method</span></span>         | <span data-ttu-id="0daaf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0daaf-108">Return Type</span></span>  |<span data-ttu-id="0daaf-109">说明</span><span class="sxs-lookup"><span data-stu-id="0daaf-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="0daaf-110">获取 companyInformation</span><span class="sxs-lookup"><span data-stu-id="0daaf-110">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="0daaf-111">companyInformation</span><span class="sxs-lookup"><span data-stu-id="0daaf-111">companyInformation</span></span>|<span data-ttu-id="0daaf-112">获取公司信息。</span><span class="sxs-lookup"><span data-stu-id="0daaf-112">Gets a company information.</span></span>|
|[<span data-ttu-id="0daaf-113">修补程序 companyInformation</span><span class="sxs-lookup"><span data-stu-id="0daaf-113">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="0daaf-114">companyInformation</span><span class="sxs-lookup"><span data-stu-id="0daaf-114">companyInformation</span></span>|<span data-ttu-id="0daaf-115">更新公司信息。</span><span class="sxs-lookup"><span data-stu-id="0daaf-115">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="0daaf-116">属性</span><span class="sxs-lookup"><span data-stu-id="0daaf-116">Properties</span></span>
| <span data-ttu-id="0daaf-117">属性</span><span class="sxs-lookup"><span data-stu-id="0daaf-117">Property</span></span>     | <span data-ttu-id="0daaf-118">类型</span><span class="sxs-lookup"><span data-stu-id="0daaf-118">Type</span></span>      |<span data-ttu-id="0daaf-119">说明</span><span class="sxs-lookup"><span data-stu-id="0daaf-119">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="0daaf-120">id</span><span class="sxs-lookup"><span data-stu-id="0daaf-120">id</span></span>            |<span data-ttu-id="0daaf-121">GUID</span><span class="sxs-lookup"><span data-stu-id="0daaf-121">GUID</span></span>|<span data-ttu-id="0daaf-122">公司的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0daaf-122">The unique ID of the company.</span></span> <span data-ttu-id="0daaf-123">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="0daaf-123">Non-editable.</span></span>|
|<span data-ttu-id="0daaf-124">displayName</span><span class="sxs-lookup"><span data-stu-id="0daaf-124">displayName</span></span>   |<span data-ttu-id="0daaf-125">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-125">string</span></span>   |<span data-ttu-id="0daaf-126">公司的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0daaf-126">The company's display name.</span></span>           |
|<span data-ttu-id="0daaf-127">address</span><span class="sxs-lookup"><span data-stu-id="0daaf-127">address</span></span>       |[<span data-ttu-id="0daaf-128">翻.省略</span><span class="sxs-lookup"><span data-stu-id="0daaf-128">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="0daaf-129">公司地址。</span><span class="sxs-lookup"><span data-stu-id="0daaf-129">The company's address.</span></span> <span data-ttu-id="0daaf-130">查看复杂类型以获取其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="0daaf-130">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="0daaf-131">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="0daaf-131">phoneNumber</span></span>   |<span data-ttu-id="0daaf-132">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-132">string</span></span>   |<span data-ttu-id="0daaf-133">公司的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0daaf-133">The company's telephone number.</span></span>       |
|<span data-ttu-id="0daaf-134">faxNumber</span><span class="sxs-lookup"><span data-stu-id="0daaf-134">faxNumber</span></span>     |<span data-ttu-id="0daaf-135">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-135">string</span></span>   |<span data-ttu-id="0daaf-136">公司的传真号码。</span><span class="sxs-lookup"><span data-stu-id="0daaf-136">The company's fax number.</span></span>             |
|<span data-ttu-id="0daaf-137">email</span><span class="sxs-lookup"><span data-stu-id="0daaf-137">email</span></span>         |<span data-ttu-id="0daaf-138">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-138">string</span></span>   |<span data-ttu-id="0daaf-139">公司的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0daaf-139">The company's email address.</span></span>          |
|<span data-ttu-id="0daaf-140">website</span><span class="sxs-lookup"><span data-stu-id="0daaf-140">website</span></span>       |<span data-ttu-id="0daaf-141">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-141">string</span></span>   |<span data-ttu-id="0daaf-142">公司的网站地址。</span><span class="sxs-lookup"><span data-stu-id="0daaf-142">The company's website address.</span></span>        |
|<span data-ttu-id="0daaf-143">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="0daaf-143">taxRegistrationNumber</span></span>|<span data-ttu-id="0daaf-144">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-144">string</span></span>|<span data-ttu-id="0daaf-145">公司的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="0daaf-145">The company's tax registration number.</span></span>|
|<span data-ttu-id="0daaf-146">currencyCode</span><span class="sxs-lookup"><span data-stu-id="0daaf-146">currencyCode</span></span>  |<span data-ttu-id="0daaf-147">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-147">string</span></span>   |<span data-ttu-id="0daaf-148">公司参与业务的货币。</span><span class="sxs-lookup"><span data-stu-id="0daaf-148">The currency the company does business in.</span></span> <span data-ttu-id="0daaf-149">只读。</span><span class="sxs-lookup"><span data-stu-id="0daaf-149">Read-Only.</span></span>|
|<span data-ttu-id="0daaf-150">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="0daaf-150">currentFiscalYearStartDate</span></span>|<span data-ttu-id="0daaf-151">date</span><span class="sxs-lookup"><span data-stu-id="0daaf-151">date</span></span>|<span data-ttu-id="0daaf-152">公司的当前会计年度开始日期。</span><span class="sxs-lookup"><span data-stu-id="0daaf-152">The company's current fiscal year start date.</span></span> <span data-ttu-id="0daaf-153">只读。</span><span class="sxs-lookup"><span data-stu-id="0daaf-153">Read-Only.</span></span>|
|<span data-ttu-id="0daaf-154">领域</span><span class="sxs-lookup"><span data-stu-id="0daaf-154">industry</span></span>      |<span data-ttu-id="0daaf-155">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-155">string</span></span>   |<span data-ttu-id="0daaf-156">公司所属的行业。</span><span class="sxs-lookup"><span data-stu-id="0daaf-156">The industry the company is part of.</span></span>  |
|<span data-ttu-id="0daaf-157">头像</span><span class="sxs-lookup"><span data-stu-id="0daaf-157">picture</span></span>       |<span data-ttu-id="0daaf-158">stream</span><span class="sxs-lookup"><span data-stu-id="0daaf-158">stream</span></span>   |<span data-ttu-id="0daaf-159">公司徽标。</span><span class="sxs-lookup"><span data-stu-id="0daaf-159">The company logo.</span></span> <span data-ttu-id="0daaf-160">只读。</span><span class="sxs-lookup"><span data-stu-id="0daaf-160">Read-Only.</span></span>          |
|<span data-ttu-id="0daaf-161">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="0daaf-161">businessProfileId</span></span>|<span data-ttu-id="0daaf-162">string</span><span class="sxs-lookup"><span data-stu-id="0daaf-162">string</span></span>|<span data-ttu-id="0daaf-163">链接到财务公司的业务配置文件 ID。</span><span class="sxs-lookup"><span data-stu-id="0daaf-163">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="0daaf-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0daaf-164">Read-Only.</span></span>|
|<span data-ttu-id="0daaf-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0daaf-165">lastModifiedDateTime</span></span>|<span data-ttu-id="0daaf-166">datetime</span><span class="sxs-lookup"><span data-stu-id="0daaf-166">datetime</span></span>|<span data-ttu-id="0daaf-167">上次修改公司的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0daaf-167">The last datetime the company was modified.</span></span> <span data-ttu-id="0daaf-168">只读。</span><span class="sxs-lookup"><span data-stu-id="0daaf-168">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="0daaf-169">关系</span><span class="sxs-lookup"><span data-stu-id="0daaf-169">Relationships</span></span>
<span data-ttu-id="0daaf-170">无</span><span class="sxs-lookup"><span data-stu-id="0daaf-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0daaf-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0daaf-171">JSON representation</span></span>

<span data-ttu-id="0daaf-172">下面是 companyInformation 的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0daaf-172">Here is a JSON representation of the companyInformation</span></span>
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```



