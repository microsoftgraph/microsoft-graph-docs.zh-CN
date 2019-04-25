---
title: secureScores 资源类型
description: 'top = n, 其中 n = 要检索的数据的天数。 '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549200"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="26c30-103">secureScores 资源类型</span><span class="sxs-lookup"><span data-stu-id="26c30-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26c30-104">表示租户和控制级别上的每日记分数据的租户安全分数。</span><span class="sxs-lookup"><span data-stu-id="26c30-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="26c30-105">默认情况下, 将保留90天的数据。</span><span class="sxs-lookup"><span data-stu-id="26c30-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="26c30-106">此数据按**createdDateTime**进行排序, 从最新到最早。</span><span class="sxs-lookup"><span data-stu-id="26c30-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="26c30-107">这将允许您使用 $top = n 对响应进行分页, 其中 n = 要检索的数据的天数。</span><span class="sxs-lookup"><span data-stu-id="26c30-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="26c30-108">方法</span><span class="sxs-lookup"><span data-stu-id="26c30-108">Methods</span></span>

| <span data-ttu-id="26c30-109">方法</span><span class="sxs-lookup"><span data-stu-id="26c30-109">Method</span></span>   | <span data-ttu-id="26c30-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="26c30-110">Return Type</span></span>|<span data-ttu-id="26c30-111">说明</span><span class="sxs-lookup"><span data-stu-id="26c30-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26c30-112">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="26c30-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="26c30-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="26c30-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="26c30-114">读取 secureScores 对象的属性和元数据。</span><span class="sxs-lookup"><span data-stu-id="26c30-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="26c30-115">属性</span><span class="sxs-lookup"><span data-stu-id="26c30-115">Properties</span></span>
<span data-ttu-id="26c30-116">包含租户安全分数 (每日快照数据) 的属性的实体类型。</span><span class="sxs-lookup"><span data-stu-id="26c30-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="26c30-117">属性</span><span class="sxs-lookup"><span data-stu-id="26c30-117">Property</span></span> |<span data-ttu-id="26c30-118">类型</span><span class="sxs-lookup"><span data-stu-id="26c30-118">Type</span></span> |<span data-ttu-id="26c30-119">说明</span><span class="sxs-lookup"><span data-stu-id="26c30-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="26c30-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="26c30-120">azureTenantId</span></span>   |   <span data-ttu-id="26c30-121">String</span><span class="sxs-lookup"><span data-stu-id="26c30-121">String</span></span>  |   <span data-ttu-id="26c30-122">租户 ID 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="26c30-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="26c30-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26c30-123">createdDateTime</span></span> |   <span data-ttu-id="26c30-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26c30-124">DateTimeOffset</span></span>  |   <span data-ttu-id="26c30-125">创建实体的日期。</span><span class="sxs-lookup"><span data-stu-id="26c30-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="26c30-126">id</span><span class="sxs-lookup"><span data-stu-id="26c30-126">id</span></span>  |   <span data-ttu-id="26c30-127">String</span><span class="sxs-lookup"><span data-stu-id="26c30-127">String</span></span>  |   <span data-ttu-id="26c30-128">azureTenantId_createdDateTime 的组合。</span><span class="sxs-lookup"><span data-stu-id="26c30-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="26c30-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="26c30-129">licensedUserCount</span></span>   |   <span data-ttu-id="26c30-130">Int32</span><span class="sxs-lookup"><span data-stu-id="26c30-130">Int32</span></span>   |   <span data-ttu-id="26c30-131">给定租户的许可用户计数。</span><span class="sxs-lookup"><span data-stu-id="26c30-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="26c30-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="26c30-132">activeUserCount</span></span> |   <span data-ttu-id="26c30-133">Int32</span><span class="sxs-lookup"><span data-stu-id="26c30-133">Int32</span></span>   |   <span data-ttu-id="26c30-134">给定租户的活动用户计数。</span><span class="sxs-lookup"><span data-stu-id="26c30-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="26c30-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="26c30-135">currentScore</span></span>    |   <span data-ttu-id="26c30-136">双精度</span><span class="sxs-lookup"><span data-stu-id="26c30-136">Double</span></span>  |   <span data-ttu-id="26c30-137">租户当前在指定日期的得分。</span><span class="sxs-lookup"><span data-stu-id="26c30-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="26c30-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="26c30-138">maxScore</span></span> |  <span data-ttu-id="26c30-139">双精度</span><span class="sxs-lookup"><span data-stu-id="26c30-139">Double</span></span>  |   <span data-ttu-id="26c30-140">指定日期上可能的租户最大分数。</span><span class="sxs-lookup"><span data-stu-id="26c30-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="26c30-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="26c30-141">enabledServices</span></span> |   <span data-ttu-id="26c30-142">String collection</span><span class="sxs-lookup"><span data-stu-id="26c30-142">String collection</span></span>   |   <span data-ttu-id="26c30-143">适用于租户的 Microsoft 提供的服务 (例如, Exchange online、Skype、Sharepoint)。</span><span class="sxs-lookup"><span data-stu-id="26c30-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="26c30-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="26c30-144">averageComparativeScores</span></span> |  <span data-ttu-id="26c30-145">[averageComparativeScore](averagecomparativescore.md)集合</span><span class="sxs-lookup"><span data-stu-id="26c30-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="26c30-146">作用域内不同作用域 (例如, 按行业划分的平均分数、按座位的平均方式) 和控制类别 (标识、数据、设备、应用程序、基础结构)。</span><span class="sxs-lookup"><span data-stu-id="26c30-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="26c30-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="26c30-147">controlScores</span></span> | <span data-ttu-id="26c30-148">[controlScore](controlscore.md)集合</span><span class="sxs-lookup"><span data-stu-id="26c30-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="26c30-149">包含一组控件的租户分数。</span><span class="sxs-lookup"><span data-stu-id="26c30-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="26c30-150">关系</span><span class="sxs-lookup"><span data-stu-id="26c30-150">Relationships</span></span>

<span data-ttu-id="26c30-151">无。</span><span class="sxs-lookup"><span data-stu-id="26c30-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26c30-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26c30-152">JSON representation</span></span>

<span data-ttu-id="26c30-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26c30-153">The following is a JSON representation of the resource.</span></span>

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
