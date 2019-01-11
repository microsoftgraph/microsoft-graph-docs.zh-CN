---
title: secureScores 资源类型
description: '顶部 = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: 332a9656d8237bb07d5c7739b666e09539cf984f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828733"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="ffc88-103">secureScores 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffc88-103">secureScores resource type</span></span>

> <span data-ttu-id="ffc88-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffc88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffc88-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffc88-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffc88-106">代表租户的租户和控制级别记分数据，每天安全分数。</span><span class="sxs-lookup"><span data-stu-id="ffc88-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="ffc88-107">默认情况下保留 90 天的数据。</span><span class="sxs-lookup"><span data-stu-id="ffc88-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="ffc88-108">此数据排序依据**createdDateTime**，从最新公开到最早。</span><span class="sxs-lookup"><span data-stu-id="ffc88-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="ffc88-109">这将允许您向页响应使用 $top = n，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="ffc88-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="ffc88-110">方法</span><span class="sxs-lookup"><span data-stu-id="ffc88-110">Methods</span></span>

| <span data-ttu-id="ffc88-111">方法</span><span class="sxs-lookup"><span data-stu-id="ffc88-111">Method</span></span>   | <span data-ttu-id="ffc88-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffc88-112">Return Type</span></span>|<span data-ttu-id="ffc88-113">说明</span><span class="sxs-lookup"><span data-stu-id="ffc88-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffc88-114">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="ffc88-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="ffc88-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="ffc88-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="ffc88-116">读取属性和 secureScores 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="ffc88-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ffc88-117">属性</span><span class="sxs-lookup"><span data-stu-id="ffc88-117">Properties</span></span>
<span data-ttu-id="ffc88-118">实体类型包含属性的租户安全得分 （每日快照数据）。</span><span class="sxs-lookup"><span data-stu-id="ffc88-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="ffc88-119">属性</span><span class="sxs-lookup"><span data-stu-id="ffc88-119">Property</span></span> |<span data-ttu-id="ffc88-120">类型</span><span class="sxs-lookup"><span data-stu-id="ffc88-120">Type</span></span> |<span data-ttu-id="ffc88-121">Description</span><span class="sxs-lookup"><span data-stu-id="ffc88-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ffc88-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="ffc88-122">azureTenantId</span></span>   |   <span data-ttu-id="ffc88-123">字符串</span><span class="sxs-lookup"><span data-stu-id="ffc88-123">String</span></span>  |   <span data-ttu-id="ffc88-124">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="ffc88-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="ffc88-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffc88-125">createdDateTime</span></span> |   <span data-ttu-id="ffc88-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffc88-126">DateTimeOffset</span></span>  |   <span data-ttu-id="ffc88-127">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="ffc88-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="ffc88-128">id</span><span class="sxs-lookup"><span data-stu-id="ffc88-128">id</span></span>  |   <span data-ttu-id="ffc88-129">字符串</span><span class="sxs-lookup"><span data-stu-id="ffc88-129">String</span></span>  |   <span data-ttu-id="ffc88-130">AzureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="ffc88-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="ffc88-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="ffc88-131">licensedUserCount</span></span>   |   <span data-ttu-id="ffc88-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ffc88-132">Int32</span></span>   |   <span data-ttu-id="ffc88-133">许可的给定租户的用户计数。</span><span class="sxs-lookup"><span data-stu-id="ffc88-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="ffc88-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="ffc88-134">activeUserCount</span></span> |   <span data-ttu-id="ffc88-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ffc88-135">Int32</span></span>   |   <span data-ttu-id="ffc88-136">给定租户的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="ffc88-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="ffc88-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="ffc88-137">currentScore</span></span>    |   <span data-ttu-id="ffc88-138">Double</span><span class="sxs-lookup"><span data-stu-id="ffc88-138">Double</span></span>  |   <span data-ttu-id="ffc88-139">在指定日期的租户当前获得分数。</span><span class="sxs-lookup"><span data-stu-id="ffc88-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="ffc88-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="ffc88-140">maxScore</span></span> |  <span data-ttu-id="ffc88-141">Double</span><span class="sxs-lookup"><span data-stu-id="ffc88-141">Double</span></span>  |   <span data-ttu-id="ffc88-142">在指定日期租户最大得分。</span><span class="sxs-lookup"><span data-stu-id="ffc88-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="ffc88-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="ffc88-143">enabledServices</span></span> |   <span data-ttu-id="ffc88-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="ffc88-144">String collection</span></span>   |   <span data-ttu-id="ffc88-145">租户 （例如，Exchange online、 Skype、 Sharepoint） 的 Microsoft 提供服务。</span><span class="sxs-lookup"><span data-stu-id="ffc88-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="ffc88-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="ffc88-146">averageComparativeScores</span></span> |  <span data-ttu-id="ffc88-147">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffc88-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="ffc88-148">按不同的作用域 （例如，按行业，平均由安装的平均） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 范围内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="ffc88-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="ffc88-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="ffc88-149">controlScores</span></span> | <span data-ttu-id="ffc88-150">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="ffc88-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="ffc88-151">包含租户分数的一组控件。</span><span class="sxs-lookup"><span data-stu-id="ffc88-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="ffc88-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="ffc88-152">Relationships</span></span>

<span data-ttu-id="ffc88-153">无。</span><span class="sxs-lookup"><span data-stu-id="ffc88-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffc88-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffc88-154">JSON representation</span></span>

<span data-ttu-id="ffc88-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffc88-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
