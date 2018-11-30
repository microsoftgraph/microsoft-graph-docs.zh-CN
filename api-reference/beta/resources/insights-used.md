---
title: 使用资源类型
description: 表示特定用户所使用的文档洞察。 见解返回最相关的文档的用户查看或访问。 这包括文档中的文档：
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047325"
---
# <a name="used-resource-type"></a><span data-ttu-id="95763-105">使用资源类型</span><span class="sxs-lookup"><span data-stu-id="95763-105">used resource type</span></span>

> <span data-ttu-id="95763-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95763-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95763-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95763-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95763-108">表示特定用户所使用的文档洞察。</span><span class="sxs-lookup"><span data-stu-id="95763-108">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="95763-109">见解返回最相关的文档的用户查看或访问。</span><span class="sxs-lookup"><span data-stu-id="95763-109">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="95763-110">这包括文档中的文档：</span><span class="sxs-lookup"><span data-stu-id="95763-110">This includes documents in:</span></span>

- <span data-ttu-id="95763-111">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="95763-111">OneDrive for Business</span></span>
- <span data-ttu-id="95763-112">SharePoint</span><span class="sxs-lookup"><span data-stu-id="95763-112">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="95763-113">方法</span><span class="sxs-lookup"><span data-stu-id="95763-113">Methods</span></span>

| <span data-ttu-id="95763-114">方法</span><span class="sxs-lookup"><span data-stu-id="95763-114">Method</span></span>       | <span data-ttu-id="95763-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="95763-115">Return Type</span></span>  |<span data-ttu-id="95763-116">说明</span><span class="sxs-lookup"><span data-stu-id="95763-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95763-117">使用列表</span><span class="sxs-lookup"><span data-stu-id="95763-117">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="95763-118">[insights_used](insights-used.md)集合</span><span class="sxs-lookup"><span data-stu-id="95763-118">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="95763-119">获取使用过的文件列表。</span><span class="sxs-lookup"><span data-stu-id="95763-119">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="95763-120">属性</span><span class="sxs-lookup"><span data-stu-id="95763-120">Properties</span></span>

| <span data-ttu-id="95763-121">属性</span><span class="sxs-lookup"><span data-stu-id="95763-121">Property</span></span>              | <span data-ttu-id="95763-122">类型</span><span class="sxs-lookup"><span data-stu-id="95763-122">Type</span></span>                      | <span data-ttu-id="95763-123">说明</span><span class="sxs-lookup"><span data-stu-id="95763-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="95763-124">id</span><span class="sxs-lookup"><span data-stu-id="95763-124">id</span></span>                    | <span data-ttu-id="95763-125">字符串</span><span class="sxs-lookup"><span data-stu-id="95763-125">String</span></span>                    | <span data-ttu-id="95763-126">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="95763-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="95763-127">只读。</span><span class="sxs-lookup"><span data-stu-id="95763-127">Read only.</span></span>        |
| <span data-ttu-id="95763-128">lastUsed</span><span class="sxs-lookup"><span data-stu-id="95763-128">lastUsed</span></span>              | [<span data-ttu-id="95763-129">usageDetails</span><span class="sxs-lookup"><span data-stu-id="95763-129">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="95763-130">有关项目时上次查看和修改的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="95763-130">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="95763-131">只读。</span><span class="sxs-lookup"><span data-stu-id="95763-131">Read only.</span></span>     |
| <span data-ttu-id="95763-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="95763-132">resourceVisualization</span></span> | [<span data-ttu-id="95763-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="95763-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="95763-134">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="95763-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="95763-135">只读</span><span class="sxs-lookup"><span data-stu-id="95763-135">Read-only</span></span>      |
| <span data-ttu-id="95763-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="95763-136">resourceReference</span></span>     | [<span data-ttu-id="95763-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="95763-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="95763-138">使用文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="95763-138">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="95763-139">只读</span><span class="sxs-lookup"><span data-stu-id="95763-139">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="95763-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="95763-140">Relationships</span></span>

| <span data-ttu-id="95763-141">属性</span><span class="sxs-lookup"><span data-stu-id="95763-141">Property</span></span>      | <span data-ttu-id="95763-142">类型</span><span class="sxs-lookup"><span data-stu-id="95763-142">Type</span></span>          | <span data-ttu-id="95763-143">说明</span><span class="sxs-lookup"><span data-stu-id="95763-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="95763-144">资源</span><span class="sxs-lookup"><span data-stu-id="95763-144">resource</span></span>      | <span data-ttu-id="95763-145">实体</span><span class="sxs-lookup"><span data-stu-id="95763-145">Entity</span></span>        | <span data-ttu-id="95763-146">用于导航到已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="95763-146">Used for navigating to the item that was used.</span></span> <span data-ttu-id="95763-147">文件附件的类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="95763-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="95763-148">对于链接附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="95763-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95763-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95763-149">JSON representation</span></span>
<span data-ttu-id="95763-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95763-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```