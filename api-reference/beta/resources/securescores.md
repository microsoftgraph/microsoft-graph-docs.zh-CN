---
title: secureScores 资源类型
description: '顶部 = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576078"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="17f3e-103">secureScores 资源类型</span><span class="sxs-lookup"><span data-stu-id="17f3e-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17f3e-104">代表租户的租户和控制级别记分数据，每天安全分数。</span><span class="sxs-lookup"><span data-stu-id="17f3e-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="17f3e-105">默认情况下保留 90 天的数据。</span><span class="sxs-lookup"><span data-stu-id="17f3e-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="17f3e-106">此数据排序依据**createdDateTime**，从最新公开到最早。</span><span class="sxs-lookup"><span data-stu-id="17f3e-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="17f3e-107">这将允许您向页响应使用 $top = n，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="17f3e-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="17f3e-108">方法</span><span class="sxs-lookup"><span data-stu-id="17f3e-108">Methods</span></span>

| <span data-ttu-id="17f3e-109">方法</span><span class="sxs-lookup"><span data-stu-id="17f3e-109">Method</span></span>   | <span data-ttu-id="17f3e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="17f3e-110">Return Type</span></span>|<span data-ttu-id="17f3e-111">说明</span><span class="sxs-lookup"><span data-stu-id="17f3e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17f3e-112">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="17f3e-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="17f3e-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="17f3e-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="17f3e-114">读取属性和 secureScores 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="17f3e-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="17f3e-115">属性</span><span class="sxs-lookup"><span data-stu-id="17f3e-115">Properties</span></span>
<span data-ttu-id="17f3e-116">实体类型包含属性的租户安全得分 （每日快照数据）。</span><span class="sxs-lookup"><span data-stu-id="17f3e-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="17f3e-117">属性</span><span class="sxs-lookup"><span data-stu-id="17f3e-117">Property</span></span> |<span data-ttu-id="17f3e-118">类型</span><span class="sxs-lookup"><span data-stu-id="17f3e-118">Type</span></span> |<span data-ttu-id="17f3e-119">说明</span><span class="sxs-lookup"><span data-stu-id="17f3e-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="17f3e-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="17f3e-120">azureTenantId</span></span>   |   <span data-ttu-id="17f3e-121">String</span><span class="sxs-lookup"><span data-stu-id="17f3e-121">String</span></span>  |   <span data-ttu-id="17f3e-122">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="17f3e-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="17f3e-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17f3e-123">createdDateTime</span></span> |   <span data-ttu-id="17f3e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f3e-124">DateTimeOffset</span></span>  |   <span data-ttu-id="17f3e-125">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="17f3e-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="17f3e-126">id</span><span class="sxs-lookup"><span data-stu-id="17f3e-126">id</span></span>  |   <span data-ttu-id="17f3e-127">String</span><span class="sxs-lookup"><span data-stu-id="17f3e-127">String</span></span>  |   <span data-ttu-id="17f3e-128">AzureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="17f3e-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="17f3e-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="17f3e-129">licensedUserCount</span></span>   |   <span data-ttu-id="17f3e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="17f3e-130">Int32</span></span>   |   <span data-ttu-id="17f3e-131">许可的给定租户的用户计数。</span><span class="sxs-lookup"><span data-stu-id="17f3e-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="17f3e-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="17f3e-132">activeUserCount</span></span> |   <span data-ttu-id="17f3e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="17f3e-133">Int32</span></span>   |   <span data-ttu-id="17f3e-134">给定租户的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="17f3e-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="17f3e-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="17f3e-135">currentScore</span></span>    |   <span data-ttu-id="17f3e-136">双精度</span><span class="sxs-lookup"><span data-stu-id="17f3e-136">Double</span></span>  |   <span data-ttu-id="17f3e-137">在指定日期的租户当前获得分数。</span><span class="sxs-lookup"><span data-stu-id="17f3e-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="17f3e-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="17f3e-138">maxScore</span></span> |  <span data-ttu-id="17f3e-139">双精度</span><span class="sxs-lookup"><span data-stu-id="17f3e-139">Double</span></span>  |   <span data-ttu-id="17f3e-140">在指定日期租户最大得分。</span><span class="sxs-lookup"><span data-stu-id="17f3e-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="17f3e-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="17f3e-141">enabledServices</span></span> |   <span data-ttu-id="17f3e-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="17f3e-142">String collection</span></span>   |   <span data-ttu-id="17f3e-143">租户 （例如，Exchange online、 Skype、 Sharepoint） 的 Microsoft 提供服务。</span><span class="sxs-lookup"><span data-stu-id="17f3e-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="17f3e-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="17f3e-144">averageComparativeScores</span></span> |  <span data-ttu-id="17f3e-145">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="17f3e-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="17f3e-146">按不同的作用域 （例如，按行业，平均由安装的平均） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 范围内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="17f3e-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="17f3e-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="17f3e-147">controlScores</span></span> | <span data-ttu-id="17f3e-148">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="17f3e-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="17f3e-149">包含租户分数的一组控件。</span><span class="sxs-lookup"><span data-stu-id="17f3e-149">Contains tenant scores for a set of controls.</span></span>   |
|   <span data-ttu-id="17f3e-150">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="17f3e-150">vendorInformation</span></span> | [<span data-ttu-id="17f3e-151">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="17f3e-151">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="17f3e-152">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="17f3e-152">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="17f3e-153">关系</span><span class="sxs-lookup"><span data-stu-id="17f3e-153">Relationships</span></span>

<span data-ttu-id="17f3e-154">无。</span><span class="sxs-lookup"><span data-stu-id="17f3e-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17f3e-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17f3e-155">JSON representation</span></span>

<span data-ttu-id="17f3e-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17f3e-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
    "id": "String",
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
