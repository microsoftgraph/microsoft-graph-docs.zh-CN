---
title: officeGraphInsights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 807cb786577b9c9ddd512d9dcce9a03517170f5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966501"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="c3e9a-104">officeGraphInsights 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3e9a-104">officeGraphInsights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e9a-105">Insights 是使用高级分析和机器学习技术计算的关系。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="c3e9a-106">例如，你可以标识与用户有关的 OneDrive 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="c3e9a-107">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="c3e9a-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="c3e9a-108">[Trending](insights-trending.md) - 返回与用户有关的 OneDrive 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="c3e9a-109">[Used](insights-used.md) - 返回用户查看和修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="c3e9a-110">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="c3e9a-111">[Shared](insights-shared.md) - 返回与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="c3e9a-112">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="c3e9a-113">返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="c3e9a-114">resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="c3e9a-115">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="c3e9a-116">关系</span><span class="sxs-lookup"><span data-stu-id="c3e9a-116">Relationships</span></span>

| <span data-ttu-id="c3e9a-117">关系</span><span class="sxs-lookup"><span data-stu-id="c3e9a-117">Relationship</span></span>      | <span data-ttu-id="c3e9a-118">类型</span><span class="sxs-lookup"><span data-stu-id="c3e9a-118">Type</span></span>          | <span data-ttu-id="c3e9a-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3e9a-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="c3e9a-120">趋势</span><span class="sxs-lookup"><span data-stu-id="c3e9a-120">trending</span></span>      | <span data-ttu-id="c3e9a-121">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3e9a-121">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="c3e9a-122">用于标识趋势文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="c3e9a-123">趋势文档可以存储在 OneDrive 或 SharePoint 网站中。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="c3e9a-124">使用的内容</span><span class="sxs-lookup"><span data-stu-id="c3e9a-124">used</span></span>      | <span data-ttu-id="c3e9a-125">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3e9a-125">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="c3e9a-126">用于标识用户已查看和修改文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="c3e9a-127">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="c3e9a-128">shared</span><span class="sxs-lookup"><span data-stu-id="c3e9a-128">shared</span></span>        | <span data-ttu-id="c3e9a-129">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3e9a-129">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="c3e9a-130">用于标识与用户共享的文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="c3e9a-131">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="c3e9a-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3e9a-132">JSON representation</span></span>

<span data-ttu-id="c3e9a-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3e9a-133">Here is a JSON representation of the resource</span></span>
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
