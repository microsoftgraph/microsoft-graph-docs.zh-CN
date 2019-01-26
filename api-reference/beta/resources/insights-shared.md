---
title: 共享的资源类型
description: 表示文件共享或特定用户洞察。 支持以下共享的文件：
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49e18318c1e93d2393b957b404ff4617b334f237
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573177"
---
# <a name="shared-resource-type"></a><span data-ttu-id="51f4c-104">共享的资源类型</span><span class="sxs-lookup"><span data-stu-id="51f4c-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f4c-105">表示文件共享或特定用户洞察。</span><span class="sxs-lookup"><span data-stu-id="51f4c-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="51f4c-106">支持以下共享的文件：</span><span class="sxs-lookup"><span data-stu-id="51f4c-106">The following shared files are supported:</span></span>

- <span data-ttu-id="51f4c-107">邀请电子邮件或会议中的直接附加文件。</span><span class="sxs-lookup"><span data-stu-id="51f4c-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="51f4c-108">业务和 SharePoint 的现代附件的文件存储在 OneDrive 中的业务和电子邮件中作为链接共享用户的 SharePoint OneDrive。</span><span class="sxs-lookup"><span data-stu-id="51f4c-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="51f4c-109">**注意**： 我们当前正在填充数据的共享 api 的结果。</span><span class="sxs-lookup"><span data-stu-id="51f4c-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="51f4c-110">可能在发布后第一周中缺少一些数据。</span><span class="sxs-lookup"><span data-stu-id="51f4c-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="51f4c-111">方法</span><span class="sxs-lookup"><span data-stu-id="51f4c-111">Methods</span></span>

| <span data-ttu-id="51f4c-112">方法</span><span class="sxs-lookup"><span data-stu-id="51f4c-112">Method</span></span>       | <span data-ttu-id="51f4c-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="51f4c-113">Return Type</span></span>  |<span data-ttu-id="51f4c-114">说明</span><span class="sxs-lookup"><span data-stu-id="51f4c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51f4c-115">共享列表</span><span class="sxs-lookup"><span data-stu-id="51f4c-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="51f4c-116">[insights_shared](insights-shared.md)集合</span><span class="sxs-lookup"><span data-stu-id="51f4c-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="51f4c-117">获取共享文件的列表。</span><span class="sxs-lookup"><span data-stu-id="51f4c-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="51f4c-118">属性</span><span class="sxs-lookup"><span data-stu-id="51f4c-118">Properties</span></span>

| <span data-ttu-id="51f4c-119">属性</span><span class="sxs-lookup"><span data-stu-id="51f4c-119">Property</span></span>              | <span data-ttu-id="51f4c-120">类型</span><span class="sxs-lookup"><span data-stu-id="51f4c-120">Type</span></span>                      | <span data-ttu-id="51f4c-121">说明</span><span class="sxs-lookup"><span data-stu-id="51f4c-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="51f4c-122">id</span><span class="sxs-lookup"><span data-stu-id="51f4c-122">id</span></span>                    | <span data-ttu-id="51f4c-123">String</span><span class="sxs-lookup"><span data-stu-id="51f4c-123">String</span></span>                    | <span data-ttu-id="51f4c-124">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="51f4c-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="51f4c-125">只读。</span><span class="sxs-lookup"><span data-stu-id="51f4c-125">Read only.</span></span>        |
| <span data-ttu-id="51f4c-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="51f4c-126">lastShared</span></span>            | [<span data-ttu-id="51f4c-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="51f4c-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="51f4c-128">有关共享项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="51f4c-128">Details about the shared item.</span></span> <span data-ttu-id="51f4c-129">只读。</span><span class="sxs-lookup"><span data-stu-id="51f4c-129">Read only.</span></span>        |
| <span data-ttu-id="51f4c-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="51f4c-130">resourceVisualization</span></span> | [<span data-ttu-id="51f4c-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="51f4c-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="51f4c-132">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="51f4c-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="51f4c-133">只读</span><span class="sxs-lookup"><span data-stu-id="51f4c-133">Read-only</span></span>      |
| <span data-ttu-id="51f4c-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="51f4c-134">resourceReference</span></span>     | [<span data-ttu-id="51f4c-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="51f4c-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="51f4c-136">引用的共享文档，如 url 和类型的文档属性。</span><span class="sxs-lookup"><span data-stu-id="51f4c-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="51f4c-137">只读</span><span class="sxs-lookup"><span data-stu-id="51f4c-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="51f4c-138">关系</span><span class="sxs-lookup"><span data-stu-id="51f4c-138">Relationships</span></span>

| <span data-ttu-id="51f4c-139">属性</span><span class="sxs-lookup"><span data-stu-id="51f4c-139">Property</span></span>      | <span data-ttu-id="51f4c-140">类型</span><span class="sxs-lookup"><span data-stu-id="51f4c-140">Type</span></span>          | <span data-ttu-id="51f4c-141">说明</span><span class="sxs-lookup"><span data-stu-id="51f4c-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="51f4c-142">资源</span><span class="sxs-lookup"><span data-stu-id="51f4c-142">resource</span></span>      | <span data-ttu-id="51f4c-143">实体集合</span><span class="sxs-lookup"><span data-stu-id="51f4c-143">entity collection</span></span> | <span data-ttu-id="51f4c-144">用于导航到共享的项目。</span><span class="sxs-lookup"><span data-stu-id="51f4c-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="51f4c-145">文件附件的类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="51f4c-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="51f4c-146">对于链接附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="51f4c-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51f4c-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51f4c-147">JSON representation</span></span>
<span data-ttu-id="51f4c-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51f4c-148">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shared"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
