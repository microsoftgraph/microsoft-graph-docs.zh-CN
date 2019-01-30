---
title: resourceVisualization 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641293"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="aa166-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa166-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa166-104">包含属性的[见解](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa166-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa166-105">JSON representation</span></span>

<span data-ttu-id="aa166-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa166-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="aa166-107">属性</span><span class="sxs-lookup"><span data-stu-id="aa166-107">Properties</span></span>

| <span data-ttu-id="aa166-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa166-108">Property</span></span>              | <span data-ttu-id="aa166-109">类型</span><span class="sxs-lookup"><span data-stu-id="aa166-109">Type</span></span>          | <span data-ttu-id="aa166-110">说明</span><span class="sxs-lookup"><span data-stu-id="aa166-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="aa166-111">title</span><span class="sxs-lookup"><span data-stu-id="aa166-111">title</span></span>                 | <span data-ttu-id="aa166-112">String</span><span class="sxs-lookup"><span data-stu-id="aa166-112">String</span></span>        | <span data-ttu-id="aa166-113">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="aa166-113">The item's title text.</span></span>               |
| <span data-ttu-id="aa166-114">type</span><span class="sxs-lookup"><span data-stu-id="aa166-114">type</span></span>              | <span data-ttu-id="aa166-115">String</span><span class="sxs-lookup"><span data-stu-id="aa166-115">String</span></span>        | <span data-ttu-id="aa166-116">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-116">The item's media type.</span></span> <span data-ttu-id="aa166-117">可用于根据特定类型的特定文件筛选。</span><span class="sxs-lookup"><span data-stu-id="aa166-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="aa166-118">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-118">See below for supported types.</span></span> |
| <span data-ttu-id="aa166-119">媒体类型</span><span class="sxs-lookup"><span data-stu-id="aa166-119">mediaType</span></span>             | <span data-ttu-id="aa166-120">String</span><span class="sxs-lookup"><span data-stu-id="aa166-120">String</span></span>        | <span data-ttu-id="aa166-121">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-121">The item's media type.</span></span> <span data-ttu-id="aa166-122">可用于筛选文件根据支持 IANA 媒体 Mime 类型为特定类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="aa166-123">请注意，不是所有媒体 Mime 类型都受都支持。</span><span class="sxs-lookup"><span data-stu-id="aa166-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="aa166-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="aa166-124">previewImageUrl</span></span>       | <span data-ttu-id="aa166-125">String</span><span class="sxs-lookup"><span data-stu-id="aa166-125">String</span></span>        | <span data-ttu-id="aa166-126">导致项目的预览图像 URL。</span><span class="sxs-lookup"><span data-stu-id="aa166-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="aa166-127">previewText</span><span class="sxs-lookup"><span data-stu-id="aa166-127">previewText</span></span>           | <span data-ttu-id="aa166-128">String</span><span class="sxs-lookup"><span data-stu-id="aa166-128">String</span></span>        | <span data-ttu-id="aa166-129">预览文本项。</span><span class="sxs-lookup"><span data-stu-id="aa166-129">A preview text for the item.</span></span> |
| <span data-ttu-id="aa166-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="aa166-130">containerWebUrl</span></span>       | <span data-ttu-id="aa166-131">String</span><span class="sxs-lookup"><span data-stu-id="aa166-131">String</span></span>        | <span data-ttu-id="aa166-132">前导到在其中存储项目的文件夹路径。</span><span class="sxs-lookup"><span data-stu-id="aa166-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="aa166-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="aa166-133">containerDisplayName</span></span>  | <span data-ttu-id="aa166-134">String</span><span class="sxs-lookup"><span data-stu-id="aa166-134">String</span></span>        | <span data-ttu-id="aa166-135">描述项目的存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="aa166-135">A string describing where the item is stored.</span></span> <span data-ttu-id="aa166-136">例如，SharePoint 网站或标识的 OneDrive 存储项目所有者的用户名称的名称。</span><span class="sxs-lookup"><span data-stu-id="aa166-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="aa166-137">containerType</span><span class="sxs-lookup"><span data-stu-id="aa166-137">containerType</span></span>         | <span data-ttu-id="aa166-138">String</span><span class="sxs-lookup"><span data-stu-id="aa166-138">String</span></span> | <span data-ttu-id="aa166-139">可用于筛选按在其中存储文件的容器的类型。</span><span class="sxs-lookup"><span data-stu-id="aa166-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="aa166-140">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="aa166-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="aa166-141">类型属性值</span><span class="sxs-lookup"><span data-stu-id="aa166-141">Type property values</span></span>
-   <span data-ttu-id="aa166-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="aa166-142">PowerPoint</span></span>
-   <span data-ttu-id="aa166-143">Word</span><span class="sxs-lookup"><span data-stu-id="aa166-143">Word</span></span>
-   <span data-ttu-id="aa166-144">Excel</span><span class="sxs-lookup"><span data-stu-id="aa166-144">Excel</span></span>
-   <span data-ttu-id="aa166-145">Pdf</span><span class="sxs-lookup"><span data-stu-id="aa166-145">Pdf</span></span>
-   <span data-ttu-id="aa166-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="aa166-146">OneNote</span></span>
-   <span data-ttu-id="aa166-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="aa166-147">OneNotePage</span></span>
-   <span data-ttu-id="aa166-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="aa166-148">InfoPath</span></span>
-   <span data-ttu-id="aa166-149">Visio</span><span class="sxs-lookup"><span data-stu-id="aa166-149">Visio</span></span>
-   <span data-ttu-id="aa166-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="aa166-150">Publisher</span></span>
-   <span data-ttu-id="aa166-151">项目</span><span class="sxs-lookup"><span data-stu-id="aa166-151">Project</span></span>
-   <span data-ttu-id="aa166-152">Access</span><span class="sxs-lookup"><span data-stu-id="aa166-152">Access</span></span>
-   <span data-ttu-id="aa166-153">邮件</span><span class="sxs-lookup"><span data-stu-id="aa166-153">Mail</span></span>
-   <span data-ttu-id="aa166-154">Csv</span><span class="sxs-lookup"><span data-stu-id="aa166-154">Csv</span></span>
-   <span data-ttu-id="aa166-155">存档</span><span class="sxs-lookup"><span data-stu-id="aa166-155">Archive</span></span>
-   <span data-ttu-id="aa166-156">Xps</span><span class="sxs-lookup"><span data-stu-id="aa166-156">Xps</span></span>
-   <span data-ttu-id="aa166-157">音频</span><span class="sxs-lookup"><span data-stu-id="aa166-157">Audio</span></span>
-   <span data-ttu-id="aa166-158">视频</span><span class="sxs-lookup"><span data-stu-id="aa166-158">Video</span></span>
-   <span data-ttu-id="aa166-159">图像</span><span class="sxs-lookup"><span data-stu-id="aa166-159">Image</span></span>
-   <span data-ttu-id="aa166-160">Web</span><span class="sxs-lookup"><span data-stu-id="aa166-160">Web</span></span>
-   <span data-ttu-id="aa166-161">文本</span><span class="sxs-lookup"><span data-stu-id="aa166-161">Text</span></span>
-   <span data-ttu-id="aa166-162">Xml</span><span class="sxs-lookup"><span data-stu-id="aa166-162">Xml</span></span>
-   <span data-ttu-id="aa166-163">文章</span><span class="sxs-lookup"><span data-stu-id="aa166-163">Story</span></span>
-   <span data-ttu-id="aa166-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="aa166-164">ExternalContent</span></span>
-   <span data-ttu-id="aa166-165">Folder</span><span class="sxs-lookup"><span data-stu-id="aa166-165">Folder</span></span>
-   <span data-ttu-id="aa166-166">Other</span><span class="sxs-lookup"><span data-stu-id="aa166-166">Other</span></span>

<span data-ttu-id="aa166-167">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="aa166-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="aa166-168">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="aa166-168">containerType property values</span></span>
<span data-ttu-id="aa166-169">受支持的类型从其[洞察](insights.md)返回文件的容器可能因用。</span><span class="sxs-lookup"><span data-stu-id="aa166-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="aa166-170">例如，仅[共享](insights-shared.md)洞察返回文件 '收存箱、 框中，和 GDrive。</span><span class="sxs-lookup"><span data-stu-id="aa166-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="aa166-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="aa166-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="aa166-172">Site</span><span class="sxs-lookup"><span data-stu-id="aa166-172">Site</span></span>
-   <span data-ttu-id="aa166-173">邮件</span><span class="sxs-lookup"><span data-stu-id="aa166-173">Mail</span></span>
-   <span data-ttu-id="aa166-174">收存箱</span><span class="sxs-lookup"><span data-stu-id="aa166-174">DropBox</span></span>
-   <span data-ttu-id="aa166-175">盒状</span><span class="sxs-lookup"><span data-stu-id="aa166-175">Box</span></span>
-   <span data-ttu-id="aa166-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="aa166-176">GDrive</span></span>

<span data-ttu-id="aa166-177">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="aa166-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
