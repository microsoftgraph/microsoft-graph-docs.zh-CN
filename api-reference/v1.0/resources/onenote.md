---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8c81804c9ea93e6da9f0f9b7134f5b38aa4afd64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961977"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="fde69-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="fde69-103">onenote resource type</span></span>

<span data-ttu-id="fde69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fde69-105">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="fde69-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="fde69-106">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fde69-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="fde69-107">位置可以是 Microsoft 365 的用户笔记簿，或是消费者版 OneDrive ，或者是组笔记，或者可以是Microsoft 365 上的 SharePoint 站点托管团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="fde69-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="fde69-108">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="fde69-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="fde69-109">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fde69-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="fde69-110">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fde69-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="fde69-111">授权</span><span class="sxs-lookup"><span data-stu-id="fde69-111">Authorization</span></span>

<span data-ttu-id="fde69-112">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="fde69-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="fde69-113">关系</span><span class="sxs-lookup"><span data-stu-id="fde69-113">Relationships</span></span>
| <span data-ttu-id="fde69-114">关系</span><span class="sxs-lookup"><span data-stu-id="fde69-114">Relationship</span></span> | <span data-ttu-id="fde69-115">类型</span><span class="sxs-lookup"><span data-stu-id="fde69-115">Type</span></span>   |<span data-ttu-id="fde69-116">说明</span><span class="sxs-lookup"><span data-stu-id="fde69-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fde69-117">笔记本</span><span class="sxs-lookup"><span data-stu-id="fde69-117">notebooks</span></span>|<span data-ttu-id="fde69-118">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-118">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="fde69-119">用户或组所有的 OneNote 笔记本集合。</span><span class="sxs-lookup"><span data-stu-id="fde69-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="fde69-120">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-120">Read-only.</span></span> <span data-ttu-id="fde69-121">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fde69-121">Nullable.</span></span>|
|<span data-ttu-id="fde69-122">operations</span><span class="sxs-lookup"><span data-stu-id="fde69-122">operations</span></span>|<span data-ttu-id="fde69-123">[OnenoteOperation](onenoteoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-123">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="fde69-124">OneNote 操作状态。</span><span class="sxs-lookup"><span data-stu-id="fde69-124">The status of OneNote operations.</span></span> <span data-ttu-id="fde69-125">不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fde69-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="fde69-126">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-126">Read-only.</span></span> <span data-ttu-id="fde69-127">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fde69-127">Nullable.</span></span>|
|<span data-ttu-id="fde69-128">pages</span><span class="sxs-lookup"><span data-stu-id="fde69-128">pages</span></span>|<span data-ttu-id="fde69-129">[OnenotePage](page.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-129">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="fde69-130">用户或组所有的全部 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="fde69-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fde69-131">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-131">Read-only.</span></span> <span data-ttu-id="fde69-132">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fde69-132">Nullable.</span></span>|
|<span data-ttu-id="fde69-133">resources</span><span class="sxs-lookup"><span data-stu-id="fde69-133">resources</span></span>|<span data-ttu-id="fde69-134">[OnenoteResource](resource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-134">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="fde69-135">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="fde69-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="fde69-136">不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。</span><span class="sxs-lookup"><span data-stu-id="fde69-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="fde69-137">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-137">Read-only.</span></span> <span data-ttu-id="fde69-138">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fde69-138">Nullable.</span></span>|
|<span data-ttu-id="fde69-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="fde69-139">sectionGroups</span></span>|<span data-ttu-id="fde69-140">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-140">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="fde69-141">用户或组所有的全部 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="fde69-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fde69-142">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-142">Read-only.</span></span> <span data-ttu-id="fde69-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fde69-143">Nullable.</span></span>|
|<span data-ttu-id="fde69-144">sections</span><span class="sxs-lookup"><span data-stu-id="fde69-144">sections</span></span>|<span data-ttu-id="fde69-145">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-145">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="fde69-146">用户或组所有的全部 OneNote 笔记本中的节。</span><span class="sxs-lookup"><span data-stu-id="fde69-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fde69-147">只读。</span><span class="sxs-lookup"><span data-stu-id="fde69-147">Read-only.</span></span> <span data-ttu-id="fde69-148">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fde69-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="fde69-149">方法</span><span class="sxs-lookup"><span data-stu-id="fde69-149">Methods</span></span>

| <span data-ttu-id="fde69-150">方法</span><span class="sxs-lookup"><span data-stu-id="fde69-150">Method</span></span>           | <span data-ttu-id="fde69-151">返回类型</span><span class="sxs-lookup"><span data-stu-id="fde69-151">Return Type</span></span>    |<span data-ttu-id="fde69-152">说明</span><span class="sxs-lookup"><span data-stu-id="fde69-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fde69-153">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="fde69-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="fde69-154">笔记本</span><span class="sxs-lookup"><span data-stu-id="fde69-154">Notebook</span></span>](notebook.md)| <span data-ttu-id="fde69-155">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="fde69-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="fde69-156">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="fde69-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="fde69-157">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="fde69-157">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="fde69-158">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="fde69-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="fde69-159">创建页面</span><span class="sxs-lookup"><span data-stu-id="fde69-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="fde69-160">页面</span><span class="sxs-lookup"><span data-stu-id="fde69-160">Page</span></span>](page.md)| <span data-ttu-id="fde69-161">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="fde69-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="fde69-162">列出页面</span><span class="sxs-lookup"><span data-stu-id="fde69-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="fde69-163">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="fde69-163">[Page](page.md) collection</span></span>| <span data-ttu-id="fde69-164">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="fde69-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="fde69-165">列出分区组</span><span class="sxs-lookup"><span data-stu-id="fde69-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="fde69-166">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-166">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="fde69-167">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="fde69-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="fde69-168">列出节</span><span class="sxs-lookup"><span data-stu-id="fde69-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="fde69-169">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fde69-169">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="fde69-170">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="fde69-170">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fde69-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fde69-171">JSON Representation</span></span>
<span data-ttu-id="fde69-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde69-172">Here is a JSON representation of the resource.</span></span>
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

