---
title: Onenote 资源类型
description: 适用于 Onenote 资源的入口点。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 8240336bfcb9e45e33172c2c1551b71a65c315e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462800"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="fbe2e-103">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbe2e-103">onenote resource type</span></span>

<span data-ttu-id="fbe2e-104">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="fbe2e-105">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fbe2e-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="fbe2e-106">位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="fbe2e-107">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="fbe2e-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="fbe2e-108">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fbe2e-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="fbe2e-109">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="fbe2e-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="fbe2e-110">授权</span><span class="sxs-lookup"><span data-stu-id="fbe2e-110">Authorization</span></span>

<span data-ttu-id="fbe2e-111">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](/graph/permissions-reference#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="fbe2e-112">关系</span><span class="sxs-lookup"><span data-stu-id="fbe2e-112">Relationships</span></span>
| <span data-ttu-id="fbe2e-113">关系</span><span class="sxs-lookup"><span data-stu-id="fbe2e-113">Relationship</span></span> | <span data-ttu-id="fbe2e-114">类型</span><span class="sxs-lookup"><span data-stu-id="fbe2e-114">Type</span></span>   |<span data-ttu-id="fbe2e-115">说明</span><span class="sxs-lookup"><span data-stu-id="fbe2e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbe2e-116">笔记本</span><span class="sxs-lookup"><span data-stu-id="fbe2e-116">notebooks</span></span>|<span data-ttu-id="fbe2e-117">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-117">Notebook collection</span></span>|<span data-ttu-id="fbe2e-118">用户或组所有的 OneNote 笔记本集合。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="fbe2e-119">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-119">Read-only.</span></span> <span data-ttu-id="fbe2e-120">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-120">Nullable.</span></span>|
|<span data-ttu-id="fbe2e-121">operations</span><span class="sxs-lookup"><span data-stu-id="fbe2e-121">operations</span></span>|<span data-ttu-id="fbe2e-122">[OnenoteOperation](onenoteoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="fbe2e-123">OneNote 操作状态。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-123">The status of OneNote operations.</span></span> <span data-ttu-id="fbe2e-124">不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="fbe2e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-125">Read-only.</span></span> <span data-ttu-id="fbe2e-126">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-126">Nullable.</span></span>|
|<span data-ttu-id="fbe2e-127">pages</span><span class="sxs-lookup"><span data-stu-id="fbe2e-127">pages</span></span>|<span data-ttu-id="fbe2e-128">[OnenotePage](page.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="fbe2e-129">用户或组所有的全部 OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fbe2e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-130">Read-only.</span></span> <span data-ttu-id="fbe2e-131">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-131">Nullable.</span></span>|
|<span data-ttu-id="fbe2e-132">resources</span><span class="sxs-lookup"><span data-stu-id="fbe2e-132">resources</span></span>|<span data-ttu-id="fbe2e-133">[OnenoteResource](resource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="fbe2e-134">OneNote 页面中的图像和其他文件资源。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="fbe2e-135">不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="fbe2e-136">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-136">Read-only.</span></span> <span data-ttu-id="fbe2e-137">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-137">Nullable.</span></span>|
|<span data-ttu-id="fbe2e-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="fbe2e-138">sectionGroups</span></span>|<span data-ttu-id="fbe2e-139">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-139">SectionGroup collection</span></span>|<span data-ttu-id="fbe2e-140">用户或组所有的全部 OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fbe2e-141">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-141">Read-only.</span></span> <span data-ttu-id="fbe2e-142">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-142">Nullable.</span></span>|
|<span data-ttu-id="fbe2e-143">sections</span><span class="sxs-lookup"><span data-stu-id="fbe2e-143">sections</span></span>|<span data-ttu-id="fbe2e-144">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="fbe2e-145">用户或组所有的全部 OneNote 笔记本中的节。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="fbe2e-146">只读。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-146">Read-only.</span></span> <span data-ttu-id="fbe2e-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="fbe2e-148">方法</span><span class="sxs-lookup"><span data-stu-id="fbe2e-148">Methods</span></span>

| <span data-ttu-id="fbe2e-149">方法</span><span class="sxs-lookup"><span data-stu-id="fbe2e-149">Method</span></span>           | <span data-ttu-id="fbe2e-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbe2e-150">Return Type</span></span>    |<span data-ttu-id="fbe2e-151">说明</span><span class="sxs-lookup"><span data-stu-id="fbe2e-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbe2e-152">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="fbe2e-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="fbe2e-153">笔记本</span><span class="sxs-lookup"><span data-stu-id="fbe2e-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="fbe2e-154">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-154">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="fbe2e-155">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="fbe2e-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="fbe2e-156">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-156">Notebook collection</span></span>| <span data-ttu-id="fbe2e-157">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-157">Represents a collection of notebooks.</span></span>|
|[<span data-ttu-id="fbe2e-158">创建页面</span><span class="sxs-lookup"><span data-stu-id="fbe2e-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="fbe2e-159">页面</span><span class="sxs-lookup"><span data-stu-id="fbe2e-159">Page</span></span>](page.md)| <span data-ttu-id="fbe2e-160">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-160">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="fbe2e-161">列出页面</span><span class="sxs-lookup"><span data-stu-id="fbe2e-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="fbe2e-162">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-162">Page collection</span></span>| <span data-ttu-id="fbe2e-163">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-163">Represents a collection of pages.</span></span>|
|[<span data-ttu-id="fbe2e-164">列出分区组</span><span class="sxs-lookup"><span data-stu-id="fbe2e-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="fbe2e-165">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-165">SectionGroup collection</span></span>| <span data-ttu-id="fbe2e-166">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-166">Represents a collection of section groups.</span></span>|
|[<span data-ttu-id="fbe2e-167">列出节</span><span class="sxs-lookup"><span data-stu-id="fbe2e-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="fbe2e-168">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbe2e-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="fbe2e-169">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-169">Represents a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fbe2e-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbe2e-170">JSON Representation</span></span>
<span data-ttu-id="fbe2e-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbe2e-171">Here is a JSON representation of the resource.</span></span>
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
