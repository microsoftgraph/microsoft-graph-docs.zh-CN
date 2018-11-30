---
title: secureScores 资源类型
description: '顶部 = n，其中 n = 要检索的数据的天数。 '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042314"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="7ebe0-103">secureScores 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ebe0-103">secureScores resource type</span></span>

> <span data-ttu-id="7ebe0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ebe0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ebe0-106">代表租户的租户和控制级别记分数据，每天安全分数。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="7ebe0-107">默认情况下保留 90 天的数据。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="7ebe0-108">此数据排序依据**createdDateTime**，从最新公开到最早。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="7ebe0-109">这将允许您向页响应使用 $top = n，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="7ebe0-110">方法</span><span class="sxs-lookup"><span data-stu-id="7ebe0-110">Methods</span></span>

| <span data-ttu-id="7ebe0-111">方法</span><span class="sxs-lookup"><span data-stu-id="7ebe0-111">Method</span></span>   | <span data-ttu-id="7ebe0-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ebe0-112">Return Type</span></span>|<span data-ttu-id="7ebe0-113">说明</span><span class="sxs-lookup"><span data-stu-id="7ebe0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ebe0-114">列表 secureScores</span><span class="sxs-lookup"><span data-stu-id="7ebe0-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="7ebe0-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="7ebe0-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="7ebe0-116">读取属性和 secureScores 对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="7ebe0-117">属性</span><span class="sxs-lookup"><span data-stu-id="7ebe0-117">Properties</span></span>
<span data-ttu-id="7ebe0-118">实体类型包含属性的租户安全得分 （每日快照数据）。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="7ebe0-119">属性</span><span class="sxs-lookup"><span data-stu-id="7ebe0-119">Property</span></span> |<span data-ttu-id="7ebe0-120">类型</span><span class="sxs-lookup"><span data-stu-id="7ebe0-120">Type</span></span> |<span data-ttu-id="7ebe0-121">说明</span><span class="sxs-lookup"><span data-stu-id="7ebe0-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="7ebe0-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="7ebe0-122">azureTenantId</span></span>   |   <span data-ttu-id="7ebe0-123">字符串</span><span class="sxs-lookup"><span data-stu-id="7ebe0-123">String</span></span>  |   <span data-ttu-id="7ebe0-124">GUID string 租户 id。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="7ebe0-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ebe0-125">createdDateTime</span></span> |   <span data-ttu-id="7ebe0-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ebe0-126">DateTimeOffset</span></span>  |   <span data-ttu-id="7ebe0-127">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="7ebe0-128">id</span><span class="sxs-lookup"><span data-stu-id="7ebe0-128">id</span></span>  |   <span data-ttu-id="7ebe0-129">字符串</span><span class="sxs-lookup"><span data-stu-id="7ebe0-129">String</span></span>  |   <span data-ttu-id="7ebe0-130">AzureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="7ebe0-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="7ebe0-131">licensedUserCount</span></span>   |   <span data-ttu-id="7ebe0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7ebe0-132">Int32</span></span>   |   <span data-ttu-id="7ebe0-133">许可的给定租户的用户计数。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="7ebe0-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="7ebe0-134">activeUserCount</span></span> |   <span data-ttu-id="7ebe0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7ebe0-135">Int32</span></span>   |   <span data-ttu-id="7ebe0-136">给定租户的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="7ebe0-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="7ebe0-137">currentScore</span></span>    |   <span data-ttu-id="7ebe0-138">双精度数</span><span class="sxs-lookup"><span data-stu-id="7ebe0-138">Double</span></span>  |   <span data-ttu-id="7ebe0-139">在指定日期的租户当前获得分数。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="7ebe0-140">maxScore</span><span class="sxs-lookup"><span data-stu-id="7ebe0-140">maxScore</span></span> |  <span data-ttu-id="7ebe0-141">双精度数</span><span class="sxs-lookup"><span data-stu-id="7ebe0-141">Double</span></span>  |   <span data-ttu-id="7ebe0-142">在指定日期租户最大得分。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="7ebe0-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="7ebe0-143">enabledServices</span></span> |   <span data-ttu-id="7ebe0-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="7ebe0-144">String collection</span></span>   |   <span data-ttu-id="7ebe0-145">租户 （例如，Exchange online、 Skype、 Sharepoint） 的 Microsoft 提供服务。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="7ebe0-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="7ebe0-146">averageComparativeScores</span></span> |  <span data-ttu-id="7ebe0-147">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ebe0-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="7ebe0-148">按不同的作用域 （例如，按行业，平均由安装的平均） 和控制类别 （Identity、 数据、 设备、 应用程序、 基础结构） 范围内的平均得分。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="7ebe0-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="7ebe0-149">controlScores</span></span> | <span data-ttu-id="7ebe0-150">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ebe0-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="7ebe0-151">包含租户分数的一组控件。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="7ebe0-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="7ebe0-152">Relationships</span></span>

<span data-ttu-id="7ebe0-153">无。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ebe0-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ebe0-154">JSON representation</span></span>

<span data-ttu-id="7ebe0-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ebe0-155">The following is a JSON representation of the resource.</span></span>

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
