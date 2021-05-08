---
title: accessReviewHistoryDefinition 资源类型
description: 表示访问评审历史记录数据的集合。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96619cb95c11a77106c86cbdcc720f1a486721c7
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232912"
---
# <a name="accessreviewhistorydefinition-resource-type"></a><span data-ttu-id="5739b-103">accessReviewHistoryDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5739b-103">accessReviewHistoryDefinition resource type</span></span>

<span data-ttu-id="5739b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5739b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5739b-105">表示访问评审历史记录数据和用于收集数据的范围的集合。</span><span class="sxs-lookup"><span data-stu-id="5739b-105">Represents a collection of access review history data and the scopes used to collect that data.</span></span> <span data-ttu-id="5739b-106">**reviewHistoryPeriodStartDateTime**、 **reviewHistoryPeriodEndDateTime**、 **decisions** 和 **scopes** 属性的 **accessReviewHistoryDefinition** are used when selecting review history data， and can be modified.</span><span class="sxs-lookup"><span data-stu-id="5739b-106">The **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions**, and **scopes** properties of an **accessReviewHistoryDefinition** are used when selecting review history data, and can be modified.</span></span> <span data-ttu-id="5739b-107">每个 **accessReviewHistoryDefinition** 对象只能使用 30 天。</span><span class="sxs-lookup"><span data-stu-id="5739b-107">Each **accessReviewHistoryDefinition** object is only available for 30 days.</span></span> <span data-ttu-id="5739b-108">一旦历史记录定义的状态移动到链接，就可以通过调用 `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)来检索定义的数据。</span><span class="sxs-lookup"><span data-stu-id="5739b-108">Once a history definition's status has moved to `done` a link can be generated to retrieve the definition's data by calling [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5739b-109">方法</span><span class="sxs-lookup"><span data-stu-id="5739b-109">Methods</span></span>
|<span data-ttu-id="5739b-110">方法</span><span class="sxs-lookup"><span data-stu-id="5739b-110">Method</span></span>|<span data-ttu-id="5739b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5739b-111">Return type</span></span>|<span data-ttu-id="5739b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5739b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5739b-113">列出 accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="5739b-113">List accessReviewHistoryDefinitions</span></span>](../api/accessreviewhistorydefinition-list.md)|<span data-ttu-id="5739b-114">[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5739b-114">[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) collection</span></span>|<span data-ttu-id="5739b-115">获取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5739b-115">Get a list of the [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) objects and their properties.</span></span>|
|[<span data-ttu-id="5739b-116">创建 accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5739b-116">Create accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-post.md)|[<span data-ttu-id="5739b-117">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5739b-117">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="5739b-118">创建新的 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5739b-118">Create a new [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="5739b-119">获取 accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5739b-119">Get accessReviewHistoryDefinition</span></span>](../api/accessreviewhistorydefinition-get.md)|[<span data-ttu-id="5739b-120">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5739b-120">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="5739b-121">读取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5739b-121">Read the properties and relationships of an [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) object.</span></span>|
|[<span data-ttu-id="5739b-122">generateDownloadUri</span><span class="sxs-lookup"><span data-stu-id="5739b-122">generateDownloadUri</span></span>](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[<span data-ttu-id="5739b-123">accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="5739b-123">accessReviewHistoryDefinition</span></span>](accessreviewhistorydefinition.md)|<span data-ttu-id="5739b-124">生成可用于检索审阅历史记录数据的 URI。</span><span class="sxs-lookup"><span data-stu-id="5739b-124">Generate a URI that can be used to retrieve review history data.</span></span>|

## <a name="properties"></a><span data-ttu-id="5739b-125">属性</span><span class="sxs-lookup"><span data-stu-id="5739b-125">Properties</span></span>
|<span data-ttu-id="5739b-126">属性</span><span class="sxs-lookup"><span data-stu-id="5739b-126">Property</span></span>|<span data-ttu-id="5739b-127">类型</span><span class="sxs-lookup"><span data-stu-id="5739b-127">Type</span></span>|<span data-ttu-id="5739b-128">说明</span><span class="sxs-lookup"><span data-stu-id="5739b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5739b-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="5739b-129">createdBy</span></span>|[<span data-ttu-id="5739b-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5739b-130">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="5739b-131">创建此审阅历史记录定义的用户。</span><span class="sxs-lookup"><span data-stu-id="5739b-131">User who created this review history definition.</span></span> |
|<span data-ttu-id="5739b-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5739b-132">createdDateTime</span></span>|<span data-ttu-id="5739b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5739b-133">DateTimeOffset</span></span>|<span data-ttu-id="5739b-134">创建访问评审定义的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5739b-134">Timestamp when the access review definition was created.</span></span>|
|<span data-ttu-id="5739b-135">决策</span><span class="sxs-lookup"><span data-stu-id="5739b-135">decisions</span></span>|<span data-ttu-id="5739b-136">String collection</span><span class="sxs-lookup"><span data-stu-id="5739b-136">String collection</span></span>|<span data-ttu-id="5739b-137">确定提取的审阅历史记录数据中将包含哪些审阅决策（如果已指定）。</span><span class="sxs-lookup"><span data-stu-id="5739b-137">Determines which review decisions will be included in the fetched review history data if specified.</span></span> <span data-ttu-id="5739b-138">创建时可选。</span><span class="sxs-lookup"><span data-stu-id="5739b-138">Optional on create.</span></span> <span data-ttu-id="5739b-139">如果未提供创建决策，则默认情况下将包含所有决策。</span><span class="sxs-lookup"><span data-stu-id="5739b-139">All decisions will be included by default if no decisions are provided on create.</span></span> <span data-ttu-id="5739b-140">可能的值是 `approve` `deny` `dontKnow` ：、、、 `notReviewed` 和 `notNotified` 。</span><span class="sxs-lookup"><span data-stu-id="5739b-140">Possible values are: `approve`, `deny`, `dontKnow`, `notReviewed`, and `notNotified`.</span></span>|
|<span data-ttu-id="5739b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5739b-141">displayName</span></span>|<span data-ttu-id="5739b-142">String</span><span class="sxs-lookup"><span data-stu-id="5739b-142">String</span></span>|<span data-ttu-id="5739b-143">访问评审历史记录数据收集的名称。</span><span class="sxs-lookup"><span data-stu-id="5739b-143">Name for the access review history data collection.</span></span> <span data-ttu-id="5739b-144">必需。</span><span class="sxs-lookup"><span data-stu-id="5739b-144">Required.</span></span>|
|<span data-ttu-id="5739b-145">downloadUri</span><span class="sxs-lookup"><span data-stu-id="5739b-145">downloadUri</span></span>|<span data-ttu-id="5739b-146">String</span><span class="sxs-lookup"><span data-stu-id="5739b-146">String</span></span>|<span data-ttu-id="5739b-147">可用于检索审阅历史记录数据的 Uri。</span><span class="sxs-lookup"><span data-stu-id="5739b-147">Uri which can be used to retrieve review history data.</span></span> <span data-ttu-id="5739b-148">生成后，此 URI 将处于活动状态 24 小时。</span><span class="sxs-lookup"><span data-stu-id="5739b-148">This URI will be active for 24 hours after being generated.</span></span>|
|<span data-ttu-id="5739b-149">fulfilledDateTime</span><span class="sxs-lookup"><span data-stu-id="5739b-149">fulfilledDateTime</span></span>|<span data-ttu-id="5739b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5739b-150">DateTimeOffset</span></span>|<span data-ttu-id="5739b-151">收集此定义的所有可用数据的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5739b-151">Timestamp when all of the available data for this definition was collected.</span></span> <span data-ttu-id="5739b-152">This will be set after this definition's status is set to `done` .</span><span class="sxs-lookup"><span data-stu-id="5739b-152">This will be set after this definition's status is set to `done`.</span></span>|
|<span data-ttu-id="5739b-153">id</span><span class="sxs-lookup"><span data-stu-id="5739b-153">id</span></span>|<span data-ttu-id="5739b-154">String</span><span class="sxs-lookup"><span data-stu-id="5739b-154">String</span></span>|<span data-ttu-id="5739b-155">为访问评审历史记录定义分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5739b-155">The assigned unique identifier of an access review history definition.</span></span>|
|<span data-ttu-id="5739b-156">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="5739b-156">reviewHistoryPeriodEndDateTime</span></span>|<span data-ttu-id="5739b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5739b-157">DateTimeOffset</span></span>|<span data-ttu-id="5739b-158">时间戳、在此日期当天或之后开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="5739b-158">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="5739b-159">必需。</span><span class="sxs-lookup"><span data-stu-id="5739b-159">Required.</span></span>|
|<span data-ttu-id="5739b-160">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="5739b-160">reviewHistoryPeriodStartDateTime</span></span>|<span data-ttu-id="5739b-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5739b-161">DateTimeOffset</span></span>|<span data-ttu-id="5739b-162">时间戳、在此日期或之前开始审阅将包含在提取的历史记录数据中。</span><span class="sxs-lookup"><span data-stu-id="5739b-162">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="5739b-163">必需。</span><span class="sxs-lookup"><span data-stu-id="5739b-163">Required.</span></span>|
|<span data-ttu-id="5739b-164">scopes</span><span class="sxs-lookup"><span data-stu-id="5739b-164">scopes</span></span>|<span data-ttu-id="5739b-165">microsoft.graph.accessReviewQueryScope 集合</span><span class="sxs-lookup"><span data-stu-id="5739b-165">microsoft.graph.accessReviewQueryScope collection</span></span>|<span data-ttu-id="5739b-166">用于确定提取的历史记录数据中包含的审阅的范围。</span><span class="sxs-lookup"><span data-stu-id="5739b-166">Used to scope what reviews are included in the fetched history data.</span></span> <span data-ttu-id="5739b-167">获取其范围与提供的范围匹配的审阅。</span><span class="sxs-lookup"><span data-stu-id="5739b-167">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="5739b-168">请参阅 [accessreviewqueryscope](accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="5739b-168">See [accessreviewqueryscope](accessreviewqueryscope.md).</span></span> <span data-ttu-id="5739b-169">必需。</span><span class="sxs-lookup"><span data-stu-id="5739b-169">Required.</span></span>|
|<span data-ttu-id="5739b-170">状态</span><span class="sxs-lookup"><span data-stu-id="5739b-170">status</span></span>|<span data-ttu-id="5739b-171">String collection</span><span class="sxs-lookup"><span data-stu-id="5739b-171">String collection</span></span>|<span data-ttu-id="5739b-172">表示审阅历史记录数据收集的状态。</span><span class="sxs-lookup"><span data-stu-id="5739b-172">Represents the status of the review history data collection.</span></span> <span data-ttu-id="5739b-173">可取值为：`done`、`inprogress`、`error`、`requested`。</span><span class="sxs-lookup"><span data-stu-id="5739b-173">Possible values are: `done`, `inprogress`, `error`, `requested`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5739b-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5739b-174">JSON representation</span></span>
<span data-ttu-id="5739b-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5739b-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
