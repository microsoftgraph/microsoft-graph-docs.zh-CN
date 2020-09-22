---
title: secureScore 资源类型
description: 表示租户和控制级别上的每日记分数据的租户安全分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e4f798ae64b881c95ed4330901c0a34ba4073f0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984094"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="8d3d4-103">secureScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d3d4-103">secureScore resource type</span></span>

<span data-ttu-id="8d3d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d3d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d3d4-105">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="8d3d4-106">默认情况下，将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="8d3d4-107">此数据按 **createdDateTime**进行排序，从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="8d3d4-108">这将允许您使用 $top = n 对响应进行分页，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="8d3d4-109">方法</span><span class="sxs-lookup"><span data-stu-id="8d3d4-109">Methods</span></span>

| <span data-ttu-id="8d3d4-110">方法</span><span class="sxs-lookup"><span data-stu-id="8d3d4-110">Method</span></span>   | <span data-ttu-id="8d3d4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d3d4-111">Return Type</span></span>|<span data-ttu-id="8d3d4-112">说明</span><span class="sxs-lookup"><span data-stu-id="8d3d4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d3d4-113">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="8d3d4-113">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="8d3d4-114">[secureScores](securescore.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d3d4-114">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="8d3d4-115">获取 secureScore 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-115">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="8d3d4-116">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="8d3d4-116">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="8d3d4-117">secureScore</span><span class="sxs-lookup"><span data-stu-id="8d3d4-117">secureScore</span></span>](securescore.md) |<span data-ttu-id="8d3d4-118">读取 secureScore 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-118">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="8d3d4-119">属性</span><span class="sxs-lookup"><span data-stu-id="8d3d4-119">Properties</span></span>

|<span data-ttu-id="8d3d4-120">属性</span><span class="sxs-lookup"><span data-stu-id="8d3d4-120">Property</span></span> |<span data-ttu-id="8d3d4-121">类型</span><span class="sxs-lookup"><span data-stu-id="8d3d4-121">Type</span></span> |<span data-ttu-id="8d3d4-122">说明</span><span class="sxs-lookup"><span data-stu-id="8d3d4-122">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="8d3d4-123">id</span><span class="sxs-lookup"><span data-stu-id="8d3d4-123">id</span></span> |<span data-ttu-id="8d3d4-124">String</span><span class="sxs-lookup"><span data-stu-id="8d3d4-124">String</span></span>|<span data-ttu-id="8d3d4-125">提供程序生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-125">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="8d3d4-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-126">Read-only.</span></span> <span data-ttu-id="8d3d4-127">必需。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-127">Required.</span></span>|
|   <span data-ttu-id="8d3d4-128">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="8d3d4-128">azureTenantId</span></span>   |   <span data-ttu-id="8d3d4-129">字符串</span><span class="sxs-lookup"><span data-stu-id="8d3d4-129">String</span></span>  |   <span data-ttu-id="8d3d4-130">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-130">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="8d3d4-131">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="8d3d4-131">activeUserCount</span></span> |   <span data-ttu-id="8d3d4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3d4-132">Int32</span></span>   |   <span data-ttu-id="8d3d4-133">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-133">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="8d3d4-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d3d4-134">createdDateTime</span></span> |   <span data-ttu-id="8d3d4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d3d4-135">DateTimeOffset</span></span>  |   <span data-ttu-id="8d3d4-136">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-136">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="8d3d4-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="8d3d4-137">currentScore</span></span>    |   <span data-ttu-id="8d3d4-138">双精度</span><span class="sxs-lookup"><span data-stu-id="8d3d4-138">Double</span></span>  |   <span data-ttu-id="8d3d4-139">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="8d3d4-140">enabledServices</span><span class="sxs-lookup"><span data-stu-id="8d3d4-140">enabledServices</span></span> |   <span data-ttu-id="8d3d4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8d3d4-141">String collection</span></span>   |   <span data-ttu-id="8d3d4-142">Microsoft 为租户提供的服务 (例如，Exchange online、Skype、Sharepoint) 。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-142">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="8d3d4-143">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="8d3d4-143">licensedUserCount</span></span>   |   <span data-ttu-id="8d3d4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3d4-144">Int32</span></span>   |   <span data-ttu-id="8d3d4-145">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-145">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="8d3d4-146">maxScore</span><span class="sxs-lookup"><span data-stu-id="8d3d4-146">maxScore</span></span> |  <span data-ttu-id="8d3d4-147">双精度</span><span class="sxs-lookup"><span data-stu-id="8d3d4-147">Double</span></span>  |   <span data-ttu-id="8d3d4-148">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-148">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="8d3d4-149">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="8d3d4-149">averageComparativeScores</span></span> |  <span data-ttu-id="8d3d4-150">[averageComparativeScore](averagecomparativescore.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d3d4-150">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="8d3d4-151">不同作用域的平均分数 (例如，行业平均值、座位) 和控制类别的平均 (标识、数据、设备、应用程序、基础结构) 在范围内。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-151">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="8d3d4-152">controlScores</span><span class="sxs-lookup"><span data-stu-id="8d3d4-152">controlScores</span></span> | <span data-ttu-id="8d3d4-153">[controlScore](controlscore.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d3d4-153">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="8d3d4-154">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-154">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="8d3d4-155">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="8d3d4-155">vendorInformation</span></span> |[<span data-ttu-id="8d3d4-156">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="8d3d4-156">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="8d3d4-157">包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft;provider = SecureScore) 。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-157">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="8d3d4-158">必需。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-158">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8d3d4-159">关系</span><span class="sxs-lookup"><span data-stu-id="8d3d4-159">Relationships</span></span>

<span data-ttu-id="8d3d4-160">无。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d3d4-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d3d4-161">JSON representation</span></span>

<span data-ttu-id="8d3d4-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d3d4-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

