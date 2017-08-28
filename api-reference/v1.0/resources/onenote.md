# <a name="onenote-resource-type"></a><span data-ttu-id="cc041-101">Onenote 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc041-101">onenote resource type</span></span>

<span data-ttu-id="cc041-102">适用于 Onenote 资源的入口点。</span><span class="sxs-lookup"><span data-stu-id="cc041-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="cc041-103">所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="cc041-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="cc041-104">位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。</span><span class="sxs-lookup"><span data-stu-id="cc041-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="cc041-105">**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：</span><span class="sxs-lookup"><span data-stu-id="cc041-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="cc041-106">**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="cc041-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="cc041-107">**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：</span><span class="sxs-lookup"><span data-stu-id="cc041-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="cc041-108">授权</span><span class="sxs-lookup"><span data-stu-id="cc041-108">Authorization</span></span>

<span data-ttu-id="cc041-109">有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="cc041-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="cc041-110">关系</span><span class="sxs-lookup"><span data-stu-id="cc041-110">Relationships</span></span>
| <span data-ttu-id="cc041-111">关系</span><span class="sxs-lookup"><span data-stu-id="cc041-111">Relationship</span></span> | <span data-ttu-id="cc041-112">类型</span><span class="sxs-lookup"><span data-stu-id="cc041-112">Type</span></span>   |<span data-ttu-id="cc041-113">说明</span><span class="sxs-lookup"><span data-stu-id="cc041-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc041-114">笔记本</span><span class="sxs-lookup"><span data-stu-id="cc041-114">notebooks</span></span>|<span data-ttu-id="cc041-115">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="cc041-p101">用户或组所有的 OneNote 笔记本集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc041-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cc041-119">操作</span><span class="sxs-lookup"><span data-stu-id="cc041-119">operations</span></span>|<span data-ttu-id="cc041-120">[操作](onenoteoperation.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-120">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="cc041-p102">OneNote 操作状态。不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc041-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cc041-125">页面</span><span class="sxs-lookup"><span data-stu-id="cc041-125">pages</span></span>|<span data-ttu-id="cc041-126">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-126">[Page](page.md) collection</span></span>|<span data-ttu-id="cc041-p103">用户或组所有的全部 OneNote 笔记本中的页面。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc041-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="cc041-130">资源</span><span class="sxs-lookup"><span data-stu-id="cc041-130">resources</span></span>|<span data-ttu-id="cc041-131">[资源](resource.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-131">[Resource](resource.md) collection</span></span> |<span data-ttu-id="cc041-p104">OneNote 页面中的图像和其他文件资源。不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc041-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="cc041-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="cc041-136">sectionGroups</span></span>|<span data-ttu-id="cc041-137">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc041-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="cc041-p105">用户或组所有的全部 OneNote 笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc041-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="cc041-141">节</span><span class="sxs-lookup"><span data-stu-id="cc041-141">sections</span></span>|<span data-ttu-id="cc041-142">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-142">[Section](section.md) collection</span></span>|<span data-ttu-id="cc041-p106">用户或组所有的全部 OneNote 笔记本中的节。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc041-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="cc041-146">方法</span><span class="sxs-lookup"><span data-stu-id="cc041-146">Methods</span></span>

| <span data-ttu-id="cc041-147">方法</span><span class="sxs-lookup"><span data-stu-id="cc041-147">Method</span></span>           | <span data-ttu-id="cc041-148">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc041-148">Return Type</span></span>    |<span data-ttu-id="cc041-149">说明</span><span class="sxs-lookup"><span data-stu-id="cc041-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc041-150">创建笔记本</span><span class="sxs-lookup"><span data-stu-id="cc041-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="cc041-151">笔记本</span><span class="sxs-lookup"><span data-stu-id="cc041-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="cc041-152">通过发布到笔记本集合创建笔记本。</span><span class="sxs-lookup"><span data-stu-id="cc041-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="cc041-153">列出笔记本</span><span class="sxs-lookup"><span data-stu-id="cc041-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="cc041-154">[笔记本](notebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="cc041-155">获取笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="cc041-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="cc041-156">创建页面</span><span class="sxs-lookup"><span data-stu-id="cc041-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="cc041-157">页面</span><span class="sxs-lookup"><span data-stu-id="cc041-157">Page</span></span>](page.md)| <span data-ttu-id="cc041-158">通过发布到页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="cc041-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="cc041-159">列出页面</span><span class="sxs-lookup"><span data-stu-id="cc041-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="cc041-160">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-160">[Page](page.md) collection</span></span>| <span data-ttu-id="cc041-161">获取页面的集合。</span><span class="sxs-lookup"><span data-stu-id="cc041-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="cc041-162">列出分区组</span><span class="sxs-lookup"><span data-stu-id="cc041-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="cc041-163">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc041-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="cc041-164">获取分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="cc041-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="cc041-165">列出节</span><span class="sxs-lookup"><span data-stu-id="cc041-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="cc041-166">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc041-166">[Section](section.md) collection</span></span>| <span data-ttu-id="cc041-167">获取节的集合。</span><span class="sxs-lookup"><span data-stu-id="cc041-167">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
