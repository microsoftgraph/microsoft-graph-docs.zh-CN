---
title: officeGraphInsights 资源类型
description: 表示 itemInsights 的基本类型。 officeGraphInsights 向后兼容 insights API 的早期版本。 访问 insights API 时只能使用 itemInsights。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ce1f51a3e0b53dc1ed108febf9a3b91055349ce5
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427324"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="fe46d-105">officeGraphInsights 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe46d-105">officeGraphInsights resource type</span></span>

<span data-ttu-id="fe46d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe46d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe46d-107">使用 [itemInsights](iteminsights.md) 替代 **officeGraphInsights** 以访问 insights API。</span><span class="sxs-lookup"><span data-stu-id="fe46d-107">Use [itemInsights](iteminsights.md) in place of **officeGraphInsights** to access the insights API.</span></span>

<span data-ttu-id="fe46d-108">**officeGraphInsights** 向后兼容 insights API 的早期版本。</span><span class="sxs-lookup"><span data-stu-id="fe46d-108">**officeGraphInsights** is for backward compatibility from earlier versions of the insights API.</span></span> <span data-ttu-id="fe46d-109">它是 [itemInsights](iteminsights.md) 的基础类型。</span><span class="sxs-lookup"><span data-stu-id="fe46d-109">It is the base type for [itemInsights](iteminsights.md).</span></span>

<span data-ttu-id="fe46d-110">Insights 是使用高级分析和机器学习技术计算的关系。</span><span class="sxs-lookup"><span data-stu-id="fe46d-110">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="fe46d-111">例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="fe46d-111">You can, for example, identify OneDrive for Business documents trending around users.</span></span>

<span data-ttu-id="fe46d-112">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="fe46d-112">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="fe46d-113">[趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="fe46d-113">[Trending](insights-trending.md) - returns documents from OneDrive for Business and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="fe46d-114">[使用](insights-used.md) - 返回用户查看或修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="fe46d-114">[Used](insights-used.md) - returns documents viewed or modified by a user.</span></span> <span data-ttu-id="fe46d-115">包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。</span><span class="sxs-lookup"><span data-stu-id="fe46d-115">Includes documents the user used in OneDrive for Business, and SharePoint.</span></span>
- <span data-ttu-id="fe46d-116">[分享](insights-shared.md) - 返回与用户共享或由用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="fe46d-116">[Shared](insights-shared.md) - returns documents shared with or by the user.</span></span> <span data-ttu-id="fe46d-117">文档可以作为 OneDrive for Business 和 SharePoint 的 URL、文件附件、参考附件共享，这些可以在 Outlook 邮件和会议中找到。</span><span class="sxs-lookup"><span data-stu-id="fe46d-117">Documents can be shared as URLs, file attachments, reference attachments to OneDrive for Business and SharePoint files found in Outlook messages and meetings.</span></span>

<span data-ttu-id="fe46d-118">每个见解都返回 **resourceVisualization** 和 **resourceReference** 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="fe46d-118">Each insight is returned with a **resourceVisualization** and **resourceReference** complex value type (CVT).</span></span> <span data-ttu-id="fe46d-119">**resourceVisualization** CVT 包含诸如 **title** 和 **previewImageUrl** 之类的属性。</span><span class="sxs-lookup"><span data-stu-id="fe46d-119">The **resourceVisualization** CVT contains properties such as **title** and **previewImageUrl**.</span></span> <span data-ttu-id="fe46d-120">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="fe46d-120">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="fe46d-121">关系</span><span class="sxs-lookup"><span data-stu-id="fe46d-121">Relationships</span></span>

| <span data-ttu-id="fe46d-122">关系</span><span class="sxs-lookup"><span data-stu-id="fe46d-122">Relationship</span></span>      | <span data-ttu-id="fe46d-123">类型</span><span class="sxs-lookup"><span data-stu-id="fe46d-123">Type</span></span>          | <span data-ttu-id="fe46d-124">说明</span><span class="sxs-lookup"><span data-stu-id="fe46d-124">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="fe46d-125">趋势</span><span class="sxs-lookup"><span data-stu-id="fe46d-125">trending</span></span>      | <span data-ttu-id="fe46d-126">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe46d-126">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="fe46d-127">从派生类型 [itemInsights](iteminsights.md) 访问此属性。</span><span class="sxs-lookup"><span data-stu-id="fe46d-127">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="fe46d-128">使用的内容</span><span class="sxs-lookup"><span data-stu-id="fe46d-128">used</span></span>      | <span data-ttu-id="fe46d-129">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe46d-129">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="fe46d-130">从派生类型 [itemInsights](iteminsights.md) 访问此属性。</span><span class="sxs-lookup"><span data-stu-id="fe46d-130">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|
| <span data-ttu-id="fe46d-131">shared</span><span class="sxs-lookup"><span data-stu-id="fe46d-131">shared</span></span>        | <span data-ttu-id="fe46d-132">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe46d-132">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="fe46d-133">从派生类型 [itemInsights](iteminsights.md) 访问此属性。</span><span class="sxs-lookup"><span data-stu-id="fe46d-133">Access this property from the derived type [itemInsights](iteminsights.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fe46d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe46d-134">JSON representation</span></span>

<span data-ttu-id="fe46d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe46d-135">Here is a JSON representation of the resource</span></span>
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

