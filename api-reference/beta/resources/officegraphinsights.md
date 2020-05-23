---
title: officeGraphInsights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 266c570169c219259d19a6c1f78e01c83fe8e2c2
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226887"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="abe78-104">officeGraphInsights 资源类型</span><span class="sxs-lookup"><span data-stu-id="abe78-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="abe78-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe78-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe78-106">Insights 是使用高级分析和机器学习技术计算的关系。</span><span class="sxs-lookup"><span data-stu-id="abe78-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="abe78-107">例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="abe78-107">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="abe78-108">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="abe78-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="abe78-109">[趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="abe78-109">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="abe78-110">[使用](insights-used.md) - 返回用户查看或修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="abe78-110">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="abe78-111">包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。</span><span class="sxs-lookup"><span data-stu-id="abe78-111">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="abe78-112">[分享](insights-shared.md) - 返回与用户共享或用户分享的文档。</span><span class="sxs-lookup"><span data-stu-id="abe78-112">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="abe78-113">文档可以作为 OneDrive for Business 和 SharePoint 的 URL、文件附件、参考附件共享，这些可以在 Outlook 邮件和会议中找到。</span><span class="sxs-lookup"><span data-stu-id="abe78-113">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="abe78-114">每个见解都返回 **resourceVisualization** 和 **resourceReference** 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="abe78-114">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="abe78-115">**resourceVisualization** CVT 包含诸如 **title** 和 **previewImageUrl**之类的属性。</span><span class="sxs-lookup"><span data-stu-id="abe78-115">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="abe78-116">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="abe78-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="abe78-117">关系</span><span class="sxs-lookup"><span data-stu-id="abe78-117">Relationships</span></span>

| <span data-ttu-id="abe78-118">关系</span><span class="sxs-lookup"><span data-stu-id="abe78-118">Relationship</span></span>      | <span data-ttu-id="abe78-119">类型</span><span class="sxs-lookup"><span data-stu-id="abe78-119">Type</span></span>          | <span data-ttu-id="abe78-120">说明</span><span class="sxs-lookup"><span data-stu-id="abe78-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="abe78-121">趋势</span><span class="sxs-lookup"><span data-stu-id="abe78-121">trending</span></span>      | <span data-ttu-id="abe78-122">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abe78-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="abe78-123">用于标识与用户趋势文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="abe78-123">Calculated relationship identifying documents trending around a user.</span></span> <span data-ttu-id="abe78-124">趋势文档是根据用户最近的人际网络活动来计算的，包括存储在 OneDrive for Business 和 SharePoint 的文件。</span><span class="sxs-lookup"><span data-stu-id="abe78-124">Trending documents are calculated based on activity of the user's closest network of people and include files stored in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="abe78-125">趋势见解帮助用户发现可能有用的内容，这些内容用户有权访问，但之前从未看过。</span><span class="sxs-lookup"><span data-stu-id="abe78-125">Trending insights help the user to discover potentially useful content that the user has access to, but has never viewed before.</span></span>|
| <span data-ttu-id="abe78-126">使用的内容</span><span class="sxs-lookup"><span data-stu-id="abe78-126">used</span></span>      | <span data-ttu-id="abe78-127">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abe78-127">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="abe78-128">用于标识用户查看或修改的最新文档的计算关系，包括按使用时间排序的 OneDrive for Business 和 SharePoint 文档。</span><span class="sxs-lookup"><span data-stu-id="abe78-128">Calculated relationship identifying the latest documents viewed or modified by a user, including OneDrive for Business and SharePoint documents, ranked by recency of use.</span></span>|
| <span data-ttu-id="abe78-129">shared</span><span class="sxs-lookup"><span data-stu-id="abe78-129">shared</span></span>        | <span data-ttu-id="abe78-130">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abe78-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="abe78-131">用于标识与用户共享的或用户分享的文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="abe78-131">Calculated relationship identifying documents shared with or by the user.</span></span> <span data-ttu-id="abe78-132">这包括 OneDrive for Business 和 SharePoint 的 URL、文件附件、参考附件，这些可以在 Outlook 邮件和会议中找到。</span><span class="sxs-lookup"><span data-stu-id="abe78-132">This includes URLs, file attachments, and reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span> <span data-ttu-id="abe78-133">这还包括 Teams 对话的 URL 和引用附件。</span><span class="sxs-lookup"><span data-stu-id="abe78-133">This also includes URLs and reference attachments to Teams conversations.</span></span> <span data-ttu-id="abe78-134">按分享时间排序。</span><span class="sxs-lookup"><span data-stu-id="abe78-134">Ordered by recency of share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abe78-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abe78-135">JSON representation</span></span>

<span data-ttu-id="abe78-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abe78-136">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
