---
title: secureScore 资源类型
description: 'top = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3db31203f9c5827459ab2149efbd3adb28030d0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087542"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="980d2-103">secureScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="980d2-103">secureScore resource type</span></span>

<span data-ttu-id="980d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="980d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="980d2-105">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="980d2-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="980d2-106">默认情况下，将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="980d2-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="980d2-107">此数据按 **createdDateTime**进行排序，从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="980d2-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="980d2-108">这将允许您使用 $top = n 对响应进行分页，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="980d2-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span>


## <a name="methods"></a><span data-ttu-id="980d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="980d2-109">Methods</span></span>

| <span data-ttu-id="980d2-110">方法</span><span class="sxs-lookup"><span data-stu-id="980d2-110">Method</span></span>   | <span data-ttu-id="980d2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="980d2-111">Return Type</span></span>|<span data-ttu-id="980d2-112">说明</span><span class="sxs-lookup"><span data-stu-id="980d2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="980d2-113">列出 secureScore</span><span class="sxs-lookup"><span data-stu-id="980d2-113">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="980d2-114">secureScores</span><span class="sxs-lookup"><span data-stu-id="980d2-114">secureScores</span></span>](securescores.md) |<span data-ttu-id="980d2-115">读取 secureScores 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="980d2-115">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="980d2-116">属性</span><span class="sxs-lookup"><span data-stu-id="980d2-116">Properties</span></span>
<span data-ttu-id="980d2-117">包含租户安全分数的属性的实体类型 (每日快照数据) 。</span><span class="sxs-lookup"><span data-stu-id="980d2-117">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="980d2-118">属性</span><span class="sxs-lookup"><span data-stu-id="980d2-118">Property</span></span> |<span data-ttu-id="980d2-119">类型</span><span class="sxs-lookup"><span data-stu-id="980d2-119">Type</span></span> |<span data-ttu-id="980d2-120">说明</span><span class="sxs-lookup"><span data-stu-id="980d2-120">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="980d2-121">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="980d2-121">azureTenantId</span></span>   |   <span data-ttu-id="980d2-122">字符串</span><span class="sxs-lookup"><span data-stu-id="980d2-122">String</span></span>  |   <span data-ttu-id="980d2-123">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="980d2-123">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="980d2-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="980d2-124">createdDateTime</span></span> |   <span data-ttu-id="980d2-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980d2-125">DateTimeOffset</span></span>  |   <span data-ttu-id="980d2-126">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="980d2-126">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="980d2-127">id</span><span class="sxs-lookup"><span data-stu-id="980d2-127">id</span></span>  |   <span data-ttu-id="980d2-128">字符串</span><span class="sxs-lookup"><span data-stu-id="980d2-128">String</span></span>  |   <span data-ttu-id="980d2-129">AzureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="980d2-129">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="980d2-130">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="980d2-130">licensedUserCount</span></span>   |   <span data-ttu-id="980d2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="980d2-131">Int32</span></span>   |   <span data-ttu-id="980d2-132">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="980d2-132">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="980d2-133">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="980d2-133">activeUserCount</span></span> |   <span data-ttu-id="980d2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="980d2-134">Int32</span></span>   |   <span data-ttu-id="980d2-135">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="980d2-135">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="980d2-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="980d2-136">currentScore</span></span>    |   <span data-ttu-id="980d2-137">双精度</span><span class="sxs-lookup"><span data-stu-id="980d2-137">Double</span></span>  |   <span data-ttu-id="980d2-138">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="980d2-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="980d2-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="980d2-139">maxScore</span></span> |  <span data-ttu-id="980d2-140">双精度</span><span class="sxs-lookup"><span data-stu-id="980d2-140">Double</span></span>  |   <span data-ttu-id="980d2-141">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="980d2-141">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="980d2-142">enabledServices</span><span class="sxs-lookup"><span data-stu-id="980d2-142">enabledServices</span></span> |   <span data-ttu-id="980d2-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="980d2-143">String collection</span></span>   |   <span data-ttu-id="980d2-144">Microsoft 为租户提供的服务 (例如，Exchange online、Skype、Sharepoint) 。</span><span class="sxs-lookup"><span data-stu-id="980d2-144">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="980d2-145">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="980d2-145">averageComparativeScores</span></span> |  <span data-ttu-id="980d2-146">[averageComparativeScore](averagecomparativescore.md) 集合</span><span class="sxs-lookup"><span data-stu-id="980d2-146">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="980d2-147">不同作用域的平均分数 (例如，行业平均值、座位) 和控制类别的平均 (标识、数据、设备、应用程序、基础结构) 在范围内。</span><span class="sxs-lookup"><span data-stu-id="980d2-147">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="980d2-148">controlScores</span><span class="sxs-lookup"><span data-stu-id="980d2-148">controlScores</span></span> | <span data-ttu-id="980d2-149">[controlScore](controlscore.md) 集合</span><span class="sxs-lookup"><span data-stu-id="980d2-149">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="980d2-150">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="980d2-150">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="980d2-151">关系</span><span class="sxs-lookup"><span data-stu-id="980d2-151">Relationships</span></span>

<span data-ttu-id="980d2-152">无。</span><span class="sxs-lookup"><span data-stu-id="980d2-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="980d2-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="980d2-153">JSON representation</span></span>

<span data-ttu-id="980d2-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="980d2-154">The following is a JSON representation of the resource.</span></span>

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


