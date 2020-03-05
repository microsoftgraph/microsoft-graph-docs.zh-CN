---
title: secureScore 资源类型
description: 'top = n，其中 n = 要检索的数据的天数。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9c699ced69587d3e9791d22bc464013907319620
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520855"
---
# <a name="securescore-resource-type"></a><span data-ttu-id="ee676-103">secureScore 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee676-103">secureScore resource type</span></span>

<span data-ttu-id="ee676-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ee676-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee676-105">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="ee676-105">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="ee676-106">默认情况下，将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="ee676-106">By default, 90 days of data is held.</span></span> <span data-ttu-id="ee676-107">此数据按**createdDateTime**进行排序，从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="ee676-107">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="ee676-108">这将允许您使用 $top = n 对响应进行分页，其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="ee676-108">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="ee676-109">方法</span><span class="sxs-lookup"><span data-stu-id="ee676-109">Methods</span></span>

| <span data-ttu-id="ee676-110">方法</span><span class="sxs-lookup"><span data-stu-id="ee676-110">Method</span></span>   | <span data-ttu-id="ee676-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee676-111">Return Type</span></span>|<span data-ttu-id="ee676-112">说明</span><span class="sxs-lookup"><span data-stu-id="ee676-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee676-113">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="ee676-113">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="ee676-114">secureScores</span><span class="sxs-lookup"><span data-stu-id="ee676-114">secureScores</span></span>](securescores.md) |<span data-ttu-id="ee676-115">读取 secureScores 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="ee676-115">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="ee676-116">属性</span><span class="sxs-lookup"><span data-stu-id="ee676-116">Properties</span></span>
<span data-ttu-id="ee676-117">包含租户安全分数（每日快照数据）的属性的实体类型。</span><span class="sxs-lookup"><span data-stu-id="ee676-117">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="ee676-118">属性</span><span class="sxs-lookup"><span data-stu-id="ee676-118">Property</span></span> |<span data-ttu-id="ee676-119">类型</span><span class="sxs-lookup"><span data-stu-id="ee676-119">Type</span></span> |<span data-ttu-id="ee676-120">说明</span><span class="sxs-lookup"><span data-stu-id="ee676-120">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ee676-121">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="ee676-121">azureTenantId</span></span>   |   <span data-ttu-id="ee676-122">字符串</span><span class="sxs-lookup"><span data-stu-id="ee676-122">String</span></span>  |   <span data-ttu-id="ee676-123">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="ee676-123">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="ee676-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee676-124">createdDateTime</span></span> |   <span data-ttu-id="ee676-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee676-125">DateTimeOffset</span></span>  |   <span data-ttu-id="ee676-126">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="ee676-126">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="ee676-127">id</span><span class="sxs-lookup"><span data-stu-id="ee676-127">id</span></span>  |   <span data-ttu-id="ee676-128">String</span><span class="sxs-lookup"><span data-stu-id="ee676-128">String</span></span>  |   <span data-ttu-id="ee676-129">AzureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="ee676-129">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="ee676-130">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="ee676-130">licensedUserCount</span></span>   |   <span data-ttu-id="ee676-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ee676-131">Int32</span></span>   |   <span data-ttu-id="ee676-132">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="ee676-132">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="ee676-133">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="ee676-133">activeUserCount</span></span> |   <span data-ttu-id="ee676-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ee676-134">Int32</span></span>   |   <span data-ttu-id="ee676-135">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="ee676-135">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="ee676-136">currentScore</span><span class="sxs-lookup"><span data-stu-id="ee676-136">currentScore</span></span>    |   <span data-ttu-id="ee676-137">双精度</span><span class="sxs-lookup"><span data-stu-id="ee676-137">Double</span></span>  |   <span data-ttu-id="ee676-138">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="ee676-138">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="ee676-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="ee676-139">maxScore</span></span> |  <span data-ttu-id="ee676-140">双精度</span><span class="sxs-lookup"><span data-stu-id="ee676-140">Double</span></span>  |   <span data-ttu-id="ee676-141">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="ee676-141">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="ee676-142">enabledServices</span><span class="sxs-lookup"><span data-stu-id="ee676-142">enabledServices</span></span> |   <span data-ttu-id="ee676-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="ee676-143">String collection</span></span>   |   <span data-ttu-id="ee676-144">适用于租户的 Microsoft 提供的服务（例如，Exchange online、Skype、Sharepoint）。</span><span class="sxs-lookup"><span data-stu-id="ee676-144">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="ee676-145">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="ee676-145">averageComparativeScores</span></span> |  <span data-ttu-id="ee676-146">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="ee676-146">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="ee676-147">作用域内不同作用域（例如，按行业划分的平均分数、按座位的平均方式）和控制类别（标识、数据、设备、应用程序、基础结构）。</span><span class="sxs-lookup"><span data-stu-id="ee676-147">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="ee676-148">controlScores</span><span class="sxs-lookup"><span data-stu-id="ee676-148">controlScores</span></span> | <span data-ttu-id="ee676-149">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="ee676-149">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="ee676-150">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="ee676-150">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="ee676-151">关系</span><span class="sxs-lookup"><span data-stu-id="ee676-151">Relationships</span></span>

<span data-ttu-id="ee676-152">无。</span><span class="sxs-lookup"><span data-stu-id="ee676-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee676-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee676-153">JSON representation</span></span>

<span data-ttu-id="ee676-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee676-154">The following is a JSON representation of the resource.</span></span>

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
