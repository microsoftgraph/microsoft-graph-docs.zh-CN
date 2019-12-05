---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 39810868e779f9de62535e4b463f477f12739e85
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39845019"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="17d1b-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="17d1b-103">resourceVisualization resource type</span></span>

<span data-ttu-id="17d1b-104">包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="17d1b-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="17d1b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17d1b-105">JSON representation</span></span>

<span data-ttu-id="17d1b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17d1b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="17d1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="17d1b-107">Properties</span></span>

| <span data-ttu-id="17d1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="17d1b-108">Property</span></span>              | <span data-ttu-id="17d1b-109">类型</span><span class="sxs-lookup"><span data-stu-id="17d1b-109">Type</span></span>          | <span data-ttu-id="17d1b-110">说明</span><span class="sxs-lookup"><span data-stu-id="17d1b-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="17d1b-111">title</span><span class="sxs-lookup"><span data-stu-id="17d1b-111">title</span></span>                 | <span data-ttu-id="17d1b-112">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-112">String</span></span>        | <span data-ttu-id="17d1b-113">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="17d1b-113">The item's title text.</span></span>               |
| <span data-ttu-id="17d1b-114">type</span><span class="sxs-lookup"><span data-stu-id="17d1b-114">type</span></span>              | <span data-ttu-id="17d1b-115">字符串</span><span class="sxs-lookup"><span data-stu-id="17d1b-115">String</span></span>        | <span data-ttu-id="17d1b-116">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="17d1b-116">The item's media type.</span></span> <span data-ttu-id="17d1b-117">可用于根据特定类型筛选特定文件。</span><span class="sxs-lookup"><span data-stu-id="17d1b-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="17d1b-118">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="17d1b-118">See below for supported types.</span></span> |
| <span data-ttu-id="17d1b-119">群组</span><span class="sxs-lookup"><span data-stu-id="17d1b-119">mediaType</span></span>             | <span data-ttu-id="17d1b-120">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-120">String</span></span>        | <span data-ttu-id="17d1b-121">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="17d1b-121">The item's media type.</span></span> <span data-ttu-id="17d1b-122">可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。</span><span class="sxs-lookup"><span data-stu-id="17d1b-122">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="17d1b-123">请注意，并非所有媒体 Mime 类型都受支持。</span><span class="sxs-lookup"><span data-stu-id="17d1b-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="17d1b-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="17d1b-124">previewImageUrl</span></span>       | <span data-ttu-id="17d1b-125">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-125">String</span></span>        | <span data-ttu-id="17d1b-126">指向项目的预览图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="17d1b-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="17d1b-127">previewText</span><span class="sxs-lookup"><span data-stu-id="17d1b-127">previewText</span></span>           | <span data-ttu-id="17d1b-128">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-128">String</span></span>        | <span data-ttu-id="17d1b-129">项目的预览文本。</span><span class="sxs-lookup"><span data-stu-id="17d1b-129">A preview text for the item.</span></span> |
| <span data-ttu-id="17d1b-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="17d1b-130">containerWebUrl</span></span>       | <span data-ttu-id="17d1b-131">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-131">String</span></span>        | <span data-ttu-id="17d1b-132">指向存储项目的文件夹的路径。</span><span class="sxs-lookup"><span data-stu-id="17d1b-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="17d1b-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="17d1b-133">containerDisplayName</span></span>  | <span data-ttu-id="17d1b-134">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-134">String</span></span>        | <span data-ttu-id="17d1b-135">一个描述项目存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="17d1b-135">A string describing where the item is stored.</span></span> <span data-ttu-id="17d1b-136">例如，SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。</span><span class="sxs-lookup"><span data-stu-id="17d1b-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="17d1b-137">containerType</span><span class="sxs-lookup"><span data-stu-id="17d1b-137">containerType</span></span>         | <span data-ttu-id="17d1b-138">String</span><span class="sxs-lookup"><span data-stu-id="17d1b-138">String</span></span> | <span data-ttu-id="17d1b-139">可用于按存储文件的容器的类型进行筛选。</span><span class="sxs-lookup"><span data-stu-id="17d1b-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="17d1b-140">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="17d1b-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="17d1b-141">类型属性值</span><span class="sxs-lookup"><span data-stu-id="17d1b-141">Type property values</span></span>
-   <span data-ttu-id="17d1b-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="17d1b-142">PowerPoint</span></span>
-   <span data-ttu-id="17d1b-143">Word</span><span class="sxs-lookup"><span data-stu-id="17d1b-143">Word</span></span>
-   <span data-ttu-id="17d1b-144">Excel</span><span class="sxs-lookup"><span data-stu-id="17d1b-144">Excel</span></span>
-   <span data-ttu-id="17d1b-145">Pdf</span><span class="sxs-lookup"><span data-stu-id="17d1b-145">Pdf</span></span>
-   <span data-ttu-id="17d1b-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="17d1b-146">OneNote</span></span>
-   <span data-ttu-id="17d1b-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="17d1b-147">OneNotePage</span></span>
-   <span data-ttu-id="17d1b-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="17d1b-148">InfoPath</span></span>
-   <span data-ttu-id="17d1b-149">Visio</span><span class="sxs-lookup"><span data-stu-id="17d1b-149">Visio</span></span>
-   <span data-ttu-id="17d1b-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="17d1b-150">Publisher</span></span>
-   <span data-ttu-id="17d1b-151">项目</span><span class="sxs-lookup"><span data-stu-id="17d1b-151">Project</span></span>
-   <span data-ttu-id="17d1b-152">Access</span><span class="sxs-lookup"><span data-stu-id="17d1b-152">Access</span></span>
-   <span data-ttu-id="17d1b-153">邮件</span><span class="sxs-lookup"><span data-stu-id="17d1b-153">Mail</span></span>
-   <span data-ttu-id="17d1b-154">Csv</span><span class="sxs-lookup"><span data-stu-id="17d1b-154">Csv</span></span>
-   <span data-ttu-id="17d1b-155">存档</span><span class="sxs-lookup"><span data-stu-id="17d1b-155">Archive</span></span>
-   <span data-ttu-id="17d1b-156">Xps</span><span class="sxs-lookup"><span data-stu-id="17d1b-156">Xps</span></span>
-   <span data-ttu-id="17d1b-157">音频</span><span class="sxs-lookup"><span data-stu-id="17d1b-157">Audio</span></span>
-   <span data-ttu-id="17d1b-158">视频</span><span class="sxs-lookup"><span data-stu-id="17d1b-158">Video</span></span>
-   <span data-ttu-id="17d1b-159">图像</span><span class="sxs-lookup"><span data-stu-id="17d1b-159">Image</span></span>
-   <span data-ttu-id="17d1b-160">Web</span><span class="sxs-lookup"><span data-stu-id="17d1b-160">Web</span></span>
-   <span data-ttu-id="17d1b-161">文本</span><span class="sxs-lookup"><span data-stu-id="17d1b-161">Text</span></span>
-   <span data-ttu-id="17d1b-162">Xml</span><span class="sxs-lookup"><span data-stu-id="17d1b-162">Xml</span></span>
-   <span data-ttu-id="17d1b-163">Story</span><span class="sxs-lookup"><span data-stu-id="17d1b-163">Story</span></span>
-   <span data-ttu-id="17d1b-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="17d1b-164">ExternalContent</span></span>
-   <span data-ttu-id="17d1b-165">Folder</span><span class="sxs-lookup"><span data-stu-id="17d1b-165">Folder</span></span>
-   <span data-ttu-id="17d1b-166">Other</span><span class="sxs-lookup"><span data-stu-id="17d1b-166">Other</span></span>

<span data-ttu-id="17d1b-167">示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="17d1b-167">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="17d1b-168">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="17d1b-168">containerType property values</span></span>
<span data-ttu-id="17d1b-169">根据[officeGraphInsights](officegraphinsights.md)返回文件的容器，受支持的类型可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="17d1b-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="17d1b-170">例如，仅[sharedInsight](insights-shared.md)真知灼见将从 "收存箱"、"Box" 和 "GDrive" 返回文件。</span><span class="sxs-lookup"><span data-stu-id="17d1b-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="17d1b-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="17d1b-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="17d1b-172">Site</span><span class="sxs-lookup"><span data-stu-id="17d1b-172">Site</span></span>
-   <span data-ttu-id="17d1b-173">邮件</span><span class="sxs-lookup"><span data-stu-id="17d1b-173">Mail</span></span>
-   <span data-ttu-id="17d1b-174">箱</span><span class="sxs-lookup"><span data-stu-id="17d1b-174">DropBox</span></span>
-   <span data-ttu-id="17d1b-175">Box</span><span class="sxs-lookup"><span data-stu-id="17d1b-175">Box</span></span>
-   <span data-ttu-id="17d1b-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="17d1b-176">GDrive</span></span>

<span data-ttu-id="17d1b-177">示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="17d1b-177">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
