---
title: onenote 资源类型
description: OneNote 资源的入口点。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 44dfe7b33632bb6691802e46b66f54015b6aa6ae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341489"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="8a9bb-103">onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a9bb-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a9bb-104">OneNote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="8a9bb-105">通过 Microsoft Graph API 对 OneNote 服务进行的所有调用都使用此服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="8a9bb-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="8a9bb-106">该位置可以是 office 365 上的用户笔记本, 也可以是 office 365 上的使用者 OneDrive、组笔记本或 SharePoint 网站托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="8a9bb-107">**用户笔记本**若要访问消费者 OneDrive 或 OneDrive for business 上的个人笔记本, 请使用下列 url 之一:</span><span class="sxs-lookup"><span data-stu-id="8a9bb-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="8a9bb-108">**组笔记本**若要访问组拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="8a9bb-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="8a9bb-109">**SharePoint 网站笔记本**若要访问 SharePoint 团队网站拥有的笔记本, 请使用以下服务根 URL:</span><span class="sxs-lookup"><span data-stu-id="8a9bb-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="8a9bb-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a9bb-110">Authorization</span></span>

<span data-ttu-id="8a9bb-111">有关使用 OneNote api 所需的权限的信息, 请参阅[Notes 权限](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="8a9bb-112">关系</span><span class="sxs-lookup"><span data-stu-id="8a9bb-112">Relationships</span></span>
| <span data-ttu-id="8a9bb-113">关系</span><span class="sxs-lookup"><span data-stu-id="8a9bb-113">Relationship</span></span> | <span data-ttu-id="8a9bb-114">类型</span><span class="sxs-lookup"><span data-stu-id="8a9bb-114">Type</span></span>   |<span data-ttu-id="8a9bb-115">说明</span><span class="sxs-lookup"><span data-stu-id="8a9bb-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a9bb-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="8a9bb-116">notebooks</span></span>|<span data-ttu-id="8a9bb-117">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-117">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="8a9bb-118">用户或组拥有的 OneNote 笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="8a9bb-119">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-119">Read-only.</span></span> <span data-ttu-id="8a9bb-120">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-120">Nullable.</span></span>|
|<span data-ttu-id="8a9bb-121">operations</span><span class="sxs-lookup"><span data-stu-id="8a9bb-121">operations</span></span>|<span data-ttu-id="8a9bb-122">[onenoteOperation](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-122">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="8a9bb-123">OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-123">The status of OneNote operations.</span></span> <span data-ttu-id="8a9bb-124">不支持获取操作集合, 但如果响应中返回了`Operation-Location`标头, 则可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="8a9bb-125">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-125">Read-only.</span></span> <span data-ttu-id="8a9bb-126">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-126">Nullable.</span></span>|
|<span data-ttu-id="8a9bb-127">pages</span><span class="sxs-lookup"><span data-stu-id="8a9bb-127">pages</span></span>|<span data-ttu-id="8a9bb-128">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-128">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="8a9bb-129">由用户或组拥有的所有 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="8a9bb-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-130">Read-only.</span></span> <span data-ttu-id="8a9bb-131">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-131">Nullable.</span></span>|
|<span data-ttu-id="8a9bb-132">资源</span><span class="sxs-lookup"><span data-stu-id="8a9bb-132">resources</span></span>|<span data-ttu-id="8a9bb-133">[onenoteResource](onenoteresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-133">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="8a9bb-134">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="8a9bb-135">不支持获取资源集合, 但可以[获取特定资源的二进制内容](onenoteresource.md)。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="8a9bb-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-136">Read-only.</span></span> <span data-ttu-id="8a9bb-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-137">Nullable.</span></span>|
|<span data-ttu-id="8a9bb-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="8a9bb-138">sectionGroups</span></span>|<span data-ttu-id="8a9bb-139">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-139">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="8a9bb-140">由用户或组拥有的所有 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="8a9bb-141">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-141">Read-only.</span></span> <span data-ttu-id="8a9bb-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-142">Nullable.</span></span>|
|<span data-ttu-id="8a9bb-143">分区</span><span class="sxs-lookup"><span data-stu-id="8a9bb-143">sections</span></span>|<span data-ttu-id="8a9bb-144">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-144">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="8a9bb-145">所有 OneNote 笔记本中由用户或组所有的部分。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="8a9bb-146">只读。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-146">Read-only.</span></span> <span data-ttu-id="8a9bb-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="8a9bb-148">方法</span><span class="sxs-lookup"><span data-stu-id="8a9bb-148">Methods</span></span>

| <span data-ttu-id="8a9bb-149">方法</span><span class="sxs-lookup"><span data-stu-id="8a9bb-149">Method</span></span>           | <span data-ttu-id="8a9bb-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a9bb-150">Return Type</span></span>    |<span data-ttu-id="8a9bb-151">说明</span><span class="sxs-lookup"><span data-stu-id="8a9bb-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a9bb-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="8a9bb-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="8a9bb-153">笔记</span><span class="sxs-lookup"><span data-stu-id="8a9bb-153">notebook</span></span>](notebook.md)| <span data-ttu-id="8a9bb-154">通过发布到 "笔记本" 集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="8a9bb-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="8a9bb-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="8a9bb-156">[notebook](notebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-156">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="8a9bb-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="8a9bb-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="8a9bb-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="8a9bb-159">onenotePage</span><span class="sxs-lookup"><span data-stu-id="8a9bb-159">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="8a9bb-160">通过发布到 pages 集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="8a9bb-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="8a9bb-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="8a9bb-162">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-162">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="8a9bb-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="8a9bb-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="8a9bb-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="8a9bb-165">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-165">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="8a9bb-166">获取节组的集合。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="8a9bb-167">列出分区</span><span class="sxs-lookup"><span data-stu-id="8a9bb-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="8a9bb-168">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a9bb-168">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="8a9bb-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="8a9bb-169">Get a collection of sections.</span></span>|
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
