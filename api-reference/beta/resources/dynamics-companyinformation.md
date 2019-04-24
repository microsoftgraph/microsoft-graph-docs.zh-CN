---
title: companyInformation 资源类型
description: Dynamics 365 Business Central 中的公司信息。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507271"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="c00c4-103">companyInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c00c4-103">companyInformation resource type</span></span>
<span data-ttu-id="c00c4-104">表示为 Dynamics 365 Business Central 中的当前公司指定的信息, 例如名称、地址、电子邮件地址和网站地址。</span><span class="sxs-lookup"><span data-stu-id="c00c4-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="c00c4-105">方法</span><span class="sxs-lookup"><span data-stu-id="c00c4-105">Methods</span></span>

| <span data-ttu-id="c00c4-106">方法</span><span class="sxs-lookup"><span data-stu-id="c00c4-106">Method</span></span>         | <span data-ttu-id="c00c4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c00c4-107">Return Type</span></span>  |<span data-ttu-id="c00c4-108">说明</span><span class="sxs-lookup"><span data-stu-id="c00c4-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="c00c4-109">获取 companyInformation</span><span class="sxs-lookup"><span data-stu-id="c00c4-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="c00c4-110">companyInformation</span><span class="sxs-lookup"><span data-stu-id="c00c4-110">companyInformation</span></span>|<span data-ttu-id="c00c4-111">获取公司信息。</span><span class="sxs-lookup"><span data-stu-id="c00c4-111">Gets a company information.</span></span>|
|[<span data-ttu-id="c00c4-112">修补程序 companyInformation</span><span class="sxs-lookup"><span data-stu-id="c00c4-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="c00c4-113">companyInformation</span><span class="sxs-lookup"><span data-stu-id="c00c4-113">companyInformation</span></span>|<span data-ttu-id="c00c4-114">更新公司信息。</span><span class="sxs-lookup"><span data-stu-id="c00c4-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="c00c4-115">属性</span><span class="sxs-lookup"><span data-stu-id="c00c4-115">Properties</span></span>
| <span data-ttu-id="c00c4-116">属性</span><span class="sxs-lookup"><span data-stu-id="c00c4-116">Property</span></span>     | <span data-ttu-id="c00c4-117">类型</span><span class="sxs-lookup"><span data-stu-id="c00c4-117">Type</span></span>      |<span data-ttu-id="c00c4-118">说明</span><span class="sxs-lookup"><span data-stu-id="c00c4-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="c00c4-119">id</span><span class="sxs-lookup"><span data-stu-id="c00c4-119">id</span></span>            |<span data-ttu-id="c00c4-120">GUID</span><span class="sxs-lookup"><span data-stu-id="c00c4-120">GUID</span></span>|<span data-ttu-id="c00c4-121">公司的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c00c4-121">The unique ID of the company.</span></span> <span data-ttu-id="c00c4-122">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="c00c4-122">Non-editable.</span></span>|
|<span data-ttu-id="c00c4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="c00c4-123">displayName</span></span>   |<span data-ttu-id="c00c4-124">string</span><span class="sxs-lookup"><span data-stu-id="c00c4-124">string</span></span>   |<span data-ttu-id="c00c4-125">公司的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c00c4-125">The company's display name.</span></span>           |
|<span data-ttu-id="c00c4-126">address</span><span class="sxs-lookup"><span data-stu-id="c00c4-126">address</span></span>       |[<span data-ttu-id="c00c4-127">翻.省略</span><span class="sxs-lookup"><span data-stu-id="c00c4-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c00c4-128">公司地址。</span><span class="sxs-lookup"><span data-stu-id="c00c4-128">The company's address.</span></span> <span data-ttu-id="c00c4-129">查看复杂类型以获取其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c00c4-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="c00c4-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c00c4-130">phoneNumber</span></span>   |<span data-ttu-id="c00c4-131">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-131">string</span></span>   |<span data-ttu-id="c00c4-132">公司的电话号码。</span><span class="sxs-lookup"><span data-stu-id="c00c4-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="c00c4-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="c00c4-133">faxNumber</span></span>     |<span data-ttu-id="c00c4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-134">string</span></span>   |<span data-ttu-id="c00c4-135">公司的传真号码。</span><span class="sxs-lookup"><span data-stu-id="c00c4-135">The company's fax number.</span></span>             |
|<span data-ttu-id="c00c4-136">email</span><span class="sxs-lookup"><span data-stu-id="c00c4-136">email</span></span>         |<span data-ttu-id="c00c4-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-137">string</span></span>   |<span data-ttu-id="c00c4-138">公司的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c00c4-138">The company's email address.</span></span>          |
|<span data-ttu-id="c00c4-139">website</span><span class="sxs-lookup"><span data-stu-id="c00c4-139">website</span></span>       |<span data-ttu-id="c00c4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-140">string</span></span>   |<span data-ttu-id="c00c4-141">公司的网站地址。</span><span class="sxs-lookup"><span data-stu-id="c00c4-141">The company's website address.</span></span>        |
|<span data-ttu-id="c00c4-142">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="c00c4-142">taxRegistrationNumber</span></span>|<span data-ttu-id="c00c4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-143">string</span></span>|<span data-ttu-id="c00c4-144">公司的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="c00c4-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="c00c4-145">currencyCode</span><span class="sxs-lookup"><span data-stu-id="c00c4-145">currencyCode</span></span>  |<span data-ttu-id="c00c4-146">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-146">string</span></span>   |<span data-ttu-id="c00c4-147">公司参与业务的货币。</span><span class="sxs-lookup"><span data-stu-id="c00c4-147">The currency the company does business in.</span></span> <span data-ttu-id="c00c4-148">只读。</span><span class="sxs-lookup"><span data-stu-id="c00c4-148">Read-Only.</span></span>|
|<span data-ttu-id="c00c4-149">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="c00c4-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="c00c4-150">date</span><span class="sxs-lookup"><span data-stu-id="c00c4-150">date</span></span>|<span data-ttu-id="c00c4-151">公司的当前会计年度开始日期。</span><span class="sxs-lookup"><span data-stu-id="c00c4-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="c00c4-152">只读。</span><span class="sxs-lookup"><span data-stu-id="c00c4-152">Read-Only.</span></span>|
|<span data-ttu-id="c00c4-153">领域</span><span class="sxs-lookup"><span data-stu-id="c00c4-153">industry</span></span>      |<span data-ttu-id="c00c4-154">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-154">string</span></span>   |<span data-ttu-id="c00c4-155">公司所属的行业。</span><span class="sxs-lookup"><span data-stu-id="c00c4-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="c00c4-156">头像</span><span class="sxs-lookup"><span data-stu-id="c00c4-156">picture</span></span>       |<span data-ttu-id="c00c4-157">stream</span><span class="sxs-lookup"><span data-stu-id="c00c4-157">stream</span></span>   |<span data-ttu-id="c00c4-158">公司徽标。</span><span class="sxs-lookup"><span data-stu-id="c00c4-158">The company logo.</span></span> <span data-ttu-id="c00c4-159">只读。</span><span class="sxs-lookup"><span data-stu-id="c00c4-159">Read-Only.</span></span>          |
|<span data-ttu-id="c00c4-160">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="c00c4-160">businessProfileId</span></span>|<span data-ttu-id="c00c4-161">字符串</span><span class="sxs-lookup"><span data-stu-id="c00c4-161">string</span></span>|<span data-ttu-id="c00c4-162">链接到财务公司的业务配置文件 ID。</span><span class="sxs-lookup"><span data-stu-id="c00c4-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="c00c4-163">只读。</span><span class="sxs-lookup"><span data-stu-id="c00c4-163">Read-Only.</span></span>|
|<span data-ttu-id="c00c4-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c00c4-164">lastModifiedDateTime</span></span>|<span data-ttu-id="c00c4-165">datetime</span><span class="sxs-lookup"><span data-stu-id="c00c4-165">datetime</span></span>|<span data-ttu-id="c00c4-166">上次修改公司的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c00c4-166">The last datetime the company was modified.</span></span> <span data-ttu-id="c00c4-167">只读。</span><span class="sxs-lookup"><span data-stu-id="c00c4-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c00c4-168">关系</span><span class="sxs-lookup"><span data-stu-id="c00c4-168">Relationships</span></span>
<span data-ttu-id="c00c4-169">无</span><span class="sxs-lookup"><span data-stu-id="c00c4-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c00c4-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c00c4-170">JSON representation</span></span>

<span data-ttu-id="c00c4-171">下面是 companyInformation 的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c00c4-171">Here is a JSON representation of the companyInformation</span></span>
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

