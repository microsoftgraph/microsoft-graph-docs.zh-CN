---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 876acf56d4f3445d55163a8c4cdb5bc1461c45de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531293"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="3c92a-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c92a-103">resourceVisualization resource type</span></span>

<span data-ttu-id="3c92a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c92a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c92a-105">包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="3c92a-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c92a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c92a-106">JSON representation</span></span>

<span data-ttu-id="3c92a-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c92a-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c92a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c92a-108">Properties</span></span>

| <span data-ttu-id="3c92a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3c92a-109">Property</span></span>              | <span data-ttu-id="3c92a-110">类型</span><span class="sxs-lookup"><span data-stu-id="3c92a-110">Type</span></span>          | <span data-ttu-id="3c92a-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c92a-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="3c92a-112">title</span><span class="sxs-lookup"><span data-stu-id="3c92a-112">title</span></span>                 | <span data-ttu-id="3c92a-113">String</span><span class="sxs-lookup"><span data-stu-id="3c92a-113">String</span></span>        | <span data-ttu-id="3c92a-114">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="3c92a-114">The item's title text.</span></span>               |
| <span data-ttu-id="3c92a-115">type</span><span class="sxs-lookup"><span data-stu-id="3c92a-115">type</span></span>              | <span data-ttu-id="3c92a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-116">String</span></span>        | <span data-ttu-id="3c92a-117">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="3c92a-117">The item's media type.</span></span> <span data-ttu-id="3c92a-118">可用于根据特定类型筛选特定文件。</span><span class="sxs-lookup"><span data-stu-id="3c92a-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="3c92a-119">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="3c92a-119">See below for supported types.</span></span> |
| <span data-ttu-id="3c92a-120">群组</span><span class="sxs-lookup"><span data-stu-id="3c92a-120">mediaType</span></span>             | <span data-ttu-id="3c92a-121">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-121">String</span></span>        | <span data-ttu-id="3c92a-122">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="3c92a-122">The item's media type.</span></span> <span data-ttu-id="3c92a-123">可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。</span><span class="sxs-lookup"><span data-stu-id="3c92a-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="3c92a-124">请注意，并非所有媒体 Mime 类型都受支持。</span><span class="sxs-lookup"><span data-stu-id="3c92a-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="3c92a-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="3c92a-125">previewImageUrl</span></span>       | <span data-ttu-id="3c92a-126">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-126">String</span></span>        | <span data-ttu-id="3c92a-127">指向项目的预览图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="3c92a-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="3c92a-128">previewText</span><span class="sxs-lookup"><span data-stu-id="3c92a-128">previewText</span></span>           | <span data-ttu-id="3c92a-129">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-129">String</span></span>        | <span data-ttu-id="3c92a-130">项目的预览文本。</span><span class="sxs-lookup"><span data-stu-id="3c92a-130">A preview text for the item.</span></span> |
| <span data-ttu-id="3c92a-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="3c92a-131">containerWebUrl</span></span>       | <span data-ttu-id="3c92a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-132">String</span></span>        | <span data-ttu-id="3c92a-133">指向存储项目的文件夹的路径。</span><span class="sxs-lookup"><span data-stu-id="3c92a-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="3c92a-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c92a-134">containerDisplayName</span></span>  | <span data-ttu-id="3c92a-135">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-135">String</span></span>        | <span data-ttu-id="3c92a-136">一个描述项目存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="3c92a-136">A string describing where the item is stored.</span></span> <span data-ttu-id="3c92a-137">例如，SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。</span><span class="sxs-lookup"><span data-stu-id="3c92a-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="3c92a-138">containerType</span><span class="sxs-lookup"><span data-stu-id="3c92a-138">containerType</span></span>         | <span data-ttu-id="3c92a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3c92a-139">String</span></span> | <span data-ttu-id="3c92a-140">可用于按存储文件的容器的类型进行筛选。</span><span class="sxs-lookup"><span data-stu-id="3c92a-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="3c92a-141">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="3c92a-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="3c92a-142">类型属性值</span><span class="sxs-lookup"><span data-stu-id="3c92a-142">Type property values</span></span>
-   <span data-ttu-id="3c92a-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="3c92a-143">PowerPoint</span></span>
-   <span data-ttu-id="3c92a-144">Word</span><span class="sxs-lookup"><span data-stu-id="3c92a-144">Word</span></span>
-   <span data-ttu-id="3c92a-145">Excel</span><span class="sxs-lookup"><span data-stu-id="3c92a-145">Excel</span></span>
-   <span data-ttu-id="3c92a-146">Pdf</span><span class="sxs-lookup"><span data-stu-id="3c92a-146">Pdf</span></span>
-   <span data-ttu-id="3c92a-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="3c92a-147">OneNote</span></span>
-   <span data-ttu-id="3c92a-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="3c92a-148">OneNotePage</span></span>
-   <span data-ttu-id="3c92a-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="3c92a-149">InfoPath</span></span>
-   <span data-ttu-id="3c92a-150">Visio</span><span class="sxs-lookup"><span data-stu-id="3c92a-150">Visio</span></span>
-   <span data-ttu-id="3c92a-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="3c92a-151">Publisher</span></span>
-   <span data-ttu-id="3c92a-152">Project</span><span class="sxs-lookup"><span data-stu-id="3c92a-152">Project</span></span>
-   <span data-ttu-id="3c92a-153">Access</span><span class="sxs-lookup"><span data-stu-id="3c92a-153">Access</span></span>
-   <span data-ttu-id="3c92a-154">邮件</span><span class="sxs-lookup"><span data-stu-id="3c92a-154">Mail</span></span>
-   <span data-ttu-id="3c92a-155">Csv</span><span class="sxs-lookup"><span data-stu-id="3c92a-155">Csv</span></span>
-   <span data-ttu-id="3c92a-156">存档</span><span class="sxs-lookup"><span data-stu-id="3c92a-156">Archive</span></span>
-   <span data-ttu-id="3c92a-157">Xps</span><span class="sxs-lookup"><span data-stu-id="3c92a-157">Xps</span></span>
-   <span data-ttu-id="3c92a-158">音频</span><span class="sxs-lookup"><span data-stu-id="3c92a-158">Audio</span></span>
-   <span data-ttu-id="3c92a-159">视频</span><span class="sxs-lookup"><span data-stu-id="3c92a-159">Video</span></span>
-   <span data-ttu-id="3c92a-160">图像</span><span class="sxs-lookup"><span data-stu-id="3c92a-160">Image</span></span>
-   <span data-ttu-id="3c92a-161">Web</span><span class="sxs-lookup"><span data-stu-id="3c92a-161">Web</span></span>
-   <span data-ttu-id="3c92a-162">文本</span><span class="sxs-lookup"><span data-stu-id="3c92a-162">Text</span></span>
-   <span data-ttu-id="3c92a-163">Xml</span><span class="sxs-lookup"><span data-stu-id="3c92a-163">Xml</span></span>
-   <span data-ttu-id="3c92a-164">Story</span><span class="sxs-lookup"><span data-stu-id="3c92a-164">Story</span></span>
-   <span data-ttu-id="3c92a-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="3c92a-165">ExternalContent</span></span>
-   <span data-ttu-id="3c92a-166">Folder</span><span class="sxs-lookup"><span data-stu-id="3c92a-166">Folder</span></span>
-   <span data-ttu-id="3c92a-167">其他</span><span class="sxs-lookup"><span data-stu-id="3c92a-167">Other</span></span>

<span data-ttu-id="3c92a-168">示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="3c92a-168">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="3c92a-169">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="3c92a-169">containerType property values</span></span>
<span data-ttu-id="3c92a-170">根据[officeGraphInsights](officegraphinsights.md)返回文件的容器，受支持的类型可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="3c92a-170">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="3c92a-171">例如，仅[sharedInsight](insights-shared.md)真知灼见将从 "收存箱"、"Box" 和 "GDrive" 返回文件。</span><span class="sxs-lookup"><span data-stu-id="3c92a-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="3c92a-172">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="3c92a-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="3c92a-173">站点</span><span class="sxs-lookup"><span data-stu-id="3c92a-173">Site</span></span>
-   <span data-ttu-id="3c92a-174">邮件</span><span class="sxs-lookup"><span data-stu-id="3c92a-174">Mail</span></span>
-   <span data-ttu-id="3c92a-175">箱</span><span class="sxs-lookup"><span data-stu-id="3c92a-175">DropBox</span></span>
-   <span data-ttu-id="3c92a-176">Box</span><span class="sxs-lookup"><span data-stu-id="3c92a-176">Box</span></span>
-   <span data-ttu-id="3c92a-177">GDrive</span><span class="sxs-lookup"><span data-stu-id="3c92a-177">GDrive</span></span>

<span data-ttu-id="3c92a-178">示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="3c92a-178">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
