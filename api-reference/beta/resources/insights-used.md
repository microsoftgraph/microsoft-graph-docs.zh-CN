---
title: usedInsight 资源类型
description: 表示特定用户所使用的文档洞察。 见解返回最相关的文档的用户查看或访问。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 056654a5e467e202b2bde5ac8ee98dccab93d7c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574227"
---
# <a name="used-resource-type"></a><span data-ttu-id="295f5-104">使用资源类型</span><span class="sxs-lookup"><span data-stu-id="295f5-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295f5-105">表示特定用户所使用的文档洞察。</span><span class="sxs-lookup"><span data-stu-id="295f5-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="295f5-106">见解返回最相关的文档的用户查看或访问。</span><span class="sxs-lookup"><span data-stu-id="295f5-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="295f5-107">这包括文档中的文档：</span><span class="sxs-lookup"><span data-stu-id="295f5-107">This includes documents in:</span></span>

- <span data-ttu-id="295f5-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="295f5-108">OneDrive for Business</span></span>
- <span data-ttu-id="295f5-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="295f5-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="295f5-110">方法</span><span class="sxs-lookup"><span data-stu-id="295f5-110">Methods</span></span>

| <span data-ttu-id="295f5-111">方法</span><span class="sxs-lookup"><span data-stu-id="295f5-111">Method</span></span>       | <span data-ttu-id="295f5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="295f5-112">Return Type</span></span>  |<span data-ttu-id="295f5-113">说明</span><span class="sxs-lookup"><span data-stu-id="295f5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="295f5-114">使用列表</span><span class="sxs-lookup"><span data-stu-id="295f5-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="295f5-115">[insights_used](insights-used.md)集合</span><span class="sxs-lookup"><span data-stu-id="295f5-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="295f5-116">获取使用过的文件列表。</span><span class="sxs-lookup"><span data-stu-id="295f5-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="295f5-117">属性</span><span class="sxs-lookup"><span data-stu-id="295f5-117">Properties</span></span>

| <span data-ttu-id="295f5-118">属性</span><span class="sxs-lookup"><span data-stu-id="295f5-118">Property</span></span>              | <span data-ttu-id="295f5-119">类型</span><span class="sxs-lookup"><span data-stu-id="295f5-119">Type</span></span>                      | <span data-ttu-id="295f5-120">说明</span><span class="sxs-lookup"><span data-stu-id="295f5-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="295f5-121">id</span><span class="sxs-lookup"><span data-stu-id="295f5-121">id</span></span>                    | <span data-ttu-id="295f5-122">String</span><span class="sxs-lookup"><span data-stu-id="295f5-122">String</span></span>                    | <span data-ttu-id="295f5-123">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="295f5-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="295f5-124">只读。</span><span class="sxs-lookup"><span data-stu-id="295f5-124">Read only.</span></span>        |
| <span data-ttu-id="295f5-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="295f5-125">lastUsed</span></span>              | [<span data-ttu-id="295f5-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="295f5-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="295f5-127">有关项目时上次查看和修改的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="295f5-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="295f5-128">只读。</span><span class="sxs-lookup"><span data-stu-id="295f5-128">Read only.</span></span>     |
| <span data-ttu-id="295f5-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="295f5-129">resourceVisualization</span></span> | [<span data-ttu-id="295f5-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="295f5-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="295f5-131">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="295f5-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="295f5-132">只读</span><span class="sxs-lookup"><span data-stu-id="295f5-132">Read-only</span></span>      |
| <span data-ttu-id="295f5-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="295f5-133">resourceReference</span></span>     | [<span data-ttu-id="295f5-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="295f5-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="295f5-135">使用文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="295f5-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="295f5-136">只读</span><span class="sxs-lookup"><span data-stu-id="295f5-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="295f5-137">关系</span><span class="sxs-lookup"><span data-stu-id="295f5-137">Relationships</span></span>

| <span data-ttu-id="295f5-138">属性</span><span class="sxs-lookup"><span data-stu-id="295f5-138">Property</span></span>      | <span data-ttu-id="295f5-139">类型</span><span class="sxs-lookup"><span data-stu-id="295f5-139">Type</span></span>          | <span data-ttu-id="295f5-140">说明</span><span class="sxs-lookup"><span data-stu-id="295f5-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="295f5-141">资源</span><span class="sxs-lookup"><span data-stu-id="295f5-141">resource</span></span>      | <span data-ttu-id="295f5-142">实体集合</span><span class="sxs-lookup"><span data-stu-id="295f5-142">entity collection</span></span> | <span data-ttu-id="295f5-143">用于导航到已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="295f5-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="295f5-144">文件附件的类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="295f5-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="295f5-145">对于链接附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="295f5-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="295f5-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="295f5-146">JSON representation</span></span>
<span data-ttu-id="295f5-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="295f5-147">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->
```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
