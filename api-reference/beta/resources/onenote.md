---
title: onenote 资源类型
description: OneNote 资源的入口点。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561654"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="74e3e-103">onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="74e3e-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e3e-104">OneNote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="74e3e-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="74e3e-105">通过 Microsoft Graph API 对 OneNote 服务进行的所有调用都使用此服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="74e3e-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="74e3e-106">该位置可以是 office 365 上的用户笔记本, 也可以是 office 365 上的使用者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="74e3e-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="74e3e-107">**用户笔记本**若要访问消费者 OneDrive 或 OneDrive for business 上的个人笔记本, 请使用下列 url 之一:</span><span class="sxs-lookup"><span data-stu-id="74e3e-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="74e3e-108">**组笔记本**若要访问组拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="74e3e-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="74e3e-109">**SharePoint 网站笔记本**若要访问 SharePoint 团队网站拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="74e3e-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="74e3e-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e3e-110">Authorization</span></span>

<span data-ttu-id="74e3e-111">有关使用 OneNote api 所需的权限的信息, 请参阅[Notes 权限](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="74e3e-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="74e3e-112">关系</span><span class="sxs-lookup"><span data-stu-id="74e3e-112">Relationships</span></span>
| <span data-ttu-id="74e3e-113">关系</span><span class="sxs-lookup"><span data-stu-id="74e3e-113">Relationship</span></span> | <span data-ttu-id="74e3e-114">类型</span><span class="sxs-lookup"><span data-stu-id="74e3e-114">Type</span></span>   |<span data-ttu-id="74e3e-115">说明</span><span class="sxs-lookup"><span data-stu-id="74e3e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74e3e-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="74e3e-116">notebooks</span></span>|<span data-ttu-id="74e3e-117">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="74e3e-118">用户或组拥有的 OneNote 笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="74e3e-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="74e3e-119">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-119">Read-only.</span></span> <span data-ttu-id="74e3e-120">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-120">Nullable.</span></span>|
|<span data-ttu-id="74e3e-121">operations</span><span class="sxs-lookup"><span data-stu-id="74e3e-121">operations</span></span>|<span data-ttu-id="74e3e-122">[操作](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="74e3e-123">OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="74e3e-123">The status of OneNote operations.</span></span> <span data-ttu-id="74e3e-124">不支持获取操作集合, 但如果响应中返回了`Operation-Location`标头, 则可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="74e3e-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="74e3e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-125">Read-only.</span></span> <span data-ttu-id="74e3e-126">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-126">Nullable.</span></span>|
|<span data-ttu-id="74e3e-127">pages</span><span class="sxs-lookup"><span data-stu-id="74e3e-127">pages</span></span>|<span data-ttu-id="74e3e-128">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-128">[Page](page.md) collection</span></span>|<span data-ttu-id="74e3e-129">由用户或组拥有的所有 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="74e3e-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="74e3e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-130">Read-only.</span></span> <span data-ttu-id="74e3e-131">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-131">Nullable.</span></span>|
|<span data-ttu-id="74e3e-132">资源</span><span class="sxs-lookup"><span data-stu-id="74e3e-132">resources</span></span>|<span data-ttu-id="74e3e-133">[资源](resource.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="74e3e-134">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="74e3e-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="74e3e-135">不支持获取资源集合, 但可以[获取特定资源的二进制内容](resource.md)。</span><span class="sxs-lookup"><span data-stu-id="74e3e-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="74e3e-136">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-136">Read-only.</span></span> <span data-ttu-id="74e3e-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-137">Nullable.</span></span>|
|<span data-ttu-id="74e3e-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="74e3e-138">sectionGroups</span></span>|<span data-ttu-id="74e3e-139">[SectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="74e3e-140">由用户或组拥有的所有 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="74e3e-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="74e3e-141">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-141">Read-only.</span></span> <span data-ttu-id="74e3e-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-142">Nullable.</span></span>|
|<span data-ttu-id="74e3e-143">分区</span><span class="sxs-lookup"><span data-stu-id="74e3e-143">sections</span></span>|<span data-ttu-id="74e3e-144">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-144">[Section](section.md) collection</span></span>|<span data-ttu-id="74e3e-145">所有 OneNote 笔记本中由用户或组所有的部分。</span><span class="sxs-lookup"><span data-stu-id="74e3e-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="74e3e-146">只读。</span><span class="sxs-lookup"><span data-stu-id="74e3e-146">Read-only.</span></span> <span data-ttu-id="74e3e-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74e3e-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="74e3e-148">方法</span><span class="sxs-lookup"><span data-stu-id="74e3e-148">Methods</span></span>

| <span data-ttu-id="74e3e-149">方法</span><span class="sxs-lookup"><span data-stu-id="74e3e-149">Method</span></span>           | <span data-ttu-id="74e3e-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="74e3e-150">Return Type</span></span>    |<span data-ttu-id="74e3e-151">说明</span><span class="sxs-lookup"><span data-stu-id="74e3e-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74e3e-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="74e3e-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="74e3e-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="74e3e-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="74e3e-154">通过发布到 "笔记本" 集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="74e3e-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="74e3e-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="74e3e-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="74e3e-156">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="74e3e-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="74e3e-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="74e3e-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="74e3e-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="74e3e-159">Page</span><span class="sxs-lookup"><span data-stu-id="74e3e-159">Page</span></span>](page.md)| <span data-ttu-id="74e3e-160">通过发布到 pages 集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="74e3e-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="74e3e-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="74e3e-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="74e3e-162">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-162">[Page](page.md) collection</span></span>| <span data-ttu-id="74e3e-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="74e3e-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="74e3e-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="74e3e-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="74e3e-165">[SectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="74e3e-166">获取节组的集合。</span><span class="sxs-lookup"><span data-stu-id="74e3e-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="74e3e-167">列出分区</span><span class="sxs-lookup"><span data-stu-id="74e3e-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="74e3e-168">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="74e3e-168">[Section](section.md) collection</span></span>| <span data-ttu-id="74e3e-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="74e3e-169">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
