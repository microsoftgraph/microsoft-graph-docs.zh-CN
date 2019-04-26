---
title: sharedInsight 资源类型
description: '了解表示与用户共享的文件或由特定用户共享的文件。 支持以下共享文件:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 128a85bb9aa2e9f51d2393029cce3c27f8c4e6f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339977"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="927fb-104">sharedInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="927fb-104">sharedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="927fb-105">了解表示与用户共享的文件或由特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="927fb-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="927fb-106">支持以下共享文件:</span><span class="sxs-lookup"><span data-stu-id="927fb-106">The following shared files are supported:</span></span>

- <span data-ttu-id="927fb-107">直接在电子邮件或会议邀请中附加的文件。</span><span class="sxs-lookup"><span data-stu-id="927fb-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="927fb-108">onedrive for Bussiness and sharepoint 新式附件-存储在 OneDrive for business 和 sharepoint 中的文件, 用户共享为电子邮件中的链接。</span><span class="sxs-lookup"><span data-stu-id="927fb-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="927fb-109">**注意**: 我们目前正在努力使用数据填充共享 API 的结果。</span><span class="sxs-lookup"><span data-stu-id="927fb-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="927fb-110">发布后的第一周可能缺少一些数据。</span><span class="sxs-lookup"><span data-stu-id="927fb-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="927fb-111">方法</span><span class="sxs-lookup"><span data-stu-id="927fb-111">Methods</span></span>

| <span data-ttu-id="927fb-112">方法</span><span class="sxs-lookup"><span data-stu-id="927fb-112">Method</span></span>       | <span data-ttu-id="927fb-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="927fb-113">Return Type</span></span>  |<span data-ttu-id="927fb-114">说明</span><span class="sxs-lookup"><span data-stu-id="927fb-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="927fb-115">共享的列表</span><span class="sxs-lookup"><span data-stu-id="927fb-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="927fb-116">[insights_shared](insights-shared.md)集合</span><span class="sxs-lookup"><span data-stu-id="927fb-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="927fb-117">获取共享文件的列表。</span><span class="sxs-lookup"><span data-stu-id="927fb-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="927fb-118">属性</span><span class="sxs-lookup"><span data-stu-id="927fb-118">Properties</span></span>

| <span data-ttu-id="927fb-119">属性</span><span class="sxs-lookup"><span data-stu-id="927fb-119">Property</span></span>              | <span data-ttu-id="927fb-120">类型</span><span class="sxs-lookup"><span data-stu-id="927fb-120">Type</span></span>                      | <span data-ttu-id="927fb-121">说明</span><span class="sxs-lookup"><span data-stu-id="927fb-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="927fb-122">id</span><span class="sxs-lookup"><span data-stu-id="927fb-122">id</span></span>                    | <span data-ttu-id="927fb-123">String</span><span class="sxs-lookup"><span data-stu-id="927fb-123">String</span></span>                    | <span data-ttu-id="927fb-124">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="927fb-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="927fb-125">只读。</span><span class="sxs-lookup"><span data-stu-id="927fb-125">Read only.</span></span>        |
| <span data-ttu-id="927fb-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="927fb-126">lastShared</span></span>            | [<span data-ttu-id="927fb-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="927fb-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="927fb-128">共享项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="927fb-128">Details about the shared item.</span></span> <span data-ttu-id="927fb-129">只读。</span><span class="sxs-lookup"><span data-stu-id="927fb-129">Read only.</span></span>        |
| <span data-ttu-id="927fb-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="927fb-130">resourceVisualization</span></span> | [<span data-ttu-id="927fb-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="927fb-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="927fb-132">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="927fb-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="927fb-133">只读</span><span class="sxs-lookup"><span data-stu-id="927fb-133">Read-only</span></span>      |
| <span data-ttu-id="927fb-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="927fb-134">resourceReference</span></span>     | [<span data-ttu-id="927fb-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="927fb-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="927fb-136">引用共享文档的属性, 例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="927fb-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="927fb-137">只读</span><span class="sxs-lookup"><span data-stu-id="927fb-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="927fb-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="927fb-138">Relationships</span></span>

| <span data-ttu-id="927fb-139">属性</span><span class="sxs-lookup"><span data-stu-id="927fb-139">Property</span></span>      | <span data-ttu-id="927fb-140">类型</span><span class="sxs-lookup"><span data-stu-id="927fb-140">Type</span></span>          | <span data-ttu-id="927fb-141">说明</span><span class="sxs-lookup"><span data-stu-id="927fb-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="927fb-142">资源</span><span class="sxs-lookup"><span data-stu-id="927fb-142">resource</span></span>      | <span data-ttu-id="927fb-143">实体集合</span><span class="sxs-lookup"><span data-stu-id="927fb-143">entity collection</span></span> | <span data-ttu-id="927fb-144">用于导航到已共享的项目。</span><span class="sxs-lookup"><span data-stu-id="927fb-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="927fb-145">对于文件附件, 类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="927fb-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="927fb-146">对于链接的附件, 类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="927fb-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="927fb-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="927fb-147">JSON representation</span></span>
<span data-ttu-id="927fb-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="927fb-148">Here is a JSON representation of the resource</span></span>
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
