---
title: itemInsights 资源类型
description: 用户与项目之间的关系，例如使用高级分析和机器学习技术计算得出的OneDrive for Business文档。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 36b0d8957beae9f8748c0e388a0aca2134731f73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089341"
---
# <a name="iteminsights-resource-type"></a><span data-ttu-id="1ba7d-104">itemInsights 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ba7d-104">itemInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba7d-105">用户与项目之间的关系，例如使用高级分析和机器学习技术计算得出的OneDrive for Business文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-105">Relationships between a user and items such as OneDrive for Business documents, calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="1ba7d-106">例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-106">You can, for example, identify OneDrive for Business documents trending around users.</span></span> <span data-ttu-id="1ba7d-107">派生自 [officeGraphInsights](officegraphinsights.md)。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-107">Derived from [officeGraphInsights](officegraphinsights.md).</span></span>

<span data-ttu-id="1ba7d-108">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="1ba7d-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="1ba7d-109">[趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="1ba7d-110">[Used](insights-used.md) - 返回用户查看和修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="1ba7d-111">包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="1ba7d-112">[Shared](insights-shared.md) - 返回与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="1ba7d-113">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="1ba7d-114">返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="1ba7d-115">resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="1ba7d-116">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

### <a name="limiting-item-insights"></a><span data-ttu-id="1ba7d-117">限制项目见解</span><span class="sxs-lookup"><span data-stu-id="1ba7d-117">Limiting item insights</span></span>

<span data-ttu-id="1ba7d-118">更新 [itemInsightsSettings](iteminsightssettings.md) 以禁用特定 Azure AD 组或整个组织的项目见解。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-118">Update [itemInsightsSettings](iteminsightssettings.md) to disable item insights for a specific Azure AD group or an entire organization.</span></span> <span data-ttu-id="1ba7d-119">有关详细信息，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-119">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).</span></span>

## <a name="relationships"></a><span data-ttu-id="1ba7d-120">关系</span><span class="sxs-lookup"><span data-stu-id="1ba7d-120">Relationships</span></span>

| <span data-ttu-id="1ba7d-121">关系</span><span class="sxs-lookup"><span data-stu-id="1ba7d-121">Relationship</span></span>      | <span data-ttu-id="1ba7d-122">类型</span><span class="sxs-lookup"><span data-stu-id="1ba7d-122">Type</span></span>          | <span data-ttu-id="1ba7d-123">说明</span><span class="sxs-lookup"><span data-stu-id="1ba7d-123">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="1ba7d-124">趋势</span><span class="sxs-lookup"><span data-stu-id="1ba7d-124">trending</span></span>      | <span data-ttu-id="1ba7d-125">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ba7d-125">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="1ba7d-126">用于标识与用户趋势文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-126">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="1ba7d-127">趋势文档是根据用户最近的人际网络活动来计算的，包括存储在 OneDrive for Business 和 SharePoint 的文件。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-127">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="1ba7d-128">趋势见解帮助用户发现可能有用的内容，这些内容用户有权访问，但之前从未看过。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-128">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="1ba7d-129">使用的内容</span><span class="sxs-lookup"><span data-stu-id="1ba7d-129">used</span></span>      | <span data-ttu-id="1ba7d-130">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ba7d-130">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="1ba7d-131">用于标识用户查看和修改的最新文档的计算关系，包括按使用时间排序的 OneDrive for Business 和 SharePoint 文档。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-131">Calculated relationship identifying the latest documents viewed and modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="1ba7d-132">shared</span><span class="sxs-lookup"><span data-stu-id="1ba7d-132">shared</span></span>        | <span data-ttu-id="1ba7d-133">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ba7d-133">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="1ba7d-134">用于识别与或用户共享的文档的计算关系，包括电子邮件和会议中的文件附件，以及在电子邮件、会议和团队对话中找到的 OneDrive for business 和 SharePoint 文件的 URL 和参考附件。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-134">Calculated relationship identifying documents shared with or by the user, includes file attachments in emails and meetings, as well as URLs and Reference attachments to OneDrive for Business and SharePoint files found in emails, meetings, and Teams conversations.</span></span> <span data-ttu-id="1ba7d-135">按共享时间排序。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-135">Ordered by recency of share.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1ba7d-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ba7d-136">JSON representation</span></span>

<span data-ttu-id="1ba7d-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ba7d-137">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```


