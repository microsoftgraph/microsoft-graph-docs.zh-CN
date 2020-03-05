---
title: officeGraphInsights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8ac5019909a2f5ebe808be695ed7d516738c21e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447337"
---
# <a name="officegraphinsights-resource-type"></a><span data-ttu-id="5839d-104">officeGraphInsights 资源类型</span><span class="sxs-lookup"><span data-stu-id="5839d-104">officeGraphInsights resource type</span></span>

<span data-ttu-id="5839d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5839d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5839d-106">Insights 是使用高级分析和机器学习技术计算的关系。</span><span class="sxs-lookup"><span data-stu-id="5839d-106">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="5839d-107">例如，你可以标识与用户有关的 OneDrive 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="5839d-107">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="5839d-108">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="5839d-108">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="5839d-109">[Trending](insights-trending.md) - 返回与用户有关的 OneDrive 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-109">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="5839d-110">[Used](insights-used.md) - 返回用户查看和修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-110">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="5839d-111">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-111">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="5839d-112">[Shared](insights-shared.md) - 返回与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-112">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="5839d-113">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-113">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="5839d-114">返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="5839d-114">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="5839d-115">resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。</span><span class="sxs-lookup"><span data-stu-id="5839d-115">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="5839d-116">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="5839d-116">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="5839d-117">关系</span><span class="sxs-lookup"><span data-stu-id="5839d-117">Relationships</span></span>

| <span data-ttu-id="5839d-118">关系</span><span class="sxs-lookup"><span data-stu-id="5839d-118">Relationship</span></span>      | <span data-ttu-id="5839d-119">类型</span><span class="sxs-lookup"><span data-stu-id="5839d-119">Type</span></span>          | <span data-ttu-id="5839d-120">说明</span><span class="sxs-lookup"><span data-stu-id="5839d-120">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="5839d-121">趋势</span><span class="sxs-lookup"><span data-stu-id="5839d-121">trending</span></span>      | <span data-ttu-id="5839d-122">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5839d-122">[trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="5839d-123">用于标识趋势文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="5839d-123">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="5839d-124">趋势文档可以存储在 OneDrive 或 SharePoint 网站中。</span><span class="sxs-lookup"><span data-stu-id="5839d-124">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="5839d-125">使用的内容</span><span class="sxs-lookup"><span data-stu-id="5839d-125">used</span></span>      | <span data-ttu-id="5839d-126">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5839d-126">[usedInsight](insights-used.md) collection</span></span>        | <span data-ttu-id="5839d-127">用于标识用户已查看和修改文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="5839d-127">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="5839d-128">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-128">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="5839d-129">shared</span><span class="sxs-lookup"><span data-stu-id="5839d-129">shared</span></span>        | <span data-ttu-id="5839d-130">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5839d-130">[sharedInsight](insights-shared.md) collection</span></span>        | <span data-ttu-id="5839d-131">用于标识与用户共享的文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="5839d-131">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="5839d-132">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="5839d-132">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="5839d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5839d-133">JSON representation</span></span>

<span data-ttu-id="5839d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5839d-134">Here is a JSON representation of the resource</span></span>
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
