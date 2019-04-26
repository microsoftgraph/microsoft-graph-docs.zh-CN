---
title: secureScore 资源类型
description: 'top = n, 其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: 1f4ee37b5e257cfb914f45a1260f3572403f00dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343372"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="2c8be-103">secureScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c8be-103">secureScore resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c8be-104">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="2c8be-105">默认情况下, 将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="2c8be-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="2c8be-106">此数据按**createdDateTime**进行排序, 从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="2c8be-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="2c8be-107">这将允许您使用 $top = n 对响应进行分页, 其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="2c8be-108">方法</span><span class="sxs-lookup"><span data-stu-id="2c8be-108">Methods</span></span>

| <span data-ttu-id="2c8be-109">方法</span><span class="sxs-lookup"><span data-stu-id="2c8be-109">Method</span></span>   | <span data-ttu-id="2c8be-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c8be-110">Return Type</span></span>|<span data-ttu-id="2c8be-111">说明</span><span class="sxs-lookup"><span data-stu-id="2c8be-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c8be-112">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="2c8be-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="2c8be-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="2c8be-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="2c8be-114">读取 secureScores 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="2c8be-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="2c8be-115">属性</span><span class="sxs-lookup"><span data-stu-id="2c8be-115">Properties</span></span>
<span data-ttu-id="2c8be-116">包含租户安全分数 (每日快照数据) 的属性的实体类型。</span><span class="sxs-lookup"><span data-stu-id="2c8be-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="2c8be-117">属性</span><span class="sxs-lookup"><span data-stu-id="2c8be-117">Property</span></span> |<span data-ttu-id="2c8be-118">类型</span><span class="sxs-lookup"><span data-stu-id="2c8be-118">Type</span></span> |<span data-ttu-id="2c8be-119">说明</span><span class="sxs-lookup"><span data-stu-id="2c8be-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="2c8be-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="2c8be-120">azureTenantId</span></span>   |   <span data-ttu-id="2c8be-121">String</span><span class="sxs-lookup"><span data-stu-id="2c8be-121">String</span></span>  |   <span data-ttu-id="2c8be-122">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="2c8be-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="2c8be-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c8be-123">createdDateTime</span></span> |   <span data-ttu-id="2c8be-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c8be-124">DateTimeOffset</span></span>  |   <span data-ttu-id="2c8be-125">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="2c8be-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="2c8be-126">id</span><span class="sxs-lookup"><span data-stu-id="2c8be-126">id</span></span>  |   <span data-ttu-id="2c8be-127">String</span><span class="sxs-lookup"><span data-stu-id="2c8be-127">String</span></span>  |   <span data-ttu-id="2c8be-128">azureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="2c8be-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="2c8be-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="2c8be-129">licensedUserCount</span></span>   |   <span data-ttu-id="2c8be-130">Int32</span><span class="sxs-lookup"><span data-stu-id="2c8be-130">Int32</span></span>   |   <span data-ttu-id="2c8be-131">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="2c8be-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="2c8be-132">activeUserCount</span></span> |   <span data-ttu-id="2c8be-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2c8be-133">Int32</span></span>   |   <span data-ttu-id="2c8be-134">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="2c8be-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="2c8be-135">currentScore</span></span>    |   <span data-ttu-id="2c8be-136">双精度</span><span class="sxs-lookup"><span data-stu-id="2c8be-136">Double</span></span>  |   <span data-ttu-id="2c8be-137">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="2c8be-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="2c8be-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="2c8be-138">maxScore</span></span> |  <span data-ttu-id="2c8be-139">双精度</span><span class="sxs-lookup"><span data-stu-id="2c8be-139">Double</span></span>  |   <span data-ttu-id="2c8be-140">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="2c8be-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="2c8be-141">enabledServices</span></span> |   <span data-ttu-id="2c8be-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="2c8be-142">String collection</span></span>   |   <span data-ttu-id="2c8be-143">适用于租户的 Microsoft 提供的服务 (例如, Exchange online、Skype、Sharepoint)。</span><span class="sxs-lookup"><span data-stu-id="2c8be-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="2c8be-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="2c8be-144">averageComparativeScores</span></span> |  <span data-ttu-id="2c8be-145">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c8be-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="2c8be-146">作用域内不同作用域 (例如, 按行业划分的平均分数、按座位的平均方式) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="2c8be-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="2c8be-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="2c8be-147">controlScores</span></span> | <span data-ttu-id="2c8be-148">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c8be-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="2c8be-149">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="2c8be-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="2c8be-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="2c8be-150">Relationships</span></span>

<span data-ttu-id="2c8be-151">无。</span><span class="sxs-lookup"><span data-stu-id="2c8be-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8be-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c8be-152">JSON representation</span></span>

<span data-ttu-id="2c8be-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c8be-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
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
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
