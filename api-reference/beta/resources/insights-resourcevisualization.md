---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 7eddc083bd38c0902f61d326926c86f48ca78714
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620905"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="b449e-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="b449e-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b449e-104">包含[见解](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="b449e-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b449e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b449e-105">JSON representation</span></span>

<span data-ttu-id="b449e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b449e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b449e-107">属性</span><span class="sxs-lookup"><span data-stu-id="b449e-107">Properties</span></span>

| <span data-ttu-id="b449e-108">属性</span><span class="sxs-lookup"><span data-stu-id="b449e-108">Property</span></span>              | <span data-ttu-id="b449e-109">类型</span><span class="sxs-lookup"><span data-stu-id="b449e-109">Type</span></span>          | <span data-ttu-id="b449e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b449e-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="b449e-111">title</span><span class="sxs-lookup"><span data-stu-id="b449e-111">title</span></span>                 | <span data-ttu-id="b449e-112">String</span><span class="sxs-lookup"><span data-stu-id="b449e-112">String</span></span>        | <span data-ttu-id="b449e-113">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="b449e-113">The item's title text.</span></span>               |
| <span data-ttu-id="b449e-114">type</span><span class="sxs-lookup"><span data-stu-id="b449e-114">type</span></span>              | <span data-ttu-id="b449e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="b449e-115">String</span></span>        | <span data-ttu-id="b449e-116">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="b449e-116">The item's media type.</span></span> <span data-ttu-id="b449e-117">可用于根据特定类型筛选特定文件。</span><span class="sxs-lookup"><span data-stu-id="b449e-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="b449e-118">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="b449e-118">See below for supported types.</span></span> |
| <span data-ttu-id="b449e-119">群组</span><span class="sxs-lookup"><span data-stu-id="b449e-119">mediaType</span></span>             | <span data-ttu-id="b449e-120">String</span><span class="sxs-lookup"><span data-stu-id="b449e-120">String</span></span>        | <span data-ttu-id="b449e-121">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="b449e-121">The item's media type.</span></span> <span data-ttu-id="b449e-122">可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。</span><span class="sxs-lookup"><span data-stu-id="b449e-122">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="b449e-123">请注意, 并非所有媒体 Mime 类型都受支持。</span><span class="sxs-lookup"><span data-stu-id="b449e-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="b449e-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="b449e-124">previewImageUrl</span></span>       | <span data-ttu-id="b449e-125">String</span><span class="sxs-lookup"><span data-stu-id="b449e-125">String</span></span>        | <span data-ttu-id="b449e-126">指向项目的预览图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="b449e-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="b449e-127">previewText</span><span class="sxs-lookup"><span data-stu-id="b449e-127">previewText</span></span>           | <span data-ttu-id="b449e-128">String</span><span class="sxs-lookup"><span data-stu-id="b449e-128">String</span></span>        | <span data-ttu-id="b449e-129">项目的预览文本。</span><span class="sxs-lookup"><span data-stu-id="b449e-129">A preview text for the item.</span></span> |
| <span data-ttu-id="b449e-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="b449e-130">containerWebUrl</span></span>       | <span data-ttu-id="b449e-131">String</span><span class="sxs-lookup"><span data-stu-id="b449e-131">String</span></span>        | <span data-ttu-id="b449e-132">指向存储项目的文件夹的路径。</span><span class="sxs-lookup"><span data-stu-id="b449e-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="b449e-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="b449e-133">containerDisplayName</span></span>  | <span data-ttu-id="b449e-134">String</span><span class="sxs-lookup"><span data-stu-id="b449e-134">String</span></span>        | <span data-ttu-id="b449e-135">一个描述项目存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="b449e-135">A string describing where the item is stored.</span></span> <span data-ttu-id="b449e-136">例如, SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。</span><span class="sxs-lookup"><span data-stu-id="b449e-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="b449e-137">containerType</span><span class="sxs-lookup"><span data-stu-id="b449e-137">containerType</span></span>         | <span data-ttu-id="b449e-138">String</span><span class="sxs-lookup"><span data-stu-id="b449e-138">String</span></span> | <span data-ttu-id="b449e-139">可用于按存储文件的容器的类型进行筛选。</span><span class="sxs-lookup"><span data-stu-id="b449e-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="b449e-140">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="b449e-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="b449e-141">类型属性值</span><span class="sxs-lookup"><span data-stu-id="b449e-141">Type property values</span></span>
-   <span data-ttu-id="b449e-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="b449e-142">PowerPoint</span></span>
-   <span data-ttu-id="b449e-143">Word</span><span class="sxs-lookup"><span data-stu-id="b449e-143">Word</span></span>
-   <span data-ttu-id="b449e-144">Excel</span><span class="sxs-lookup"><span data-stu-id="b449e-144">Excel</span></span>
-   <span data-ttu-id="b449e-145">Pdf</span><span class="sxs-lookup"><span data-stu-id="b449e-145">Pdf</span></span>
-   <span data-ttu-id="b449e-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="b449e-146">OneNote</span></span>
-   <span data-ttu-id="b449e-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="b449e-147">OneNotePage</span></span>
-   <span data-ttu-id="b449e-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="b449e-148">InfoPath</span></span>
-   <span data-ttu-id="b449e-149">Visio</span><span class="sxs-lookup"><span data-stu-id="b449e-149">Visio</span></span>
-   <span data-ttu-id="b449e-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="b449e-150">Publisher</span></span>
-   <span data-ttu-id="b449e-151">Project</span><span class="sxs-lookup"><span data-stu-id="b449e-151">Project</span></span>
-   <span data-ttu-id="b449e-152">Access</span><span class="sxs-lookup"><span data-stu-id="b449e-152">Access</span></span>
-   <span data-ttu-id="b449e-153">邮件</span><span class="sxs-lookup"><span data-stu-id="b449e-153">Mail</span></span>
-   <span data-ttu-id="b449e-154">Csv</span><span class="sxs-lookup"><span data-stu-id="b449e-154">Csv</span></span>
-   <span data-ttu-id="b449e-155">存档</span><span class="sxs-lookup"><span data-stu-id="b449e-155">Archive</span></span>
-   <span data-ttu-id="b449e-156">Xps</span><span class="sxs-lookup"><span data-stu-id="b449e-156">Xps</span></span>
-   <span data-ttu-id="b449e-157">音频</span><span class="sxs-lookup"><span data-stu-id="b449e-157">Audio</span></span>
-   <span data-ttu-id="b449e-158">视频</span><span class="sxs-lookup"><span data-stu-id="b449e-158">Video</span></span>
-   <span data-ttu-id="b449e-159">图像</span><span class="sxs-lookup"><span data-stu-id="b449e-159">Image</span></span>
-   <span data-ttu-id="b449e-160">Web</span><span class="sxs-lookup"><span data-stu-id="b449e-160">Web</span></span>
-   <span data-ttu-id="b449e-161">文本</span><span class="sxs-lookup"><span data-stu-id="b449e-161">Text</span></span>
-   <span data-ttu-id="b449e-162">Xml</span><span class="sxs-lookup"><span data-stu-id="b449e-162">Xml</span></span>
-   <span data-ttu-id="b449e-163">Story</span><span class="sxs-lookup"><span data-stu-id="b449e-163">Story</span></span>
-   <span data-ttu-id="b449e-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="b449e-164">ExternalContent</span></span>
-   <span data-ttu-id="b449e-165">Folder</span><span class="sxs-lookup"><span data-stu-id="b449e-165">Folder</span></span>
-   <span data-ttu-id="b449e-166">Other</span><span class="sxs-lookup"><span data-stu-id="b449e-166">Other</span></span>

<span data-ttu-id="b449e-167">示例查询:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="b449e-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="b449e-168">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="b449e-168">containerType property values</span></span>
<span data-ttu-id="b449e-169">根据[officeGraphInsights](officegraphinsights.md)返回文件的容器, 受支持的类型可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="b449e-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="b449e-170">例如, 仅[sharedInsight](insights-shared.md)真知灼见将从 "收存箱"、"Box" 和 "GDrive" 返回文件。</span><span class="sxs-lookup"><span data-stu-id="b449e-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="b449e-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="b449e-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="b449e-172">Site</span><span class="sxs-lookup"><span data-stu-id="b449e-172">Site</span></span>
-   <span data-ttu-id="b449e-173">邮件</span><span class="sxs-lookup"><span data-stu-id="b449e-173">Mail</span></span>
-   <span data-ttu-id="b449e-174">箱</span><span class="sxs-lookup"><span data-stu-id="b449e-174">DropBox</span></span>
-   <span data-ttu-id="b449e-175">Box</span><span class="sxs-lookup"><span data-stu-id="b449e-175">Box</span></span>
-   <span data-ttu-id="b449e-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="b449e-176">GDrive</span></span>

<span data-ttu-id="b449e-177">示例查询:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="b449e-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
