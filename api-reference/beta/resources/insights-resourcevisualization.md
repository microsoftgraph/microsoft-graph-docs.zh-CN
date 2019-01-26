---
title: resourceVisualization 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9dc2d50a5bc694204317f8c3332263ce5259e2fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575102"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="6a452-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a452-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a452-104">包含属性的[officeGraphInsights](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-104">Complex type containing properties of [officeGraphInsights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a452-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a452-105">JSON representation</span></span>

<span data-ttu-id="6a452-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a452-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
}
```

## <a name="properties"></a><span data-ttu-id="6a452-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a452-107">Properties</span></span>

| <span data-ttu-id="6a452-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a452-108">Property</span></span>              | <span data-ttu-id="6a452-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a452-109">Type</span></span>          | <span data-ttu-id="6a452-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a452-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="6a452-111">title</span><span class="sxs-lookup"><span data-stu-id="6a452-111">title</span></span>                 | <span data-ttu-id="6a452-112">String</span><span class="sxs-lookup"><span data-stu-id="6a452-112">String</span></span>        | <span data-ttu-id="6a452-113">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="6a452-113">The item's title text.</span></span>               |
| <span data-ttu-id="6a452-114">type</span><span class="sxs-lookup"><span data-stu-id="6a452-114">type</span></span>              | <span data-ttu-id="6a452-115">String</span><span class="sxs-lookup"><span data-stu-id="6a452-115">String</span></span>        | <span data-ttu-id="6a452-116">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-116">The item's media type.</span></span> <span data-ttu-id="6a452-117">可用于根据特定类型的特定文件筛选。</span><span class="sxs-lookup"><span data-stu-id="6a452-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="6a452-118">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-118">See below for supported types.</span></span> |
| <span data-ttu-id="6a452-119">媒体类型</span><span class="sxs-lookup"><span data-stu-id="6a452-119">mediaType</span></span>             | <span data-ttu-id="6a452-120">String</span><span class="sxs-lookup"><span data-stu-id="6a452-120">String</span></span>        | <span data-ttu-id="6a452-121">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-121">The item's media type.</span></span> <span data-ttu-id="6a452-122">可用于筛选文件根据支持 IANA 媒体 Mime 类型为特定类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="6a452-123">请注意，不是所有媒体 Mime 类型都受都支持。</span><span class="sxs-lookup"><span data-stu-id="6a452-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="6a452-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="6a452-124">previewImageUrl</span></span>       | <span data-ttu-id="6a452-125">String</span><span class="sxs-lookup"><span data-stu-id="6a452-125">String</span></span>        | <span data-ttu-id="6a452-126">导致项目的预览图像 URL。</span><span class="sxs-lookup"><span data-stu-id="6a452-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="6a452-127">previewText</span><span class="sxs-lookup"><span data-stu-id="6a452-127">previewText</span></span>           | <span data-ttu-id="6a452-128">String</span><span class="sxs-lookup"><span data-stu-id="6a452-128">String</span></span>        | <span data-ttu-id="6a452-129">预览文本项。</span><span class="sxs-lookup"><span data-stu-id="6a452-129">A preview text for the item.</span></span> |
| <span data-ttu-id="6a452-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="6a452-130">containerWebUrl</span></span>       | <span data-ttu-id="6a452-131">String</span><span class="sxs-lookup"><span data-stu-id="6a452-131">String</span></span>        | <span data-ttu-id="6a452-132">前导到在其中存储项目的文件夹路径。</span><span class="sxs-lookup"><span data-stu-id="6a452-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="6a452-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a452-133">containerDisplayName</span></span>  | <span data-ttu-id="6a452-134">String</span><span class="sxs-lookup"><span data-stu-id="6a452-134">String</span></span>        | <span data-ttu-id="6a452-135">描述项目的存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="6a452-135">A string describing where the item is stored.</span></span> <span data-ttu-id="6a452-136">例如，SharePoint 网站或标识的 OneDrive 存储项目所有者的用户名称的名称。</span><span class="sxs-lookup"><span data-stu-id="6a452-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="6a452-137">containerType</span><span class="sxs-lookup"><span data-stu-id="6a452-137">containerType</span></span>         | <span data-ttu-id="6a452-138">String</span><span class="sxs-lookup"><span data-stu-id="6a452-138">String</span></span> | <span data-ttu-id="6a452-139">可用于筛选按在其中存储文件的容器的类型。</span><span class="sxs-lookup"><span data-stu-id="6a452-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="6a452-140">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="6a452-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="6a452-141">类型属性值</span><span class="sxs-lookup"><span data-stu-id="6a452-141">Type property values</span></span>
-   <span data-ttu-id="6a452-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="6a452-142">PowerPoint</span></span>
-   <span data-ttu-id="6a452-143">Word</span><span class="sxs-lookup"><span data-stu-id="6a452-143">Word</span></span>
-   <span data-ttu-id="6a452-144">Excel</span><span class="sxs-lookup"><span data-stu-id="6a452-144">Excel</span></span>
-   <span data-ttu-id="6a452-145">Pdf</span><span class="sxs-lookup"><span data-stu-id="6a452-145">Pdf</span></span>
-   <span data-ttu-id="6a452-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="6a452-146">OneNote</span></span>
-   <span data-ttu-id="6a452-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="6a452-147">OneNotePage</span></span>
-   <span data-ttu-id="6a452-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="6a452-148">InfoPath</span></span>
-   <span data-ttu-id="6a452-149">Visio</span><span class="sxs-lookup"><span data-stu-id="6a452-149">Visio</span></span>
-   <span data-ttu-id="6a452-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="6a452-150">Publisher</span></span>
-   <span data-ttu-id="6a452-151">项目</span><span class="sxs-lookup"><span data-stu-id="6a452-151">Project</span></span>
-   <span data-ttu-id="6a452-152">Access</span><span class="sxs-lookup"><span data-stu-id="6a452-152">Access</span></span>
-   <span data-ttu-id="6a452-153">邮件</span><span class="sxs-lookup"><span data-stu-id="6a452-153">Mail</span></span>
-   <span data-ttu-id="6a452-154">Csv</span><span class="sxs-lookup"><span data-stu-id="6a452-154">Csv</span></span>
-   <span data-ttu-id="6a452-155">存档</span><span class="sxs-lookup"><span data-stu-id="6a452-155">Archive</span></span>
-   <span data-ttu-id="6a452-156">Xps</span><span class="sxs-lookup"><span data-stu-id="6a452-156">Xps</span></span>
-   <span data-ttu-id="6a452-157">音频</span><span class="sxs-lookup"><span data-stu-id="6a452-157">Audio</span></span>
-   <span data-ttu-id="6a452-158">视频</span><span class="sxs-lookup"><span data-stu-id="6a452-158">Video</span></span>
-   <span data-ttu-id="6a452-159">图像</span><span class="sxs-lookup"><span data-stu-id="6a452-159">Image</span></span>
-   <span data-ttu-id="6a452-160">Web</span><span class="sxs-lookup"><span data-stu-id="6a452-160">Web</span></span>
-   <span data-ttu-id="6a452-161">文本</span><span class="sxs-lookup"><span data-stu-id="6a452-161">Text</span></span>
-   <span data-ttu-id="6a452-162">Xml</span><span class="sxs-lookup"><span data-stu-id="6a452-162">Xml</span></span>
-   <span data-ttu-id="6a452-163">文章</span><span class="sxs-lookup"><span data-stu-id="6a452-163">Story</span></span>
-   <span data-ttu-id="6a452-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="6a452-164">ExternalContent</span></span>
-   <span data-ttu-id="6a452-165">Folder</span><span class="sxs-lookup"><span data-stu-id="6a452-165">Folder</span></span>
-   <span data-ttu-id="6a452-166">Other</span><span class="sxs-lookup"><span data-stu-id="6a452-166">Other</span></span>

<span data-ttu-id="6a452-167">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="6a452-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="6a452-168">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="6a452-168">containerType property values</span></span>
<span data-ttu-id="6a452-169">受支持的类型从其[洞察](insights.md)返回文件的容器可能因用。</span><span class="sxs-lookup"><span data-stu-id="6a452-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="6a452-170">例如，仅[共享](insights-shared.md)洞察返回文件 '收存箱、 框中，和 GDrive。</span><span class="sxs-lookup"><span data-stu-id="6a452-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="6a452-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="6a452-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="6a452-172">Site</span><span class="sxs-lookup"><span data-stu-id="6a452-172">Site</span></span>
-   <span data-ttu-id="6a452-173">邮件</span><span class="sxs-lookup"><span data-stu-id="6a452-173">Mail</span></span>
-   <span data-ttu-id="6a452-174">收存箱</span><span class="sxs-lookup"><span data-stu-id="6a452-174">DropBox</span></span>
-   <span data-ttu-id="6a452-175">盒状</span><span class="sxs-lookup"><span data-stu-id="6a452-175">Box</span></span>
-   <span data-ttu-id="6a452-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="6a452-176">GDrive</span></span>

<span data-ttu-id="6a452-177">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="6a452-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
