---
title: 使用的资源类型
description: 表示特定用户使用的文档的洞察力。 该见解将返回用户查看或访问的最相关的文档。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551287"
---
# <a name="used-resource-type"></a><span data-ttu-id="97044-104">使用的资源类型</span><span class="sxs-lookup"><span data-stu-id="97044-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97044-105">表示特定用户使用的文档的洞察力。</span><span class="sxs-lookup"><span data-stu-id="97044-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="97044-106">该见解将返回用户查看或访问的最相关的文档。</span><span class="sxs-lookup"><span data-stu-id="97044-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="97044-107">其中包括以下文档:</span><span class="sxs-lookup"><span data-stu-id="97044-107">This includes documents in:</span></span>

- <span data-ttu-id="97044-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="97044-108">OneDrive for Business</span></span>
- <span data-ttu-id="97044-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="97044-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="97044-110">方法</span><span class="sxs-lookup"><span data-stu-id="97044-110">Methods</span></span>

| <span data-ttu-id="97044-111">方法</span><span class="sxs-lookup"><span data-stu-id="97044-111">Method</span></span>       | <span data-ttu-id="97044-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="97044-112">Return Type</span></span>  |<span data-ttu-id="97044-113">说明</span><span class="sxs-lookup"><span data-stu-id="97044-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97044-114">使用的列表</span><span class="sxs-lookup"><span data-stu-id="97044-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="97044-115">[insights_used](insights-used.md)集合</span><span class="sxs-lookup"><span data-stu-id="97044-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="97044-116">获取已用文件的列表。</span><span class="sxs-lookup"><span data-stu-id="97044-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="97044-117">属性</span><span class="sxs-lookup"><span data-stu-id="97044-117">Properties</span></span>

| <span data-ttu-id="97044-118">属性</span><span class="sxs-lookup"><span data-stu-id="97044-118">Property</span></span>              | <span data-ttu-id="97044-119">类型</span><span class="sxs-lookup"><span data-stu-id="97044-119">Type</span></span>                      | <span data-ttu-id="97044-120">说明</span><span class="sxs-lookup"><span data-stu-id="97044-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="97044-121">id</span><span class="sxs-lookup"><span data-stu-id="97044-121">id</span></span>                    | <span data-ttu-id="97044-122">String</span><span class="sxs-lookup"><span data-stu-id="97044-122">String</span></span>                    | <span data-ttu-id="97044-123">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="97044-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="97044-124">只读。</span><span class="sxs-lookup"><span data-stu-id="97044-124">Read only.</span></span>        |
| <span data-ttu-id="97044-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="97044-125">lastUsed</span></span>              | [<span data-ttu-id="97044-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="97044-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="97044-127">有关用户上次查看和修改项目的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="97044-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="97044-128">只读。</span><span class="sxs-lookup"><span data-stu-id="97044-128">Read only.</span></span>     |
| <span data-ttu-id="97044-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="97044-129">resourceVisualization</span></span> | [<span data-ttu-id="97044-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="97044-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="97044-131">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="97044-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="97044-132">只读</span><span class="sxs-lookup"><span data-stu-id="97044-132">Read-only</span></span>      |
| <span data-ttu-id="97044-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="97044-133">resourceReference</span></span>     | [<span data-ttu-id="97044-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="97044-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="97044-135">所用文档的引用属性, 例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="97044-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="97044-136">只读</span><span class="sxs-lookup"><span data-stu-id="97044-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="97044-137">关系</span><span class="sxs-lookup"><span data-stu-id="97044-137">Relationships</span></span>

| <span data-ttu-id="97044-138">属性</span><span class="sxs-lookup"><span data-stu-id="97044-138">Property</span></span>      | <span data-ttu-id="97044-139">类型</span><span class="sxs-lookup"><span data-stu-id="97044-139">Type</span></span>          | <span data-ttu-id="97044-140">说明</span><span class="sxs-lookup"><span data-stu-id="97044-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="97044-141">资源</span><span class="sxs-lookup"><span data-stu-id="97044-141">resource</span></span>      | <span data-ttu-id="97044-142">实体</span><span class="sxs-lookup"><span data-stu-id="97044-142">Entity</span></span>        | <span data-ttu-id="97044-143">用于导航到所使用的项目。</span><span class="sxs-lookup"><span data-stu-id="97044-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="97044-144">对于文件附件, 类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="97044-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="97044-145">对于链接的附件, 类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="97044-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97044-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97044-146">JSON representation</span></span>
<span data-ttu-id="97044-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97044-147">Here is a JSON representation of the resource</span></span>

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
