---
title: 见解资源类型
description: 见解是计算使用高级分析功能和机学习技术的关系。 例如，可以确定趋势周围用户的 OneDrive 文档。
author: simonhult
ms.openlocfilehash: f3269134f4a80462359a11d603c3f843be0c62f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318597"
---
# <a name="insights-resource-type"></a><span data-ttu-id="5a4ea-104">见解资源类型</span><span class="sxs-lookup"><span data-stu-id="5a4ea-104">insights resource type</span></span>

> <span data-ttu-id="5a4ea-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a4ea-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a4ea-107">见解是计算使用高级分析功能和机学习技术的关系。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-107">Insights are relationships calculated using advanced analytics and machine learning techniques.</span></span> <span data-ttu-id="5a4ea-108">例如，可以确定趋势周围用户的 OneDrive 文档。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-108">You can, for example, identify OneDrive documents trending around users.</span></span>

<span data-ttu-id="5a4ea-109">见解会返回以下 Api:</span><span class="sxs-lookup"><span data-stu-id="5a4ea-109">Insights are returned by the following APIs:</span></span>

- <span data-ttu-id="5a4ea-110">[趋势](insights-trending.md)-返回文档从 OneDrive 和趋势周围用户的 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-110">[Trending](insights-trending.md) - returns documents from OneDrive and from SharePoint sites trending around a user.</span></span>
- <span data-ttu-id="5a4ea-111">[用于](insights-used.md)-返回文档查看和修改的用户。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-111">[Used](insights-used.md) - returns documents viewed and modified by a user.</span></span> <span data-ttu-id="5a4ea-112">包含用户使用的文档中的 OneDrive for Business，SharePoint 中，打开作为电子邮件附件和为如框、 收存箱和 Google 驱动器的源中的链接附件。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-112">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>
- <span data-ttu-id="5a4ea-113">[共享](insights-shared.md)-返回与用户共享的文档。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-113">[Shared](insights-shared.md) - returns documents shared with a user.</span></span> <span data-ttu-id="5a4ea-114">文档可以共享作为电子邮件附件或 OneDrive for Business 链接中发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-114">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>

<span data-ttu-id="5a4ea-115">每个洞察返回了`resourceVisualization`和`resourceReference`复杂值类型 (CVT)。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-115">Each insight is returned with a `resourceVisualization` and `resourceReference` complex value type (CVT).</span></span> <span data-ttu-id="5a4ea-116">ResourceVisualization CVT 包含属性，如`title`和`previewImageUrl`。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-116">The resourceVisualization CVT contains properties such as `title` and `previewImageUrl`.</span></span> <span data-ttu-id="5a4ea-117">Microsoft 使用可视化属性来呈现像 Office 深入体验中的文件。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-117">Microsoft uses the visualization properties to render the files in experiences like Office Delve.</span></span>

## <a name="relationships"></a><span data-ttu-id="5a4ea-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="5a4ea-118">Relationships</span></span>

| <span data-ttu-id="5a4ea-119">关系</span><span class="sxs-lookup"><span data-stu-id="5a4ea-119">Relationship</span></span>      | <span data-ttu-id="5a4ea-120">类型</span><span class="sxs-lookup"><span data-stu-id="5a4ea-120">Type</span></span>          | <span data-ttu-id="5a4ea-121">说明</span><span class="sxs-lookup"><span data-stu-id="5a4ea-121">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="5a4ea-122">趋势分析</span><span class="sxs-lookup"><span data-stu-id="5a4ea-122">trending</span></span>      | <span data-ttu-id="5a4ea-123">[趋势](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a4ea-123">[Trending](insights-trending.md) collection</span></span>       | <span data-ttu-id="5a4ea-124">确定趋势文档的关系计算。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-124">Calculated relationship identifying trending documents.</span></span> <span data-ttu-id="5a4ea-125">可以存储趋势文档，在 OneDrive 或 SharePoint 网站中。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-125">Trending documents can be stored in OneDrive or in SharePoint sites.</span></span>   |
| <span data-ttu-id="5a4ea-126">used</span><span class="sxs-lookup"><span data-stu-id="5a4ea-126">used</span></span>      | <span data-ttu-id="5a4ea-127">[用于](insights-used.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a4ea-127">[Used](insights-used.md) collection</span></span>       | <span data-ttu-id="5a4ea-128">计算确定文档查看和修改的用户的关系。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-128">Calculated relationship identifying documents viewed and modified by a user.</span></span> <span data-ttu-id="5a4ea-129">包含用户使用的文档中的 OneDrive for Business，SharePoint 中，打开作为电子邮件附件和为如框、 收存箱和 Google 驱动器的源中的链接附件。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-129">Includes documents the user used in OneDrive for Business, SharePoint, opened as email attachments, and as link attachments from sources like Box, DropBox and Google Drive.</span></span>  |
| <span data-ttu-id="5a4ea-130">shared</span><span class="sxs-lookup"><span data-stu-id="5a4ea-130">shared</span></span>        | <span data-ttu-id="5a4ea-131">[共享](insights-shared.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a4ea-131">[Shared](insights-shared.md) collection</span></span>       | <span data-ttu-id="5a4ea-132">确定与用户共享的文档的关系计算。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-132">Calculated relationship identifying documents shared with a user.</span></span> <span data-ttu-id="5a4ea-133">文档可以共享作为电子邮件附件或 OneDrive for Business 链接中发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-133">Documents can be shared as email attachments or as OneDrive for Business links sent in emails.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="5a4ea-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a4ea-134">JSON representation</span></span>

<span data-ttu-id="5a4ea-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a4ea-135">Here is a JSON representation of the resource</span></span>
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```