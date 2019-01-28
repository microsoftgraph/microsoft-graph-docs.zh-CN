---
title: insights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513688"
---
# <a name="insights-resource-type"></a><span data-ttu-id="e71cc-104">insights 资源类型</span><span class="sxs-lookup"><span data-stu-id="e71cc-104">insights resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71cc-105">Insights 是使用高级分析和机器学习技术计算的关系。</span><span class="sxs-lookup"><span data-stu-id="e71cc-105">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="e71cc-106">例如，你可以标识与用户有关的 OneDrive 文档趋势。</span><span class="sxs-lookup"><span data-stu-id="e71cc-106">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="e71cc-107">Insights 由以下 API 返回：</span><span class="sxs-lookup"><span data-stu-id="e71cc-107">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="e71cc-108">[Trending](insights-trending.md) - 返回与用户有关的 OneDrive 和 SharePoint 网站趋势文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-108">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="e71cc-109">[Used](insights-used.md) - 返回用户查看和修改过的文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-109">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="e71cc-110">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-110">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="e71cc-111">[Shared](insights-shared.md) - 返回与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-111">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="e71cc-112">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-112">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="e71cc-113">返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="e71cc-113">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="e71cc-114">resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。</span><span class="sxs-lookup"><span data-stu-id="e71cc-114">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="e71cc-115">Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="e71cc-115">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="e71cc-116">关系</span><span class="sxs-lookup"><span data-stu-id="e71cc-116">Relationships</span></span>

| <span data-ttu-id="e71cc-117">关系</span><span class="sxs-lookup"><span data-stu-id="e71cc-117">Relationship</span></span>      | <span data-ttu-id="e71cc-118">类型</span><span class="sxs-lookup"><span data-stu-id="e71cc-118">Type</span></span>          | <span data-ttu-id="e71cc-119">说明</span><span class="sxs-lookup"><span data-stu-id="e71cc-119">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="e71cc-120">趋势</span><span class="sxs-lookup"><span data-stu-id="e71cc-120">trending</span></span>      | <span data-ttu-id="e71cc-121">[Trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e71cc-121">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="e71cc-122">用于标识趋势文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="e71cc-122">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="e71cc-123">趋势文档可以存储在 OneDrive 或 SharePoint 网站中。</span><span class="sxs-lookup"><span data-stu-id="e71cc-123">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="e71cc-124">使用的内容</span><span class="sxs-lookup"><span data-stu-id="e71cc-124">used</span></span>      | <span data-ttu-id="e71cc-125">[Used](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e71cc-125">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="e71cc-126">用于标识用户已查看和修改文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="e71cc-126">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="e71cc-127">包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-127">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="e71cc-128">共享的内容</span><span class="sxs-lookup"><span data-stu-id="e71cc-128">shared</span></span>        | <span data-ttu-id="e71cc-129">[Shared](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e71cc-129">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="e71cc-130">用于标识与用户共享的文档的计算关系。</span><span class="sxs-lookup"><span data-stu-id="e71cc-130">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="e71cc-131">可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。</span><span class="sxs-lookup"><span data-stu-id="e71cc-131">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="e71cc-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e71cc-132">JSON representation</span></span>

<span data-ttu-id="e71cc-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e71cc-133">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
