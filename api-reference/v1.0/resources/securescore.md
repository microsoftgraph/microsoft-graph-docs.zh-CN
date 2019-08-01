---
title: secureScore 资源类型
description: 表示租户和控制级别上的每日记分数据的租户安全分数。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395c5ed0594d1f509bb664b5aee6ea18bb42af0a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034480"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="a9f34-103">secureScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9f34-103">secureScore resource type</span></span>

<span data-ttu-id="a9f34-104">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="a9f34-105">默认情况下, 将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="a9f34-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="a9f34-106">此数据按**createdDateTime**进行排序, 从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="a9f34-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="a9f34-107">这将允许您使用 $top = n 对响应进行分页, 其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="a9f34-108">方法</span><span class="sxs-lookup"><span data-stu-id="a9f34-108">Methods</span></span>

| <span data-ttu-id="a9f34-109">方法</span><span class="sxs-lookup"><span data-stu-id="a9f34-109">Method</span></span>   | <span data-ttu-id="a9f34-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a9f34-110">Return Type</span></span>|<span data-ttu-id="a9f34-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9f34-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9f34-112">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="a9f34-112">List secureScores</span></span>](../api/security-list-securescores.md) | <span data-ttu-id="a9f34-113">[secureScores](securescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="a9f34-113">[secureScores](securescore.md) collection</span></span> |<span data-ttu-id="a9f34-114">获取 secureScore 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a9f34-114">Get secureScore object collection.</span></span>|
|[<span data-ttu-id="a9f34-115">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="a9f34-115">Get secureScore</span></span>](../api/securescore-get.md) | [<span data-ttu-id="a9f34-116">secureScore</span><span class="sxs-lookup"><span data-stu-id="a9f34-116">secureScore</span></span>](securescore.md) |<span data-ttu-id="a9f34-117">读取 secureScore 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="a9f34-117">Read properties and metadata of a secureScore object.</span></span> | 



## <a name="properties"></a><span data-ttu-id="a9f34-118">属性</span><span class="sxs-lookup"><span data-stu-id="a9f34-118">Properties</span></span>

|<span data-ttu-id="a9f34-119">属性</span><span class="sxs-lookup"><span data-stu-id="a9f34-119">Property</span></span> |<span data-ttu-id="a9f34-120">类型</span><span class="sxs-lookup"><span data-stu-id="a9f34-120">Type</span></span> |<span data-ttu-id="a9f34-121">说明</span><span class="sxs-lookup"><span data-stu-id="a9f34-121">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a9f34-122">id</span><span class="sxs-lookup"><span data-stu-id="a9f34-122">id</span></span> |<span data-ttu-id="a9f34-123">String</span><span class="sxs-lookup"><span data-stu-id="a9f34-123">String</span></span>|<span data-ttu-id="a9f34-124">提供程序生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a9f34-124">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="a9f34-125">只读。</span><span class="sxs-lookup"><span data-stu-id="a9f34-125">Read-only.</span></span> <span data-ttu-id="a9f34-126">必需。</span><span class="sxs-lookup"><span data-stu-id="a9f34-126">Required.</span></span>|
|   <span data-ttu-id="a9f34-127">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="a9f34-127">azureTenantId</span></span>   |   <span data-ttu-id="a9f34-128">字符串</span><span class="sxs-lookup"><span data-stu-id="a9f34-128">String</span></span>  |   <span data-ttu-id="a9f34-129">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="a9f34-129">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="a9f34-130">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="a9f34-130">activeUserCount</span></span> |   <span data-ttu-id="a9f34-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f34-131">Int32</span></span>   |   <span data-ttu-id="a9f34-132">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-132">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="a9f34-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f34-133">createdDateTime</span></span> |   <span data-ttu-id="a9f34-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f34-134">DateTimeOffset</span></span>  |   <span data-ttu-id="a9f34-135">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="a9f34-135">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="a9f34-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="a9f34-136">currentScore</span></span>    |   <span data-ttu-id="a9f34-137">双精度</span><span class="sxs-lookup"><span data-stu-id="a9f34-137">Double</span></span>  |   <span data-ttu-id="a9f34-138">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="a9f34-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="a9f34-139">enabledServices</span><span class="sxs-lookup"><span data-stu-id="a9f34-139">enabledServices</span></span> |   <span data-ttu-id="a9f34-140">String collection</span><span class="sxs-lookup"><span data-stu-id="a9f34-140">String collection</span></span>   |   <span data-ttu-id="a9f34-141">适用于租户的 Microsoft 提供的服务 (例如, Exchange online、Skype、Sharepoint)。</span><span class="sxs-lookup"><span data-stu-id="a9f34-141">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="a9f34-142">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="a9f34-142">licensedUserCount</span></span>   |   <span data-ttu-id="a9f34-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f34-143">Int32</span></span>   |   <span data-ttu-id="a9f34-144">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-144">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="a9f34-145">maxScore</span><span class="sxs-lookup"><span data-stu-id="a9f34-145">maxScore</span></span> |  <span data-ttu-id="a9f34-146">双精度</span><span class="sxs-lookup"><span data-stu-id="a9f34-146">Double</span></span>  |   <span data-ttu-id="a9f34-147">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-147">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="a9f34-148">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="a9f34-148">averageComparativeScores</span></span> |  <span data-ttu-id="a9f34-149">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="a9f34-149">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="a9f34-150">作用域内不同作用域 (例如, 按行业划分的平均分数、按座位的平均方式) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="a9f34-150">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="a9f34-151">controlScores</span><span class="sxs-lookup"><span data-stu-id="a9f34-151">controlScores</span></span> | <span data-ttu-id="a9f34-152">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="a9f34-152">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="a9f34-153">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="a9f34-153">Contains tenant scores for a set of controls.</span></span>   |
|<span data-ttu-id="a9f34-154">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="a9f34-154">vendorInformation</span></span> |[<span data-ttu-id="a9f34-155">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="a9f34-155">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="a9f34-156">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = SecureScore)。</span><span class="sxs-lookup"><span data-stu-id="a9f34-156">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="a9f34-157">必需。</span><span class="sxs-lookup"><span data-stu-id="a9f34-157">Required.</span></span>|


## <a name="relationships"></a><span data-ttu-id="a9f34-158">关系</span><span class="sxs-lookup"><span data-stu-id="a9f34-158">Relationships</span></span>

<span data-ttu-id="a9f34-159">无。</span><span class="sxs-lookup"><span data-stu-id="a9f34-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9f34-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9f34-160">JSON representation</span></span>

<span data-ttu-id="a9f34-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9f34-161">The following is a JSON representation of the resource.</span></span>

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
