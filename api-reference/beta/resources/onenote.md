---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
ms.openlocfilehash: c1b875b686015df8134103b0793a1e342e7f4b89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043657"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="e7339-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7339-103">onenote resource type</span></span>

> <span data-ttu-id="e7339-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e7339-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7339-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e7339-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7339-106">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="e7339-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="e7339-107">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="e7339-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="e7339-108">位置可以是在 Office 365 或使用者 OneDrive 用户笔记本、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="e7339-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="e7339-109">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="e7339-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="e7339-110">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="e7339-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="e7339-111">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="e7339-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="e7339-112">授权</span><span class="sxs-lookup"><span data-stu-id="e7339-112">Authorization</span></span>

<span data-ttu-id="e7339-113">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e7339-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="e7339-114">关系</span><span class="sxs-lookup"><span data-stu-id="e7339-114">Relationships</span></span>
| <span data-ttu-id="e7339-115">关系</span><span class="sxs-lookup"><span data-stu-id="e7339-115">Relationship</span></span> | <span data-ttu-id="e7339-116">类型</span><span class="sxs-lookup"><span data-stu-id="e7339-116">Type</span></span>   |<span data-ttu-id="e7339-117">说明</span><span class="sxs-lookup"><span data-stu-id="e7339-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7339-118">笔记本</span><span class="sxs-lookup"><span data-stu-id="e7339-118">notebooks</span></span>|<span data-ttu-id="e7339-119">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="e7339-p102">用户或组所有的 OneNote 笔记本集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7339-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7339-123">操作</span><span class="sxs-lookup"><span data-stu-id="e7339-123">operations</span></span>|<span data-ttu-id="e7339-124">[操作](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="e7339-p103">OneNote 操作状态。不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7339-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7339-129">页面</span><span class="sxs-lookup"><span data-stu-id="e7339-129">pages</span></span>|<span data-ttu-id="e7339-130">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-130">[Page](page.md) collection</span></span>|<span data-ttu-id="e7339-p104">用户或组所有的全部 OneNote 笔记本中的页面。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7339-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7339-134">资源</span><span class="sxs-lookup"><span data-stu-id="e7339-134">resources</span></span>|<span data-ttu-id="e7339-135">[资源](resource.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="e7339-p105">OneNote 页面中的图像和其他文件资源。不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7339-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7339-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e7339-140">sectionGroups</span></span>|<span data-ttu-id="e7339-141">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7339-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e7339-p106">用户或组所有的全部 OneNote 笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7339-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7339-145">节</span><span class="sxs-lookup"><span data-stu-id="e7339-145">sections</span></span>|<span data-ttu-id="e7339-146">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-146">[Section](section.md) collection</span></span>|<span data-ttu-id="e7339-p107">用户或组所有的全部 OneNote 笔记本中的节。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e7339-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e7339-150">方法</span><span class="sxs-lookup"><span data-stu-id="e7339-150">Methods</span></span>

| <span data-ttu-id="e7339-151">方法</span><span class="sxs-lookup"><span data-stu-id="e7339-151">Method</span></span>           | <span data-ttu-id="e7339-152">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7339-152">Return Type</span></span>    |<span data-ttu-id="e7339-153">说明</span><span class="sxs-lookup"><span data-stu-id="e7339-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7339-154">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="e7339-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="e7339-155">笔记本</span><span class="sxs-lookup"><span data-stu-id="e7339-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="e7339-156">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="e7339-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="e7339-157">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="e7339-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="e7339-158">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="e7339-159">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="e7339-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="e7339-160">创建页面</span><span class="sxs-lookup"><span data-stu-id="e7339-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="e7339-161">页面</span><span class="sxs-lookup"><span data-stu-id="e7339-161">Page</span></span>](page.md)| <span data-ttu-id="e7339-162">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="e7339-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="e7339-163">列出页面</span><span class="sxs-lookup"><span data-stu-id="e7339-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="e7339-164">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-164">[Page](page.md) collection</span></span>| <span data-ttu-id="e7339-165">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="e7339-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="e7339-166">列出分区组</span><span class="sxs-lookup"><span data-stu-id="e7339-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="e7339-167">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7339-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e7339-168">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="e7339-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="e7339-169">列出节</span><span class="sxs-lookup"><span data-stu-id="e7339-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="e7339-170">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7339-170">[Section](section.md) collection</span></span>| <span data-ttu-id="e7339-171">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="e7339-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
