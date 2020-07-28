---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a318ace2f69269a62cce728d1ececf01df97f3e0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427387"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="a3a6e-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3a6e-103">resourceVisualization resource type</span></span>

<span data-ttu-id="a3a6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a6e-105">包含[itemInsights](iteminsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-105">Complex type containing properties of [itemInsights](iteminsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3a6e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3a6e-106">JSON representation</span></span>

<span data-ttu-id="a3a6e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3a6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3a6e-108">Properties</span></span>

| <span data-ttu-id="a3a6e-109">属性</span><span class="sxs-lookup"><span data-stu-id="a3a6e-109">Property</span></span>              | <span data-ttu-id="a3a6e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a3a6e-110">Type</span></span>          | <span data-ttu-id="a3a6e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3a6e-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="a3a6e-112">title</span><span class="sxs-lookup"><span data-stu-id="a3a6e-112">title</span></span>                 | <span data-ttu-id="a3a6e-113">String</span><span class="sxs-lookup"><span data-stu-id="a3a6e-113">String</span></span>        | <span data-ttu-id="a3a6e-114">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-114">The item's title text.</span></span>               |
| <span data-ttu-id="a3a6e-115">type</span><span class="sxs-lookup"><span data-stu-id="a3a6e-115">type</span></span>              | <span data-ttu-id="a3a6e-116">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-116">String</span></span>        | <span data-ttu-id="a3a6e-117">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-117">The item's media type.</span></span> <span data-ttu-id="a3a6e-118">可用于根据特定类型筛选特定文件。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="a3a6e-119">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-119">See below for supported types.</span></span> |
| <span data-ttu-id="a3a6e-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="a3a6e-120">mediaType</span></span>             | <span data-ttu-id="a3a6e-121">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-121">String</span></span>        | <span data-ttu-id="a3a6e-122">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-122">The item's media type.</span></span> <span data-ttu-id="a3a6e-123">可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="a3a6e-124">请注意，并非所有媒体 Mime 类型都受支持。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="a3a6e-125">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="a3a6e-125">previewImageUrl</span></span>       | <span data-ttu-id="a3a6e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-126">String</span></span>        | <span data-ttu-id="a3a6e-127">指向项目的预览图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="a3a6e-128">previewText</span><span class="sxs-lookup"><span data-stu-id="a3a6e-128">previewText</span></span>           | <span data-ttu-id="a3a6e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-129">String</span></span>        | <span data-ttu-id="a3a6e-130">项目的预览文本。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-130">A preview text for the item.</span></span> |
| <span data-ttu-id="a3a6e-131">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="a3a6e-131">containerWebUrl</span></span>       | <span data-ttu-id="a3a6e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-132">String</span></span>        | <span data-ttu-id="a3a6e-133">指向存储项目的文件夹的路径。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="a3a6e-134">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3a6e-134">containerDisplayName</span></span>  | <span data-ttu-id="a3a6e-135">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-135">String</span></span>        | <span data-ttu-id="a3a6e-136">一个描述项目存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-136">A string describing where the item is stored.</span></span> <span data-ttu-id="a3a6e-137">例如，SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="a3a6e-138">containerType</span><span class="sxs-lookup"><span data-stu-id="a3a6e-138">containerType</span></span>         | <span data-ttu-id="a3a6e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="a3a6e-139">String</span></span> | <span data-ttu-id="a3a6e-140">可用于按存储文件的容器的类型进行筛选。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="a3a6e-141">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="a3a6e-142">类型属性值</span><span class="sxs-lookup"><span data-stu-id="a3a6e-142">Type property values</span></span>
-   <span data-ttu-id="a3a6e-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="a3a6e-143">PowerPoint</span></span>
-   <span data-ttu-id="a3a6e-144">Word</span><span class="sxs-lookup"><span data-stu-id="a3a6e-144">Word</span></span>
-   <span data-ttu-id="a3a6e-145">Excel</span><span class="sxs-lookup"><span data-stu-id="a3a6e-145">Excel</span></span>
-   <span data-ttu-id="a3a6e-146">Pdf</span><span class="sxs-lookup"><span data-stu-id="a3a6e-146">Pdf</span></span>
-   <span data-ttu-id="a3a6e-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="a3a6e-147">OneNote</span></span>
-   <span data-ttu-id="a3a6e-148">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="a3a6e-148">OneNotePage</span></span>
-   <span data-ttu-id="a3a6e-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="a3a6e-149">InfoPath</span></span>
-   <span data-ttu-id="a3a6e-150">Visio</span><span class="sxs-lookup"><span data-stu-id="a3a6e-150">Visio</span></span>
-   <span data-ttu-id="a3a6e-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="a3a6e-151">Publisher</span></span>
-   <span data-ttu-id="a3a6e-152">Project</span><span class="sxs-lookup"><span data-stu-id="a3a6e-152">Project</span></span>
-   <span data-ttu-id="a3a6e-153">Access</span><span class="sxs-lookup"><span data-stu-id="a3a6e-153">Access</span></span>
-   <span data-ttu-id="a3a6e-154">邮件</span><span class="sxs-lookup"><span data-stu-id="a3a6e-154">Mail</span></span>
-   <span data-ttu-id="a3a6e-155">Csv</span><span class="sxs-lookup"><span data-stu-id="a3a6e-155">Csv</span></span>
-   <span data-ttu-id="a3a6e-156">存档</span><span class="sxs-lookup"><span data-stu-id="a3a6e-156">Archive</span></span>
-   <span data-ttu-id="a3a6e-157">Xps</span><span class="sxs-lookup"><span data-stu-id="a3a6e-157">Xps</span></span>
-   <span data-ttu-id="a3a6e-158">音频</span><span class="sxs-lookup"><span data-stu-id="a3a6e-158">Audio</span></span>
-   <span data-ttu-id="a3a6e-159">视频</span><span class="sxs-lookup"><span data-stu-id="a3a6e-159">Video</span></span>
-   <span data-ttu-id="a3a6e-160">图像</span><span class="sxs-lookup"><span data-stu-id="a3a6e-160">Image</span></span>
-   <span data-ttu-id="a3a6e-161">Web</span><span class="sxs-lookup"><span data-stu-id="a3a6e-161">Web</span></span>
-   <span data-ttu-id="a3a6e-162">文本</span><span class="sxs-lookup"><span data-stu-id="a3a6e-162">Text</span></span>
-   <span data-ttu-id="a3a6e-163">Xml</span><span class="sxs-lookup"><span data-stu-id="a3a6e-163">Xml</span></span>
-   <span data-ttu-id="a3a6e-164">Story</span><span class="sxs-lookup"><span data-stu-id="a3a6e-164">Story</span></span>
-   <span data-ttu-id="a3a6e-165">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="a3a6e-165">ExternalContent</span></span>
-   <span data-ttu-id="a3a6e-166">Folder</span><span class="sxs-lookup"><span data-stu-id="a3a6e-166">Folder</span></span>
-   <span data-ttu-id="a3a6e-167">其他</span><span class="sxs-lookup"><span data-stu-id="a3a6e-167">Other</span></span>

<span data-ttu-id="a3a6e-168">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="a3a6e-168">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="a3a6e-169">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="a3a6e-169">containerType property values</span></span>
<span data-ttu-id="a3a6e-170">根据[itemInsights](iteminsights.md)返回文件的容器，受支持的类型可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-170">The supported types can differ based on containers from which [itemInsights](iteminsights.md) returns files.</span></span> <span data-ttu-id="a3a6e-171">例如，仅[sharedInsight](insights-shared.md)真知灼见将从 "收存箱"、"Box" 和 "GDrive" 返回文件。</span><span class="sxs-lookup"><span data-stu-id="a3a6e-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="a3a6e-172">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="a3a6e-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="a3a6e-173">Site</span><span class="sxs-lookup"><span data-stu-id="a3a6e-173">Site</span></span>
-   <span data-ttu-id="a3a6e-174">邮件</span><span class="sxs-lookup"><span data-stu-id="a3a6e-174">Mail</span></span>
-   <span data-ttu-id="a3a6e-175">箱</span><span class="sxs-lookup"><span data-stu-id="a3a6e-175">DropBox</span></span>
-   <span data-ttu-id="a3a6e-176">Box</span><span class="sxs-lookup"><span data-stu-id="a3a6e-176">Box</span></span>
-   <span data-ttu-id="a3a6e-177">GDrive</span><span class="sxs-lookup"><span data-stu-id="a3a6e-177">GDrive</span></span>

<span data-ttu-id="a3a6e-178">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="a3a6e-178">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
