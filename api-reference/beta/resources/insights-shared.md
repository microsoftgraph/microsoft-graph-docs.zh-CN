---
title: 共享的资源类型
description: 表示文件共享或特定用户洞察。 支持以下共享的文件：
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2c3d91023e2d68704b54308dff9566673f71dfb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973704"
---
# <a name="shared-resource-type"></a><span data-ttu-id="08372-104">共享的资源类型</span><span class="sxs-lookup"><span data-stu-id="08372-104">shared resource type</span></span>

> <span data-ttu-id="08372-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="08372-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08372-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="08372-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08372-107">表示文件共享或特定用户洞察。</span><span class="sxs-lookup"><span data-stu-id="08372-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="08372-108">支持以下共享的文件：</span><span class="sxs-lookup"><span data-stu-id="08372-108">The following shared files are supported:</span></span>

- <span data-ttu-id="08372-109">邀请电子邮件或会议中的直接附加文件。</span><span class="sxs-lookup"><span data-stu-id="08372-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="08372-110">业务和 SharePoint 的现代附件的文件存储在 OneDrive 中的业务和电子邮件中作为链接共享用户的 SharePoint OneDrive。</span><span class="sxs-lookup"><span data-stu-id="08372-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="08372-111">**注意**： 我们当前正在填充数据的共享 api 的结果。</span><span class="sxs-lookup"><span data-stu-id="08372-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="08372-112">可能在发布后第一周中缺少一些数据。</span><span class="sxs-lookup"><span data-stu-id="08372-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="08372-113">方法</span><span class="sxs-lookup"><span data-stu-id="08372-113">Methods</span></span>

| <span data-ttu-id="08372-114">方法</span><span class="sxs-lookup"><span data-stu-id="08372-114">Method</span></span>       | <span data-ttu-id="08372-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="08372-115">Return Type</span></span>  |<span data-ttu-id="08372-116">说明</span><span class="sxs-lookup"><span data-stu-id="08372-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08372-117">共享列表</span><span class="sxs-lookup"><span data-stu-id="08372-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="08372-118">[insights_shared](insights-shared.md)集合</span><span class="sxs-lookup"><span data-stu-id="08372-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="08372-119">获取共享文件的列表。</span><span class="sxs-lookup"><span data-stu-id="08372-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="08372-120">属性</span><span class="sxs-lookup"><span data-stu-id="08372-120">Properties</span></span>

| <span data-ttu-id="08372-121">属性</span><span class="sxs-lookup"><span data-stu-id="08372-121">Property</span></span>              | <span data-ttu-id="08372-122">类型</span><span class="sxs-lookup"><span data-stu-id="08372-122">Type</span></span>                      | <span data-ttu-id="08372-123">说明</span><span class="sxs-lookup"><span data-stu-id="08372-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="08372-124">id</span><span class="sxs-lookup"><span data-stu-id="08372-124">id</span></span>                    | <span data-ttu-id="08372-125">字符串</span><span class="sxs-lookup"><span data-stu-id="08372-125">String</span></span>                    | <span data-ttu-id="08372-126">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08372-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="08372-127">只读。</span><span class="sxs-lookup"><span data-stu-id="08372-127">Read only.</span></span>        |
| <span data-ttu-id="08372-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="08372-128">lastShared</span></span>            | [<span data-ttu-id="08372-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="08372-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="08372-130">有关共享项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="08372-130">Details about the shared item.</span></span> <span data-ttu-id="08372-131">只读。</span><span class="sxs-lookup"><span data-stu-id="08372-131">Read only.</span></span>        |
| <span data-ttu-id="08372-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="08372-132">resourceVisualization</span></span> | [<span data-ttu-id="08372-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="08372-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="08372-134">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="08372-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="08372-135">只读</span><span class="sxs-lookup"><span data-stu-id="08372-135">Read-only</span></span>      |
| <span data-ttu-id="08372-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="08372-136">resourceReference</span></span>     | [<span data-ttu-id="08372-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="08372-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="08372-138">引用的共享文档，如 url 和类型的文档属性。</span><span class="sxs-lookup"><span data-stu-id="08372-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="08372-139">只读</span><span class="sxs-lookup"><span data-stu-id="08372-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="08372-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="08372-140">Relationships</span></span>

| <span data-ttu-id="08372-141">属性</span><span class="sxs-lookup"><span data-stu-id="08372-141">Property</span></span>      | <span data-ttu-id="08372-142">类型</span><span class="sxs-lookup"><span data-stu-id="08372-142">Type</span></span>          | <span data-ttu-id="08372-143">说明</span><span class="sxs-lookup"><span data-stu-id="08372-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="08372-144">资源</span><span class="sxs-lookup"><span data-stu-id="08372-144">resource</span></span>      | <span data-ttu-id="08372-145">Entity</span><span class="sxs-lookup"><span data-stu-id="08372-145">Entity</span></span>        | <span data-ttu-id="08372-146">用于导航到共享的项目。</span><span class="sxs-lookup"><span data-stu-id="08372-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="08372-147">文件附件的类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="08372-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="08372-148">对于链接附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="08372-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08372-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08372-149">JSON representation</span></span>
<span data-ttu-id="08372-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08372-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
