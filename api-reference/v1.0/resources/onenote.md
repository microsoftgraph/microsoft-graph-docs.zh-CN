---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: cd2d8f52043541684d6c56c706ba9b0e3e3b6c78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082957"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="aca29-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="aca29-103">onenote resource type</span></span>

<span data-ttu-id="aca29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aca29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aca29-105">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="aca29-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="aca29-106">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="aca29-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="aca29-107">位置可以是 Microsoft 365 的用户笔记簿，或是消费者版 OneDrive ，或者是组笔记，或者可以是Microsoft 365 上的 SharePoint 站点托管团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="aca29-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="aca29-108">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="aca29-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="aca29-109">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="aca29-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="aca29-110">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="aca29-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="aca29-111">授权</span><span class="sxs-lookup"><span data-stu-id="aca29-111">Authorization</span></span>

<span data-ttu-id="aca29-112">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="aca29-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="aca29-113">关系</span><span class="sxs-lookup"><span data-stu-id="aca29-113">Relationships</span></span>
| <span data-ttu-id="aca29-114">关系</span><span class="sxs-lookup"><span data-stu-id="aca29-114">Relationship</span></span> | <span data-ttu-id="aca29-115">类型</span><span class="sxs-lookup"><span data-stu-id="aca29-115">Type</span></span>   |<span data-ttu-id="aca29-116">说明</span><span class="sxs-lookup"><span data-stu-id="aca29-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aca29-117">笔记本</span><span class="sxs-lookup"><span data-stu-id="aca29-117">notebooks</span></span>|<span data-ttu-id="aca29-118">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="aca29-118">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="aca29-119">用户或组所有的 OneNote 笔记本集合。</span><span class="sxs-lookup"><span data-stu-id="aca29-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="aca29-120">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-120">Read-only.</span></span> <span data-ttu-id="aca29-121">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aca29-121">Nullable.</span></span>|
|<span data-ttu-id="aca29-122">operations</span><span class="sxs-lookup"><span data-stu-id="aca29-122">operations</span></span>|<span data-ttu-id="aca29-123">[OnenoteOperation](onenoteoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-123">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="aca29-124">OneNote 操作状态。</span><span class="sxs-lookup"><span data-stu-id="aca29-124">The status of OneNote operations.</span></span> <span data-ttu-id="aca29-125">不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="aca29-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="aca29-126">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-126">Read-only.</span></span> <span data-ttu-id="aca29-127">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aca29-127">Nullable.</span></span>|
|<span data-ttu-id="aca29-128">pages</span><span class="sxs-lookup"><span data-stu-id="aca29-128">pages</span></span>|<span data-ttu-id="aca29-129">[OnenotePage](page.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-129">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="aca29-130">用户或组所有的全部 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="aca29-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="aca29-131">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-131">Read-only.</span></span> <span data-ttu-id="aca29-132">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aca29-132">Nullable.</span></span>|
|<span data-ttu-id="aca29-133">resources</span><span class="sxs-lookup"><span data-stu-id="aca29-133">resources</span></span>|<span data-ttu-id="aca29-134">[OnenoteResource](resource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-134">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="aca29-135">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="aca29-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="aca29-136">不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。</span><span class="sxs-lookup"><span data-stu-id="aca29-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="aca29-137">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-137">Read-only.</span></span> <span data-ttu-id="aca29-138">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aca29-138">Nullable.</span></span>|
|<span data-ttu-id="aca29-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="aca29-139">sectionGroups</span></span>|<span data-ttu-id="aca29-140">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-140">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="aca29-141">用户或组所有的全部 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="aca29-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="aca29-142">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-142">Read-only.</span></span> <span data-ttu-id="aca29-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aca29-143">Nullable.</span></span>|
|<span data-ttu-id="aca29-144">sections</span><span class="sxs-lookup"><span data-stu-id="aca29-144">sections</span></span>|<span data-ttu-id="aca29-145">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-145">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="aca29-146">用户或组所有的全部 OneNote 笔记本中的节。</span><span class="sxs-lookup"><span data-stu-id="aca29-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="aca29-147">只读。</span><span class="sxs-lookup"><span data-stu-id="aca29-147">Read-only.</span></span> <span data-ttu-id="aca29-148">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="aca29-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="aca29-149">方法</span><span class="sxs-lookup"><span data-stu-id="aca29-149">Methods</span></span>

| <span data-ttu-id="aca29-150">方法</span><span class="sxs-lookup"><span data-stu-id="aca29-150">Method</span></span>           | <span data-ttu-id="aca29-151">返回类型</span><span class="sxs-lookup"><span data-stu-id="aca29-151">Return Type</span></span>    |<span data-ttu-id="aca29-152">说明</span><span class="sxs-lookup"><span data-stu-id="aca29-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aca29-153">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="aca29-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="aca29-154">笔记本</span><span class="sxs-lookup"><span data-stu-id="aca29-154">Notebook</span></span>](notebook.md)| <span data-ttu-id="aca29-155">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="aca29-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="aca29-156">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="aca29-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="aca29-157">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="aca29-157">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="aca29-158">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="aca29-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="aca29-159">创建页面</span><span class="sxs-lookup"><span data-stu-id="aca29-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="aca29-160">页面</span><span class="sxs-lookup"><span data-stu-id="aca29-160">Page</span></span>](page.md)| <span data-ttu-id="aca29-161">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="aca29-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="aca29-162">列出页面</span><span class="sxs-lookup"><span data-stu-id="aca29-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="aca29-163">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="aca29-163">[Page](page.md) collection</span></span>| <span data-ttu-id="aca29-164">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="aca29-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="aca29-165">列出分区组</span><span class="sxs-lookup"><span data-stu-id="aca29-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="aca29-166">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-166">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="aca29-167">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="aca29-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="aca29-168">列出节</span><span class="sxs-lookup"><span data-stu-id="aca29-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="aca29-169">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aca29-169">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="aca29-170">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="aca29-170">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="aca29-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aca29-171">JSON Representation</span></span>
<span data-ttu-id="aca29-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aca29-172">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
```json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

