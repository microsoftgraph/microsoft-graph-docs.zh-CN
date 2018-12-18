---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: Jewan-microsoft
ms.openlocfilehash: 9570b99aad96196af6d21f41352dada9f4b869b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343650"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="249c9-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="249c9-103">onenote resource type</span></span>

<span data-ttu-id="249c9-104">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="249c9-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="249c9-105">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="249c9-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="249c9-106">位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="249c9-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="249c9-107">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="249c9-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="249c9-108">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="249c9-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="249c9-109">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="249c9-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="249c9-110">授权</span><span class="sxs-lookup"><span data-stu-id="249c9-110">Authorization</span></span>

<span data-ttu-id="249c9-111">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="249c9-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="249c9-112">关系</span><span class="sxs-lookup"><span data-stu-id="249c9-112">Relationships</span></span>
| <span data-ttu-id="249c9-113">关系</span><span class="sxs-lookup"><span data-stu-id="249c9-113">Relationship</span></span> | <span data-ttu-id="249c9-114">类型</span><span class="sxs-lookup"><span data-stu-id="249c9-114">Type</span></span>   |<span data-ttu-id="249c9-115">说明</span><span class="sxs-lookup"><span data-stu-id="249c9-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="249c9-116">笔记本</span><span class="sxs-lookup"><span data-stu-id="249c9-116">notebooks</span></span>|<span data-ttu-id="249c9-117">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="249c9-p101">用户或组所有的 OneNote 笔记本集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="249c9-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="249c9-121">操作</span><span class="sxs-lookup"><span data-stu-id="249c9-121">operations</span></span>|<span data-ttu-id="249c9-122">[OnenoteOperation](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="249c9-p102">OneNote 操作状态。不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="249c9-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="249c9-127">页面</span><span class="sxs-lookup"><span data-stu-id="249c9-127">pages</span></span>|<span data-ttu-id="249c9-128">[OnenotePage](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="249c9-p103">用户或组所有的全部 OneNote 笔记本中的页面。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="249c9-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="249c9-132">资源</span><span class="sxs-lookup"><span data-stu-id="249c9-132">resources</span></span>|<span data-ttu-id="249c9-133">[OnenoteResource](resource.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="249c9-p104">OneNote 页面中的图像和其他文件资源。不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="249c9-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="249c9-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="249c9-138">sectionGroups</span></span>|<span data-ttu-id="249c9-139">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="249c9-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="249c9-p105">用户或组所有的全部 OneNote 笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="249c9-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="249c9-143">节</span><span class="sxs-lookup"><span data-stu-id="249c9-143">sections</span></span>|<span data-ttu-id="249c9-144">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="249c9-p106">用户或组所有的全部 OneNote 笔记本中的节。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="249c9-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="249c9-148">方法</span><span class="sxs-lookup"><span data-stu-id="249c9-148">Methods</span></span>

| <span data-ttu-id="249c9-149">方法</span><span class="sxs-lookup"><span data-stu-id="249c9-149">Method</span></span>           | <span data-ttu-id="249c9-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="249c9-150">Return Type</span></span>    |<span data-ttu-id="249c9-151">说明</span><span class="sxs-lookup"><span data-stu-id="249c9-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="249c9-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="249c9-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="249c9-153">笔记本</span><span class="sxs-lookup"><span data-stu-id="249c9-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="249c9-154">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="249c9-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="249c9-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="249c9-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="249c9-156">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="249c9-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="249c9-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="249c9-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="249c9-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="249c9-159">页面</span><span class="sxs-lookup"><span data-stu-id="249c9-159">Page</span></span>](page.md)| <span data-ttu-id="249c9-160">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="249c9-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="249c9-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="249c9-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="249c9-162">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-162">[Page](page.md) collection</span></span>| <span data-ttu-id="249c9-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="249c9-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="249c9-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="249c9-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="249c9-165">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="249c9-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="249c9-166">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="249c9-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="249c9-167">列出节</span><span class="sxs-lookup"><span data-stu-id="249c9-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="249c9-168">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="249c9-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="249c9-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="249c9-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="249c9-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="249c9-170">JSON Representation</span></span>
<span data-ttu-id="249c9-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="249c9-171">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
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
