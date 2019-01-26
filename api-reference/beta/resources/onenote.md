---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 6259f817058d0faebc77a0e1a22b478697d79b66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576085"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="ed669-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed669-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed669-104">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="ed669-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="ed669-105">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="ed669-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="ed669-106">位置可以是在 Office 365 或使用者 OneDrive 用户笔记本、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="ed669-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="ed669-107">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="ed669-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="ed669-108">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="ed669-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="ed669-109">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="ed669-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="ed669-110">授权</span><span class="sxs-lookup"><span data-stu-id="ed669-110">Authorization</span></span>

<span data-ttu-id="ed669-111">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="ed669-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="ed669-112">关系</span><span class="sxs-lookup"><span data-stu-id="ed669-112">Relationships</span></span>
| <span data-ttu-id="ed669-113">关系</span><span class="sxs-lookup"><span data-stu-id="ed669-113">Relationship</span></span> | <span data-ttu-id="ed669-114">类型</span><span class="sxs-lookup"><span data-stu-id="ed669-114">Type</span></span>   |<span data-ttu-id="ed669-115">说明</span><span class="sxs-lookup"><span data-stu-id="ed669-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed669-116">笔记本</span><span class="sxs-lookup"><span data-stu-id="ed669-116">notebooks</span></span>|<span data-ttu-id="ed669-117">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="ed669-p101">用户或组所有的 OneNote 笔记本集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ed669-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ed669-121">操作</span><span class="sxs-lookup"><span data-stu-id="ed669-121">operations</span></span>|<span data-ttu-id="ed669-122">[操作](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="ed669-p102">OneNote 操作状态。不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ed669-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ed669-127">页面</span><span class="sxs-lookup"><span data-stu-id="ed669-127">pages</span></span>|<span data-ttu-id="ed669-128">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-128">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="ed669-p103">用户或组所有的全部 OneNote 笔记本中的页面。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ed669-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="ed669-132">资源</span><span class="sxs-lookup"><span data-stu-id="ed669-132">resources</span></span>|<span data-ttu-id="ed669-133">[governanceResource](resource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-133">[governanceResource](resource.md) collection</span></span> |<span data-ttu-id="ed669-p104">OneNote 页面中的图像和其他文件资源。不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ed669-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="ed669-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ed669-138">sectionGroups</span></span>|<span data-ttu-id="ed669-139">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-139">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="ed669-p105">用户或组所有的全部 OneNote 笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ed669-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="ed669-143">节</span><span class="sxs-lookup"><span data-stu-id="ed669-143">sections</span></span>|<span data-ttu-id="ed669-144">[onenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-144">[onenoteSection](section.md) collection</span></span>|<span data-ttu-id="ed669-p106">用户或组所有的全部 OneNote 笔记本中的节。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ed669-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ed669-148">方法</span><span class="sxs-lookup"><span data-stu-id="ed669-148">Methods</span></span>

| <span data-ttu-id="ed669-149">方法</span><span class="sxs-lookup"><span data-stu-id="ed669-149">Method</span></span>           | <span data-ttu-id="ed669-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed669-150">Return Type</span></span>    |<span data-ttu-id="ed669-151">说明</span><span class="sxs-lookup"><span data-stu-id="ed669-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed669-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="ed669-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="ed669-153">笔记本</span><span class="sxs-lookup"><span data-stu-id="ed669-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="ed669-154">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="ed669-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="ed669-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="ed669-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="ed669-156">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="ed669-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="ed669-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="ed669-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="ed669-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="ed669-159">onenotePage</span><span class="sxs-lookup"><span data-stu-id="ed669-159">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="ed669-160">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="ed669-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="ed669-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="ed669-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="ed669-162">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-162">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="ed669-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="ed669-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="ed669-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="ed669-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="ed669-165">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed669-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="ed669-166">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="ed669-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="ed669-167">列出节</span><span class="sxs-lookup"><span data-stu-id="ed669-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="ed669-168">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="ed669-168">[Section](section.md) collection</span></span>| <span data-ttu-id="ed669-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="ed669-169">Get a collection of sections.</span></span>|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.oneNote"
}-->
``` json
{
}
```

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
