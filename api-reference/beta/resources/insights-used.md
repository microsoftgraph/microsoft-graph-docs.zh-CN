---
title: 使用资源类型
description: 表示特定用户所使用的文档洞察。 见解返回最相关的文档的用户查看或访问。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: cb41fcb7cef5c9e39f9100ebd1d8c2640f06e2d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885531"
---
# <a name="used-resource-type"></a><span data-ttu-id="bf46e-104">使用资源类型</span><span class="sxs-lookup"><span data-stu-id="bf46e-104">used resource type</span></span>

> <span data-ttu-id="bf46e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf46e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf46e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf46e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf46e-107">表示特定用户所使用的文档洞察。</span><span class="sxs-lookup"><span data-stu-id="bf46e-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="bf46e-108">见解返回最相关的文档的用户查看或访问。</span><span class="sxs-lookup"><span data-stu-id="bf46e-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="bf46e-109">这包括文档中的文档：</span><span class="sxs-lookup"><span data-stu-id="bf46e-109">This includes documents in:</span></span>

- <span data-ttu-id="bf46e-110">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="bf46e-110">OneDrive for Business</span></span>
- <span data-ttu-id="bf46e-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="bf46e-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="bf46e-112">方法</span><span class="sxs-lookup"><span data-stu-id="bf46e-112">Methods</span></span>

| <span data-ttu-id="bf46e-113">方法</span><span class="sxs-lookup"><span data-stu-id="bf46e-113">Method</span></span>       | <span data-ttu-id="bf46e-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf46e-114">Return Type</span></span>  |<span data-ttu-id="bf46e-115">说明</span><span class="sxs-lookup"><span data-stu-id="bf46e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf46e-116">使用列表</span><span class="sxs-lookup"><span data-stu-id="bf46e-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="bf46e-117">[insights_used](insights-used.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf46e-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="bf46e-118">获取使用过的文件列表。</span><span class="sxs-lookup"><span data-stu-id="bf46e-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf46e-119">属性</span><span class="sxs-lookup"><span data-stu-id="bf46e-119">Properties</span></span>

| <span data-ttu-id="bf46e-120">属性</span><span class="sxs-lookup"><span data-stu-id="bf46e-120">Property</span></span>              | <span data-ttu-id="bf46e-121">类型</span><span class="sxs-lookup"><span data-stu-id="bf46e-121">Type</span></span>                      | <span data-ttu-id="bf46e-122">说明</span><span class="sxs-lookup"><span data-stu-id="bf46e-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="bf46e-123">id</span><span class="sxs-lookup"><span data-stu-id="bf46e-123">id</span></span>                    | <span data-ttu-id="bf46e-124">字符串</span><span class="sxs-lookup"><span data-stu-id="bf46e-124">String</span></span>                    | <span data-ttu-id="bf46e-125">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bf46e-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="bf46e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="bf46e-126">Read only.</span></span>        |
| <span data-ttu-id="bf46e-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="bf46e-127">lastUsed</span></span>              | [<span data-ttu-id="bf46e-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="bf46e-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="bf46e-129">有关项目时上次查看和修改的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="bf46e-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="bf46e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="bf46e-130">Read only.</span></span>     |
| <span data-ttu-id="bf46e-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="bf46e-131">resourceVisualization</span></span> | [<span data-ttu-id="bf46e-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="bf46e-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="bf46e-133">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="bf46e-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="bf46e-134">只读</span><span class="sxs-lookup"><span data-stu-id="bf46e-134">Read-only</span></span>      |
| <span data-ttu-id="bf46e-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="bf46e-135">resourceReference</span></span>     | [<span data-ttu-id="bf46e-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="bf46e-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="bf46e-137">使用文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="bf46e-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="bf46e-138">只读</span><span class="sxs-lookup"><span data-stu-id="bf46e-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="bf46e-139">Relationships</span><span class="sxs-lookup"><span data-stu-id="bf46e-139">Relationships</span></span>

| <span data-ttu-id="bf46e-140">属性</span><span class="sxs-lookup"><span data-stu-id="bf46e-140">Property</span></span>      | <span data-ttu-id="bf46e-141">类型</span><span class="sxs-lookup"><span data-stu-id="bf46e-141">Type</span></span>          | <span data-ttu-id="bf46e-142">说明</span><span class="sxs-lookup"><span data-stu-id="bf46e-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="bf46e-143">资源</span><span class="sxs-lookup"><span data-stu-id="bf46e-143">resource</span></span>      | <span data-ttu-id="bf46e-144">Entity</span><span class="sxs-lookup"><span data-stu-id="bf46e-144">Entity</span></span>        | <span data-ttu-id="bf46e-145">用于导航到已使用的项目。</span><span class="sxs-lookup"><span data-stu-id="bf46e-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="bf46e-146">文件附件的类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="bf46e-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="bf46e-147">对于链接附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="bf46e-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bf46e-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf46e-148">JSON representation</span></span>
<span data-ttu-id="bf46e-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf46e-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
