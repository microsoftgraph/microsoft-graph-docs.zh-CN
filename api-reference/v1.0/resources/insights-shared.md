---
title: sharedInsight 资源类型
description: 了解表示与用户共享的文件或由特定用户共享的文件。 支持以下共享文件：
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c78ef6c63d1970f92a2a68a91cd674d39cbce736
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054810"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="5a51c-104">sharedInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a51c-104">sharedInsight resource type</span></span>

<span data-ttu-id="5a51c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a51c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a51c-106">了解表示与用户共享的文件或由特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="5a51c-106">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="5a51c-107">支持以下共享文件：</span><span class="sxs-lookup"><span data-stu-id="5a51c-107">The following shared files are supported:</span></span>

- <span data-ttu-id="5a51c-108">直接在电子邮件或会议邀请中附加的文件。</span><span class="sxs-lookup"><span data-stu-id="5a51c-108">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="5a51c-109">OneDrive for Business 和 SharePoint 新式附件-存储在 OneDrive for Business 和 SharePoint 中且用户共享为电子邮件中的链接的文件。</span><span class="sxs-lookup"><span data-stu-id="5a51c-109">OneDrive for Business and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="5a51c-110">**注意**：我们目前正在努力使用数据填充共享 API 的结果。</span><span class="sxs-lookup"><span data-stu-id="5a51c-110">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="5a51c-111">发布后的第一周可能缺少一些数据。</span><span class="sxs-lookup"><span data-stu-id="5a51c-111">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="5a51c-112">方法</span><span class="sxs-lookup"><span data-stu-id="5a51c-112">Methods</span></span>

| <span data-ttu-id="5a51c-113">方法</span><span class="sxs-lookup"><span data-stu-id="5a51c-113">Method</span></span>       | <span data-ttu-id="5a51c-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a51c-114">Return Type</span></span>  |<span data-ttu-id="5a51c-115">说明</span><span class="sxs-lookup"><span data-stu-id="5a51c-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a51c-116">共享的列表</span><span class="sxs-lookup"><span data-stu-id="5a51c-116">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="5a51c-117">[sharedInsight](insights-shared.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a51c-117">[sharedInsight](insights-shared.md) collection</span></span>| <span data-ttu-id="5a51c-118">获取共享文件的列表。</span><span class="sxs-lookup"><span data-stu-id="5a51c-118">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a51c-119">属性</span><span class="sxs-lookup"><span data-stu-id="5a51c-119">Properties</span></span>

| <span data-ttu-id="5a51c-120">属性</span><span class="sxs-lookup"><span data-stu-id="5a51c-120">Property</span></span>              | <span data-ttu-id="5a51c-121">类型</span><span class="sxs-lookup"><span data-stu-id="5a51c-121">Type</span></span>                      | <span data-ttu-id="5a51c-122">说明</span><span class="sxs-lookup"><span data-stu-id="5a51c-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="5a51c-123">id</span><span class="sxs-lookup"><span data-stu-id="5a51c-123">id</span></span>                    | <span data-ttu-id="5a51c-124">String</span><span class="sxs-lookup"><span data-stu-id="5a51c-124">String</span></span>                    | <span data-ttu-id="5a51c-125">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5a51c-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="5a51c-126">只读。</span><span class="sxs-lookup"><span data-stu-id="5a51c-126">Read only.</span></span>        |
| <span data-ttu-id="5a51c-127">lastShared</span><span class="sxs-lookup"><span data-stu-id="5a51c-127">lastShared</span></span>            | [<span data-ttu-id="5a51c-128">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="5a51c-128">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="5a51c-129">共享项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5a51c-129">Details about the shared item.</span></span> <span data-ttu-id="5a51c-130">只读。</span><span class="sxs-lookup"><span data-stu-id="5a51c-130">Read only.</span></span>        |
| <span data-ttu-id="5a51c-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5a51c-131">resourceVisualization</span></span> | [<span data-ttu-id="5a51c-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5a51c-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="5a51c-133">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="5a51c-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="5a51c-134">只读</span><span class="sxs-lookup"><span data-stu-id="5a51c-134">Read-only</span></span>      |
| <span data-ttu-id="5a51c-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5a51c-135">resourceReference</span></span>     | [<span data-ttu-id="5a51c-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5a51c-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="5a51c-137">引用共享文档的属性，例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="5a51c-137">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="5a51c-138">只读</span><span class="sxs-lookup"><span data-stu-id="5a51c-138">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="5a51c-139">关系</span><span class="sxs-lookup"><span data-stu-id="5a51c-139">Relationships</span></span>

| <span data-ttu-id="5a51c-140">属性</span><span class="sxs-lookup"><span data-stu-id="5a51c-140">Property</span></span>      | <span data-ttu-id="5a51c-141">类型</span><span class="sxs-lookup"><span data-stu-id="5a51c-141">Type</span></span>          | <span data-ttu-id="5a51c-142">说明</span><span class="sxs-lookup"><span data-stu-id="5a51c-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="5a51c-143">资源</span><span class="sxs-lookup"><span data-stu-id="5a51c-143">resource</span></span>      | <span data-ttu-id="5a51c-144">实体集合</span><span class="sxs-lookup"><span data-stu-id="5a51c-144">entity collection</span></span> | <span data-ttu-id="5a51c-145">用于导航到已共享的项目。</span><span class="sxs-lookup"><span data-stu-id="5a51c-145">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="5a51c-146">对于文件附件，类型为 *fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="5a51c-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="5a51c-147">对于链接的附件，类型为 *driveItem*。</span><span class="sxs-lookup"><span data-stu-id="5a51c-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a51c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a51c-148">JSON representation</span></span>
<span data-ttu-id="5a51c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a51c-149">Here is a JSON representation of the resource</span></span>
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```

