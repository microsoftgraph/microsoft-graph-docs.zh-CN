---
title: resourceVisualization 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
ms.openlocfilehash: d0c54895468fc9a01017e448df57c09c654616e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333535"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="f67ff-103">resourceVisualization 资源类型</span><span class="sxs-lookup"><span data-stu-id="f67ff-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="f67ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f67ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f67ff-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f67ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f67ff-106">包含属性的[见解](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f67ff-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f67ff-107">JSON representation</span></span>

<span data-ttu-id="f67ff-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f67ff-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f67ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="f67ff-109">Properties</span></span>

| <span data-ttu-id="f67ff-110">属性</span><span class="sxs-lookup"><span data-stu-id="f67ff-110">Property</span></span>              | <span data-ttu-id="f67ff-111">类型</span><span class="sxs-lookup"><span data-stu-id="f67ff-111">Type</span></span>          | <span data-ttu-id="f67ff-112">说明</span><span class="sxs-lookup"><span data-stu-id="f67ff-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="f67ff-113">title</span><span class="sxs-lookup"><span data-stu-id="f67ff-113">title</span></span>                 | <span data-ttu-id="f67ff-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-114">String</span></span>        | <span data-ttu-id="f67ff-115">项目的标题文本。</span><span class="sxs-lookup"><span data-stu-id="f67ff-115">The item's title text.</span></span>               |
| <span data-ttu-id="f67ff-116">type</span><span class="sxs-lookup"><span data-stu-id="f67ff-116">type</span></span>              | <span data-ttu-id="f67ff-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-117">String</span></span>        | <span data-ttu-id="f67ff-118">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-118">The item's media type.</span></span> <span data-ttu-id="f67ff-119">可用于根据特定类型的特定文件筛选。</span><span class="sxs-lookup"><span data-stu-id="f67ff-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="f67ff-120">请参阅以下支持的类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-120">See below for supported types.</span></span> |
| <span data-ttu-id="f67ff-121">媒体类型</span><span class="sxs-lookup"><span data-stu-id="f67ff-121">mediaType</span></span>             | <span data-ttu-id="f67ff-122">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-122">String</span></span>        | <span data-ttu-id="f67ff-123">项目的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-123">The item's media type.</span></span> <span data-ttu-id="f67ff-124">可用于筛选文件根据支持 IANA 媒体 Mime 类型为特定类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="f67ff-125">请注意，不是所有媒体 Mime 类型都受都支持。</span><span class="sxs-lookup"><span data-stu-id="f67ff-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="f67ff-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="f67ff-126">previewImageUrl</span></span>       | <span data-ttu-id="f67ff-127">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-127">String</span></span>        | <span data-ttu-id="f67ff-128">导致项目的预览图像 URL。</span><span class="sxs-lookup"><span data-stu-id="f67ff-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="f67ff-129">previewText</span><span class="sxs-lookup"><span data-stu-id="f67ff-129">previewText</span></span>           | <span data-ttu-id="f67ff-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-130">String</span></span>        | <span data-ttu-id="f67ff-131">预览文本项。</span><span class="sxs-lookup"><span data-stu-id="f67ff-131">A preview text for the item.</span></span> |
| <span data-ttu-id="f67ff-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="f67ff-132">containerWebUrl</span></span>       | <span data-ttu-id="f67ff-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-133">String</span></span>        | <span data-ttu-id="f67ff-134">前导到在其中存储项目的文件夹路径。</span><span class="sxs-lookup"><span data-stu-id="f67ff-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="f67ff-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="f67ff-135">containerDisplayName</span></span>  | <span data-ttu-id="f67ff-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-136">String</span></span>        | <span data-ttu-id="f67ff-137">描述项目的存储位置的字符串。</span><span class="sxs-lookup"><span data-stu-id="f67ff-137">A string describing where the item is stored.</span></span> <span data-ttu-id="f67ff-138">例如，SharePoint 网站或标识的 OneDrive 存储项目所有者的用户名称的名称。</span><span class="sxs-lookup"><span data-stu-id="f67ff-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="f67ff-139">containerType</span><span class="sxs-lookup"><span data-stu-id="f67ff-139">containerType</span></span>         | <span data-ttu-id="f67ff-140">字符串</span><span class="sxs-lookup"><span data-stu-id="f67ff-140">String</span></span> | <span data-ttu-id="f67ff-141">可用于筛选按在其中存储文件的容器的类型。</span><span class="sxs-lookup"><span data-stu-id="f67ff-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="f67ff-142">如 Site 或 OneDriveBusiness。</span><span class="sxs-lookup"><span data-stu-id="f67ff-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="f67ff-143">类型属性值</span><span class="sxs-lookup"><span data-stu-id="f67ff-143">Type property values</span></span>
-   <span data-ttu-id="f67ff-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="f67ff-144">PowerPoint</span></span>
-   <span data-ttu-id="f67ff-145">Word</span><span class="sxs-lookup"><span data-stu-id="f67ff-145">Word</span></span>
-   <span data-ttu-id="f67ff-146">Excel</span><span class="sxs-lookup"><span data-stu-id="f67ff-146">Excel</span></span>
-   <span data-ttu-id="f67ff-147">Pdf</span><span class="sxs-lookup"><span data-stu-id="f67ff-147">Pdf</span></span>
-   <span data-ttu-id="f67ff-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="f67ff-148">OneNote</span></span>
-   <span data-ttu-id="f67ff-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="f67ff-149">OneNotePage</span></span>
-   <span data-ttu-id="f67ff-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="f67ff-150">InfoPath</span></span>
-   <span data-ttu-id="f67ff-151">Visio</span><span class="sxs-lookup"><span data-stu-id="f67ff-151">Visio</span></span>
-   <span data-ttu-id="f67ff-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="f67ff-152">Publisher</span></span>
-   <span data-ttu-id="f67ff-153">Project</span><span class="sxs-lookup"><span data-stu-id="f67ff-153">Project</span></span>
-   <span data-ttu-id="f67ff-154">Access</span><span class="sxs-lookup"><span data-stu-id="f67ff-154">Access</span></span>
-   <span data-ttu-id="f67ff-155">邮件</span><span class="sxs-lookup"><span data-stu-id="f67ff-155">Mail</span></span>
-   <span data-ttu-id="f67ff-156">Csv</span><span class="sxs-lookup"><span data-stu-id="f67ff-156">Csv</span></span>
-   <span data-ttu-id="f67ff-157">存档</span><span class="sxs-lookup"><span data-stu-id="f67ff-157">Archive</span></span>
-   <span data-ttu-id="f67ff-158">Xps</span><span class="sxs-lookup"><span data-stu-id="f67ff-158">Xps</span></span>
-   <span data-ttu-id="f67ff-159">音频</span><span class="sxs-lookup"><span data-stu-id="f67ff-159">Audio</span></span>
-   <span data-ttu-id="f67ff-160">视频</span><span class="sxs-lookup"><span data-stu-id="f67ff-160">Video</span></span>
-   <span data-ttu-id="f67ff-161">图像</span><span class="sxs-lookup"><span data-stu-id="f67ff-161">Image</span></span>
-   <span data-ttu-id="f67ff-162">Web</span><span class="sxs-lookup"><span data-stu-id="f67ff-162">Web</span></span>
-   <span data-ttu-id="f67ff-163">文本</span><span class="sxs-lookup"><span data-stu-id="f67ff-163">Text</span></span>
-   <span data-ttu-id="f67ff-164">Xml</span><span class="sxs-lookup"><span data-stu-id="f67ff-164">Xml</span></span>
-   <span data-ttu-id="f67ff-165">文章</span><span class="sxs-lookup"><span data-stu-id="f67ff-165">Story</span></span>
-   <span data-ttu-id="f67ff-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="f67ff-166">ExternalContent</span></span>
-   <span data-ttu-id="f67ff-167">Folder</span><span class="sxs-lookup"><span data-stu-id="f67ff-167">Folder</span></span>
-   <span data-ttu-id="f67ff-168">Other</span><span class="sxs-lookup"><span data-stu-id="f67ff-168">Other</span></span>

<span data-ttu-id="f67ff-169">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="f67ff-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="f67ff-170">containerType 属性值</span><span class="sxs-lookup"><span data-stu-id="f67ff-170">containerType property values</span></span>
<span data-ttu-id="f67ff-171">受支持的类型从其[洞察](insights.md)返回文件的容器可能因用。</span><span class="sxs-lookup"><span data-stu-id="f67ff-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="f67ff-172">例如，仅[共享](insights-shared.md)洞察返回文件 '收存箱、 框中，和 GDrive。</span><span class="sxs-lookup"><span data-stu-id="f67ff-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="f67ff-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="f67ff-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="f67ff-174">Site</span><span class="sxs-lookup"><span data-stu-id="f67ff-174">Site</span></span>
-   <span data-ttu-id="f67ff-175">邮件</span><span class="sxs-lookup"><span data-stu-id="f67ff-175">Mail</span></span>
-   <span data-ttu-id="f67ff-176">收存箱</span><span class="sxs-lookup"><span data-stu-id="f67ff-176">DropBox</span></span>
-   <span data-ttu-id="f67ff-177">盒状</span><span class="sxs-lookup"><span data-stu-id="f67ff-177">Box</span></span>
-   <span data-ttu-id="f67ff-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="f67ff-178">GDrive</span></span>

<span data-ttu-id="f67ff-179">示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="f67ff-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>