---
title: companyInformation 资源类型
description: Dynamics 365 Business Central 中的公司信息。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2e23660775ba96b3f898840b0bad2b53eff9584a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012665"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="a7b06-103">companyInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7b06-103">companyInformation resource type</span></span>
<span data-ttu-id="a7b06-104">表示为 Dynamics 365 Business Central 中的当前公司指定的信息, 例如名称、地址、电子邮件地址和网站地址。</span><span class="sxs-lookup"><span data-stu-id="a7b06-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="a7b06-105">方法</span><span class="sxs-lookup"><span data-stu-id="a7b06-105">Methods</span></span>

| <span data-ttu-id="a7b06-106">方法</span><span class="sxs-lookup"><span data-stu-id="a7b06-106">Method</span></span>         | <span data-ttu-id="a7b06-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7b06-107">Return Type</span></span>  |<span data-ttu-id="a7b06-108">说明</span><span class="sxs-lookup"><span data-stu-id="a7b06-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="a7b06-109">获取 companyInformation</span><span class="sxs-lookup"><span data-stu-id="a7b06-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="a7b06-110">companyInformation</span><span class="sxs-lookup"><span data-stu-id="a7b06-110">companyInformation</span></span>|<span data-ttu-id="a7b06-111">获取公司信息。</span><span class="sxs-lookup"><span data-stu-id="a7b06-111">Gets a company information.</span></span>|
|[<span data-ttu-id="a7b06-112">修补程序 companyInformation</span><span class="sxs-lookup"><span data-stu-id="a7b06-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="a7b06-113">companyInformation</span><span class="sxs-lookup"><span data-stu-id="a7b06-113">companyInformation</span></span>|<span data-ttu-id="a7b06-114">更新公司信息。</span><span class="sxs-lookup"><span data-stu-id="a7b06-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="a7b06-115">属性</span><span class="sxs-lookup"><span data-stu-id="a7b06-115">Properties</span></span>
| <span data-ttu-id="a7b06-116">属性</span><span class="sxs-lookup"><span data-stu-id="a7b06-116">Property</span></span>     | <span data-ttu-id="a7b06-117">类型</span><span class="sxs-lookup"><span data-stu-id="a7b06-117">Type</span></span>      |<span data-ttu-id="a7b06-118">说明</span><span class="sxs-lookup"><span data-stu-id="a7b06-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="a7b06-119">id</span><span class="sxs-lookup"><span data-stu-id="a7b06-119">id</span></span>            |<span data-ttu-id="a7b06-120">GUID</span><span class="sxs-lookup"><span data-stu-id="a7b06-120">GUID</span></span>|<span data-ttu-id="a7b06-121">公司的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a7b06-121">The unique ID of the company.</span></span> <span data-ttu-id="a7b06-122">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="a7b06-122">Non-editable.</span></span>|
|<span data-ttu-id="a7b06-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a7b06-123">displayName</span></span>   |<span data-ttu-id="a7b06-124">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-124">string</span></span>   |<span data-ttu-id="a7b06-125">公司的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a7b06-125">The company's display name.</span></span>           |
|<span data-ttu-id="a7b06-126">address</span><span class="sxs-lookup"><span data-stu-id="a7b06-126">address</span></span>       |[<span data-ttu-id="a7b06-127">翻.省略</span><span class="sxs-lookup"><span data-stu-id="a7b06-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="a7b06-128">公司地址。</span><span class="sxs-lookup"><span data-stu-id="a7b06-128">The company's address.</span></span> <span data-ttu-id="a7b06-129">查看复杂类型以获取其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a7b06-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="a7b06-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a7b06-130">phoneNumber</span></span>   |<span data-ttu-id="a7b06-131">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-131">string</span></span>   |<span data-ttu-id="a7b06-132">公司的电话号码。</span><span class="sxs-lookup"><span data-stu-id="a7b06-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="a7b06-133">faxNumber</span><span class="sxs-lookup"><span data-stu-id="a7b06-133">faxNumber</span></span>     |<span data-ttu-id="a7b06-134">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-134">string</span></span>   |<span data-ttu-id="a7b06-135">公司的传真号码。</span><span class="sxs-lookup"><span data-stu-id="a7b06-135">The company's fax number.</span></span>             |
|<span data-ttu-id="a7b06-136">email</span><span class="sxs-lookup"><span data-stu-id="a7b06-136">email</span></span>         |<span data-ttu-id="a7b06-137">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-137">string</span></span>   |<span data-ttu-id="a7b06-138">公司的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a7b06-138">The company's email address.</span></span>          |
|<span data-ttu-id="a7b06-139">website</span><span class="sxs-lookup"><span data-stu-id="a7b06-139">website</span></span>       |<span data-ttu-id="a7b06-140">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-140">string</span></span>   |<span data-ttu-id="a7b06-141">公司的网站地址。</span><span class="sxs-lookup"><span data-stu-id="a7b06-141">The company's website address.</span></span>        |
|<span data-ttu-id="a7b06-142">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="a7b06-142">taxRegistrationNumber</span></span>|<span data-ttu-id="a7b06-143">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-143">string</span></span>|<span data-ttu-id="a7b06-144">公司的税务登记编号。</span><span class="sxs-lookup"><span data-stu-id="a7b06-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="a7b06-145">currencyCode</span><span class="sxs-lookup"><span data-stu-id="a7b06-145">currencyCode</span></span>  |<span data-ttu-id="a7b06-146">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-146">string</span></span>   |<span data-ttu-id="a7b06-147">公司参与业务的货币。</span><span class="sxs-lookup"><span data-stu-id="a7b06-147">The currency the company does business in.</span></span> <span data-ttu-id="a7b06-148">只读。</span><span class="sxs-lookup"><span data-stu-id="a7b06-148">Read-Only.</span></span>|
|<span data-ttu-id="a7b06-149">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="a7b06-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="a7b06-150">date</span><span class="sxs-lookup"><span data-stu-id="a7b06-150">date</span></span>|<span data-ttu-id="a7b06-151">公司的当前会计年度开始日期。</span><span class="sxs-lookup"><span data-stu-id="a7b06-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="a7b06-152">只读。</span><span class="sxs-lookup"><span data-stu-id="a7b06-152">Read-Only.</span></span>|
|<span data-ttu-id="a7b06-153">领域</span><span class="sxs-lookup"><span data-stu-id="a7b06-153">industry</span></span>      |<span data-ttu-id="a7b06-154">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-154">string</span></span>   |<span data-ttu-id="a7b06-155">公司所属的行业。</span><span class="sxs-lookup"><span data-stu-id="a7b06-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="a7b06-156">头像</span><span class="sxs-lookup"><span data-stu-id="a7b06-156">picture</span></span>       |<span data-ttu-id="a7b06-157">stream</span><span class="sxs-lookup"><span data-stu-id="a7b06-157">stream</span></span>   |<span data-ttu-id="a7b06-158">公司徽标。</span><span class="sxs-lookup"><span data-stu-id="a7b06-158">The company logo.</span></span> <span data-ttu-id="a7b06-159">只读。</span><span class="sxs-lookup"><span data-stu-id="a7b06-159">Read-Only.</span></span>          |
|<span data-ttu-id="a7b06-160">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="a7b06-160">businessProfileId</span></span>|<span data-ttu-id="a7b06-161">string</span><span class="sxs-lookup"><span data-stu-id="a7b06-161">string</span></span>|<span data-ttu-id="a7b06-162">链接到财务公司的业务配置文件 ID。</span><span class="sxs-lookup"><span data-stu-id="a7b06-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="a7b06-163">只读。</span><span class="sxs-lookup"><span data-stu-id="a7b06-163">Read-Only.</span></span>|
|<span data-ttu-id="a7b06-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b06-164">lastModifiedDateTime</span></span>|<span data-ttu-id="a7b06-165">datetime</span><span class="sxs-lookup"><span data-stu-id="a7b06-165">datetime</span></span>|<span data-ttu-id="a7b06-166">上次修改公司的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7b06-166">The last datetime the company was modified.</span></span> <span data-ttu-id="a7b06-167">只读。</span><span class="sxs-lookup"><span data-stu-id="a7b06-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="a7b06-168">关系</span><span class="sxs-lookup"><span data-stu-id="a7b06-168">Relationships</span></span>
<span data-ttu-id="a7b06-169">无</span><span class="sxs-lookup"><span data-stu-id="a7b06-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7b06-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7b06-170">JSON representation</span></span>

<span data-ttu-id="a7b06-171">下面是 companyInformation 的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7b06-171">Here is a JSON representation of the companyInformation</span></span>
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

