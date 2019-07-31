---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 215cf68cbf2efffacd6259aa64b0a00d5700b842
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009382"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="9a91b-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a91b-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a91b-104">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="9a91b-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="9a91b-105">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="9a91b-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="9a91b-106">位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="9a91b-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="9a91b-107">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="9a91b-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="9a91b-108">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="9a91b-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="9a91b-109">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="9a91b-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="9a91b-110">授权</span><span class="sxs-lookup"><span data-stu-id="9a91b-110">Authorization</span></span>

<span data-ttu-id="9a91b-111">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="9a91b-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="9a91b-112">关系</span><span class="sxs-lookup"><span data-stu-id="9a91b-112">Relationships</span></span>
| <span data-ttu-id="9a91b-113">关系</span><span class="sxs-lookup"><span data-stu-id="9a91b-113">Relationship</span></span> | <span data-ttu-id="9a91b-114">类型</span><span class="sxs-lookup"><span data-stu-id="9a91b-114">Type</span></span>   |<span data-ttu-id="9a91b-115">说明</span><span class="sxs-lookup"><span data-stu-id="9a91b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a91b-116">笔记本</span><span class="sxs-lookup"><span data-stu-id="9a91b-116">notebooks</span></span>|<span data-ttu-id="9a91b-117">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-117">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="9a91b-118">用户或组所有的 OneNote 笔记本集合。</span><span class="sxs-lookup"><span data-stu-id="9a91b-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="9a91b-119">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-119">Read-only.</span></span> <span data-ttu-id="9a91b-120">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9a91b-120">Nullable.</span></span>|
|<span data-ttu-id="9a91b-121">operations</span><span class="sxs-lookup"><span data-stu-id="9a91b-121">operations</span></span>|<span data-ttu-id="9a91b-122">[onenoteOperation](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-122">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="9a91b-123">OneNote 操作状态。</span><span class="sxs-lookup"><span data-stu-id="9a91b-123">The status of OneNote operations.</span></span> <span data-ttu-id="9a91b-124">不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9a91b-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="9a91b-125">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-125">Read-only.</span></span> <span data-ttu-id="9a91b-126">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9a91b-126">Nullable.</span></span>|
|<span data-ttu-id="9a91b-127">pages</span><span class="sxs-lookup"><span data-stu-id="9a91b-127">pages</span></span>|<span data-ttu-id="9a91b-128">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-128">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="9a91b-129">用户或组所有的全部 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="9a91b-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="9a91b-130">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-130">Read-only.</span></span> <span data-ttu-id="9a91b-131">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9a91b-131">Nullable.</span></span>|
|<span data-ttu-id="9a91b-132">resources</span><span class="sxs-lookup"><span data-stu-id="9a91b-132">resources</span></span>|<span data-ttu-id="9a91b-133">[onenoteResource](onenoteresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-133">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="9a91b-134">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="9a91b-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="9a91b-135">不支持获取资源集合，但可以[获取特定资源的二进制内容](onenoteresource.md)。</span><span class="sxs-lookup"><span data-stu-id="9a91b-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="9a91b-136">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-136">Read-only.</span></span> <span data-ttu-id="9a91b-137">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9a91b-137">Nullable.</span></span>|
|<span data-ttu-id="9a91b-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="9a91b-138">sectionGroups</span></span>|<span data-ttu-id="9a91b-139">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-139">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="9a91b-140">用户或组所有的全部 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="9a91b-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="9a91b-141">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-141">Read-only.</span></span> <span data-ttu-id="9a91b-142">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9a91b-142">Nullable.</span></span>|
|<span data-ttu-id="9a91b-143">sections</span><span class="sxs-lookup"><span data-stu-id="9a91b-143">sections</span></span>|<span data-ttu-id="9a91b-144">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-144">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="9a91b-145">用户或组所有的全部 OneNote 笔记本中的节。</span><span class="sxs-lookup"><span data-stu-id="9a91b-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="9a91b-146">只读。</span><span class="sxs-lookup"><span data-stu-id="9a91b-146">Read-only.</span></span> <span data-ttu-id="9a91b-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9a91b-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="9a91b-148">方法</span><span class="sxs-lookup"><span data-stu-id="9a91b-148">Methods</span></span>

| <span data-ttu-id="9a91b-149">方法</span><span class="sxs-lookup"><span data-stu-id="9a91b-149">Method</span></span>           | <span data-ttu-id="9a91b-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a91b-150">Return Type</span></span>    |<span data-ttu-id="9a91b-151">说明</span><span class="sxs-lookup"><span data-stu-id="9a91b-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a91b-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="9a91b-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="9a91b-153">笔记</span><span class="sxs-lookup"><span data-stu-id="9a91b-153">notebook</span></span>](notebook.md)| <span data-ttu-id="9a91b-154">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="9a91b-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="9a91b-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="9a91b-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="9a91b-156">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-156">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="9a91b-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="9a91b-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="9a91b-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="9a91b-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="9a91b-159">onenotePage</span><span class="sxs-lookup"><span data-stu-id="9a91b-159">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="9a91b-160">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="9a91b-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="9a91b-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="9a91b-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="9a91b-162">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-162">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="9a91b-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="9a91b-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="9a91b-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="9a91b-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="9a91b-165">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-165">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="9a91b-166">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="9a91b-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="9a91b-167">列出节</span><span class="sxs-lookup"><span data-stu-id="9a91b-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="9a91b-168">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a91b-168">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="9a91b-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="9a91b-169">Get a collection of sections.</span></span>|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
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
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
