---
title: 使用 Microsoft Graph 获取 OneNote 内容和结构
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: f3e40662d2e750514ef6c71b3faa604e13ccc773
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921656"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="69e6a-103">使用 Microsoft Graph 获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="69e6a-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="69e6a-104">**适用于**：OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="69e6a-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="69e6a-105">若要获取 OneNote 内容和结构，请向目标终结点发送 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="69e6a-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="69e6a-106">例如：</span><span class="sxs-lookup"><span data-stu-id="69e6a-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="69e6a-107">如果请求成功，Microsoft Graph 将返回一个 200 HTTP 状态代码以及请求的实体或内容。</span><span class="sxs-lookup"><span data-stu-id="69e6a-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="69e6a-108">OneNote 实体作为符合 OData 版本 4.0 规范的 JSON 对象返回。</span><span class="sxs-lookup"><span data-stu-id="69e6a-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="69e6a-109">通过使用查询字符串选项，可以筛选查询并提高性能。</span><span class="sxs-lookup"><span data-stu-id="69e6a-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="69e6a-110">构建请求 URI</span><span class="sxs-lookup"><span data-stu-id="69e6a-110">Construct the request URI</span></span>

<span data-ttu-id="69e6a-111">若要构建请求 URI，请从服务根 URL 开始：</span><span class="sxs-lookup"><span data-stu-id="69e6a-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="69e6a-112">然后追加要检索的资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="69e6a-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="69e6a-113">（[资源路径](#resource-paths-for-get-requests)会显示在下一个节中。）</span><span class="sxs-lookup"><span data-stu-id="69e6a-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="69e6a-114">完整的请求 URI 类似于以下示例之一：</span><span class="sxs-lookup"><span data-stu-id="69e6a-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="69e6a-115">**注意：** 了解有关 [服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="69e6a-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="69e6a-116">GET 请求的资源路径</span><span class="sxs-lookup"><span data-stu-id="69e6a-116">Resource paths for GET requests</span></span>

<span data-ttu-id="69e6a-117">使用以下资源路径获取页面、节、节组、笔记本和图像或文件资源。</span><span class="sxs-lookup"><span data-stu-id="69e6a-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="69e6a-118">页面集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="69e6a-119">页面实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="69e6a-120">页面预览</span><span class="sxs-lookup"><span data-stu-id="69e6a-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="69e6a-121">页面 HTML 内容</span><span class="sxs-lookup"><span data-stu-id="69e6a-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="69e6a-122">节集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="69e6a-123">节实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="69e6a-124">SectionGroup 集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="69e6a-125">SectionGroup 实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="69e6a-126">笔记本集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="69e6a-127">笔记本实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="69e6a-128">图像或其他文件资源</span><span class="sxs-lookup"><span data-stu-id="69e6a-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="69e6a-129">页面集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-129">Page collection</span></span>

<span data-ttu-id="69e6a-130">获取所有笔记本的页面（元数据）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="69e6a-131">从特定节获取页面（元数据）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="69e6a-132">`search` 查询字符串选项仅适用于消费者笔记本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="69e6a-133">页面的默认排序顺序是 `lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="69e6a-134">默认查询将展开父节并选择节的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="69e6a-135">默认情况下，为 *GET 页面* 请求返回仅前 20 个实体。</span><span class="sxs-lookup"><span data-stu-id="69e6a-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="69e6a-136">未指定 **top** 查询字符串选项的请求将在响应中返回 `@odata.nextLink` 链接，该链接可用于获取接下来的 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="69e6a-137">对于节中的页面集合，使用 **pagelevel** 返回页面的缩进级别及其在节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="69e6a-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="69e6a-138">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="69e6a-139">页面实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-139">Page entity</span></span>

<span data-ttu-id="69e6a-140">获取特定页面的元数据。</span><span class="sxs-lookup"><span data-stu-id="69e6a-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="69e6a-141">页面可以展开 **parentNotebook** 和 **parentSection** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="69e6a-142">默认查询将展开父节并选择节的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="69e6a-143">使用 **pagelevel** 返回页面的缩进级别及其在父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="69e6a-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="69e6a-144">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="69e6a-145">页面预览</span><span class="sxs-lookup"><span data-stu-id="69e6a-145">Page preview</span></span>

<span data-ttu-id="69e6a-146">获取页面的文字和图像预览内容。</span><span class="sxs-lookup"><span data-stu-id="69e6a-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="69e6a-147">JSON 响应包含预览内容，可用于帮助用户标识页面中的内容。</span><span class="sxs-lookup"><span data-stu-id="69e6a-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

<span data-ttu-id="69e6a-148">**previewText** 属性包含来自页面的文本片段。</span><span class="sxs-lookup"><span data-stu-id="69e6a-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="69e6a-149">Microsoft Graph 返回完整短语，最多 300 个字符。</span><span class="sxs-lookup"><span data-stu-id="69e6a-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="69e6a-150">如果页面包含可用于生成预览 UI 的图像，则 **previewImageUrl** 对象中的 **href** 属性包含指向公共 [图像资源](#image-or-other-file-resource)的链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="69e6a-151">可以在 HTML 中使用此链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-151">You can use this link in HTML.</span></span> <span data-ttu-id="69e6a-152">否则，**href** 返回 null。</span><span class="sxs-lookup"><span data-stu-id="69e6a-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="69e6a-153">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="69e6a-154">页面 HTML 内容</span><span class="sxs-lookup"><span data-stu-id="69e6a-154">Page HTML content</span></span>

<span data-ttu-id="69e6a-155">获取页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="69e6a-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs]`

<span data-ttu-id="69e6a-156">（*了解有关 [返回的 HTML 内容](onenote-input-output-html.md)* 的详细信息）</span><span class="sxs-lookup"><span data-stu-id="69e6a-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="69e6a-157">使用 **includeIDs=true** 查询字符串选项获取生成的 ID，用于 [更新页面](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="69e6a-158">节集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-158">Section collection</span></span>

<span data-ttu-id="69e6a-159">获取用户拥有的所有笔记本的所有节，包括嵌套节组中的节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-160">获取直接位于特定节组下的所有节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-160">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-161">获取直接位于特定笔记本下的所有节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-161">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-162">节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="69e6a-163">节的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="69e6a-164">默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="69e6a-165">节实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-165">Section entity</span></span>

<span data-ttu-id="69e6a-166">获取特定节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-166">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="69e6a-167">节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="69e6a-168">默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="69e6a-169">SectionGroup 集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-169">SectionGroup collection</span></span>

<span data-ttu-id="69e6a-170">获取用户拥有的所有笔记本的所有节组，包括嵌套节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-170">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-171">获取直接位于特定笔记本下的所有节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-171">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-172">节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="69e6a-173">节组的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="69e6a-174">默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="69e6a-175">SectionGroup 实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-175">SectionGroup entity</span></span>

<span data-ttu-id="69e6a-176">获取特定节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-176">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="69e6a-177">节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="69e6a-178">默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="69e6a-179">笔记本集合</span><span class="sxs-lookup"><span data-stu-id="69e6a-179">Notebook collection</span></span>

<span data-ttu-id="69e6a-180">获取用户拥有的所有笔记本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-180">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="69e6a-181">笔记本可以展开 **sections** 和 **sectionGroups** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="69e6a-182">笔记本的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="69e6a-183">笔记本实体</span><span class="sxs-lookup"><span data-stu-id="69e6a-183">Notebook entity</span></span>

<span data-ttu-id="69e6a-184">获取特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="69e6a-185">笔记本可以展开 **sections** 和 **sectionGroups** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="69e6a-186">图像或其他文件资源</span><span class="sxs-lookup"><span data-stu-id="69e6a-186">Image or other file resource</span></span>

<span data-ttu-id="69e6a-187">获取特定资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="69e6a-187">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="69e6a-188">可以在页面的[输出 HTML](onenote-input-output-html.md) 中找到文件的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="69e6a-188">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="69e6a-189">例如，**img** 标记包含 **data-fullres-src** 属性中原始图像的终结点和 **src** 属性中经优化图像的终结点。</span><span class="sxs-lookup"><span data-stu-id="69e6a-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="69e6a-190">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="69e6a-191">**object** 标记包含 **data** 属性中文件资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="69e6a-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="69e6a-192">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-192">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> <span data-ttu-id="69e6a-193">**注意：** 不支持获取资源的集合。</span><span class="sxs-lookup"><span data-stu-id="69e6a-193">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="69e6a-194">在获取文件资源时，无需在请求中包含 **Accept** 内容类型。</span><span class="sxs-lookup"><span data-stu-id="69e6a-194">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="69e6a-195">有关 GET 请求的详细信息，请参阅 Microsoft Graph API REST 引用中的以下资源：</span><span class="sxs-lookup"><span data-stu-id="69e6a-195">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="69e6a-196">GET 页面</span><span class="sxs-lookup"><span data-stu-id="69e6a-196">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-197">GET 节</span><span class="sxs-lookup"><span data-stu-id="69e6a-197">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-198">GET 节组</span><span class="sxs-lookup"><span data-stu-id="69e6a-198">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-199">GET 笔记本</span><span class="sxs-lookup"><span data-stu-id="69e6a-199">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="69e6a-200">示例 GET 请求</span><span class="sxs-lookup"><span data-stu-id="69e6a-200">Example GET requests</span></span>

<span data-ttu-id="69e6a-201">可以查询 OneNote 实体和搜索页面内容以仅获取所需的信息。</span><span class="sxs-lookup"><span data-stu-id="69e6a-201">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="69e6a-202">以下示例演示了一些方法，可以在对 Microsoft Graph 的 GET 请求中使用[支持的查询字符串选项](#supported-odata-query-string-options)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-202">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="69e6a-203">**请注意：**</span><span class="sxs-lookup"><span data-stu-id="69e6a-203">**Remember:**</span></span>

- <span data-ttu-id="69e6a-204">所有的 GET 请求都以[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 开头。</span><span class="sxs-lookup"><span data-stu-id="69e6a-204">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="69e6a-205">**示例**：`https://www.onenote.com/api/v1.0/me/notes` 和 `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="69e6a-205">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="69e6a-206">URL 查询字符串中的空格必须使用 %20 编码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-206">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="69e6a-207">**示例**：`filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="69e6a-207">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="69e6a-208">属性名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-208">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="69e6a-209">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="69e6a-209">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="69e6a-210">**示例**：`filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="69e6a-210">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="69e6a-211">search & filter</span><span class="sxs-lookup"><span data-stu-id="69e6a-211">search & filter</span></span>  

<span data-ttu-id="69e6a-212">获取包含由特定应用创建的术语 *recipe* 的所有页面（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-212">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="69e6a-213">search & select</span><span class="sxs-lookup"><span data-stu-id="69e6a-213">search & select</span></span>  

<span data-ttu-id="69e6a-214">获取包含术语 *golgi app* 的所有页面的标题、OneNote 客户端链接和 **contentUrl** 链接（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-214">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="69e6a-215">expand</span><span class="sxs-lookup"><span data-stu-id="69e6a-215">expand</span></span> 

<span data-ttu-id="69e6a-216">获取所有笔记本，并展开它的节和节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-216">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="69e6a-217">获取某个特定的节组，并展开它的节和节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-217">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="69e6a-218">获取一个页面并展开其父节和父笔记本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-218">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="69e6a-219">expand（多个级别）</span><span class="sxs-lookup"><span data-stu-id="69e6a-219">expand (multiple levels)</span></span>  

<span data-ttu-id="69e6a-220">获取所有笔记本，展开其节和节组，并在每个节组中展开所有节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-220">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="69e6a-221">**注意：** 展开子实体的父项或展开父实体的子项来创建循环引用，这并不受支持。</span><span class="sxs-lookup"><span data-stu-id="69e6a-221">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="69e6a-222">expand & select（多个级别）</span><span class="sxs-lookup"><span data-stu-id="69e6a-222">expand & select (multiple levels)</span></span>  

<span data-ttu-id="69e6a-223">获取特定节组的名称和 **self** 链接，并获取其所有节的名称和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-223">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="69e6a-224">获取所有节的名称和 **self** 链接，并获取每个节的父笔记本的名称和创建时间。</span><span class="sxs-lookup"><span data-stu-id="69e6a-224">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="69e6a-225">获取所有页面的标题和 ID，并获取父节和父笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="69e6a-225">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="69e6a-226">expand & levels（多个级别）</span><span class="sxs-lookup"><span data-stu-id="69e6a-226">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="69e6a-227">获取所有笔记本、节和节组。</span><span class="sxs-lookup"><span data-stu-id="69e6a-227">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="69e6a-228">filter</span><span class="sxs-lookup"><span data-stu-id="69e6a-228">filter</span></span>

<span data-ttu-id="69e6a-229">获取 2014 年 10 月创建的所有节。</span><span class="sxs-lookup"><span data-stu-id="69e6a-229">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="69e6a-230">获取某个特定应用自 2015 年 1 月 1 日以来所创建的页面。</span><span class="sxs-lookup"><span data-stu-id="69e6a-230">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="69e6a-231">filter & expand</span><span class="sxs-lookup"><span data-stu-id="69e6a-231">filter & expand</span></span>  

<span data-ttu-id="69e6a-232">获取特定笔记本中的所有页面。</span><span class="sxs-lookup"><span data-stu-id="69e6a-232">Get all pages in a specific notebook.</span></span> <span data-ttu-id="69e6a-233">默认情况下，API 返回 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-233">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="69e6a-234">获取 *School* 笔记本的所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-234">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="69e6a-235">OData 字符串比较区分大小写，因此，作为最佳做法将使用 **tolower** 函数。</span><span class="sxs-lookup"><span data-stu-id="69e6a-235">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="69e6a-236">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="69e6a-236">filter & select & orderby</span></span>   

<span data-ttu-id="69e6a-237">获取在节名中包含术语 *spring* 的所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-237">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="69e6a-238">按照最后修改日期对节进行排序。</span><span class="sxs-lookup"><span data-stu-id="69e6a-238">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="69e6a-239">orderby</span><span class="sxs-lookup"><span data-stu-id="69e6a-239">orderby</span></span>

<span data-ttu-id="69e6a-240">获取先按照 **createdByAppId** 属性排序再按照最近创建时间排序的前 20 个页面。</span><span class="sxs-lookup"><span data-stu-id="69e6a-240">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="69e6a-241">默认情况下，API 返回 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-241">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="69e6a-242">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="69e6a-242">search & filter & top</span></span> 

<span data-ttu-id="69e6a-243">获取自 2015 年 1 月 1 日以来创建的包含短语 *cell division* 的 5 个最新页面。</span><span class="sxs-lookup"><span data-stu-id="69e6a-243">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="69e6a-244">默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-244">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="69e6a-245">页面的默认排序顺序为 `lastModifiedTime desc`（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-245">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="69e6a-246">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="69e6a-246">search & filter & top & skip</span></span>  

<span data-ttu-id="69e6a-247">获取结果集中接下来的五个页面（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-247">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="69e6a-248">以及接下来的五页（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-248">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="69e6a-249">**注意：** 如果 **search** 和 **filter** 都应用于同一请求，则结果只包含与这两个条件都匹配的实体。</span><span class="sxs-lookup"><span data-stu-id="69e6a-249">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="69e6a-250">select</span><span class="sxs-lookup"><span data-stu-id="69e6a-250">select</span></span>

<span data-ttu-id="69e6a-251">获取用户笔记本中所有节的名称、创建时间和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-251">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="69e6a-252">获取特定页面的标题、创建时间和 OneNote 客户端链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-252">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="69e6a-253">select & expand & filter（多个级别）</span><span class="sxs-lookup"><span data-stu-id="69e6a-253">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="69e6a-254">获取用户的默认笔记本中所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-254">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="69e6a-255">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="69e6a-255">top & select & orderby</span></span> 

<span data-ttu-id="69e6a-256">获取按标题字母顺序排序的前 50 个页面的标题和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="69e6a-256">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="69e6a-257">默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-257">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="69e6a-258">页面的默认排序顺序是 `lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-258">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="69e6a-259">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="69e6a-259">skip & top & select & orderby</span></span>  

<span data-ttu-id="69e6a-p115">获取第 51 至 100 页。默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-p115">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="69e6a-262">**注意：** 检索条目默认数量（即，它们不指定 **top** 表达式）的页面的 GET 请求在响应中将返回一个 **\@odata.nextLink** 链接，你可使用此链接获取接下来的 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-262">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **\@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="69e6a-263">受支持的 OData 查询字符串选项</span><span class="sxs-lookup"><span data-stu-id="69e6a-263">Supported OData query string options</span></span>

<span data-ttu-id="69e6a-264">向 Microsoft Graph 发送 GET 请求时，可以使用 OData 查询字符串选项来自定义查询并仅获取所需的信息。</span><span class="sxs-lookup"><span data-stu-id="69e6a-264">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="69e6a-265">它们可以通过减少对该服务的调用数量以及响应有效负载的大小来提高性能。</span><span class="sxs-lookup"><span data-stu-id="69e6a-265">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="69e6a-266">**注意：** 为了增强可读性，本文中的示例不使用 URL 查询字符串中空格所需的 %20 百分比编码：`filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="69e6a-266">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="69e6a-267">查询选项</span><span class="sxs-lookup"><span data-stu-id="69e6a-267">Query option</span></span> | <span data-ttu-id="69e6a-268">示例和说明</span><span class="sxs-lookup"><span data-stu-id="69e6a-268">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="69e6a-269">count</span><span class="sxs-lookup"><span data-stu-id="69e6a-269">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="69e6a-p117">集合中的实体计数。在响应的 **\@odata.count** 属性中返回此值。</span><span class="sxs-lookup"><span data-stu-id="69e6a-p117">The count of entities in the collection. The value is returned in the **\@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="69e6a-272">expand</span><span class="sxs-lookup"><span data-stu-id="69e6a-272">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="69e6a-273">要在响应中返回内联的导航属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-273">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="69e6a-274">**expand** 表达式支持以下属性：</span><span class="sxs-lookup"><span data-stu-id="69e6a-274">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="69e6a-275">- 页面：**parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="69e6a-275">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="69e6a-276">- 节：**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="69e6a-276">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="69e6a-277">- 节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="69e6a-277">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="69e6a-278">- 笔记本：**sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="69e6a-278">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="69e6a-p119">默认情况下，页面的 GET 请求同时展开 **parentSection** 并选择该节的 **id**、**name** 和 **self** 属性。节和节组的默认 GET 请求扩展 **parentNotebook** 和 **parentSectionGroup**，并选择父项的 **id**、**name** 和 **self** 属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-p119">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="69e6a-281">可用于单个实体或集合。</span><span class="sxs-lookup"><span data-stu-id="69e6a-281">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="69e6a-282">使用逗号分隔多个属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-282">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="69e6a-283">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-283">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="69e6a-284">filter</span><span class="sxs-lookup"><span data-stu-id="69e6a-284">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="69e6a-285">是否在结果集中包含条目的布尔表达式。</span><span class="sxs-lookup"><span data-stu-id="69e6a-285">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="69e6a-286">支持以下 OData 运算符和函数：</span><span class="sxs-lookup"><span data-stu-id="69e6a-286">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="69e6a-287">- 比较运算符：**eq**、**ne**、**gt**、**ge**、**lt**、**le**</span><span class="sxs-lookup"><span data-stu-id="69e6a-287">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="69e6a-288">- 逻辑运算符：**and**、**or**、**not**</span><span class="sxs-lookup"><span data-stu-id="69e6a-288">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="69e6a-289">- 字符串函数：**contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</span><span class="sxs-lookup"><span data-stu-id="69e6a-289">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="69e6a-290">[属性](#onenote-entity-properties)名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-290">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="69e6a-291">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="69e6a-291">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="69e6a-292">**示例**：`filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="69e6a-292">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="69e6a-293">orderby</span><span class="sxs-lookup"><span data-stu-id="69e6a-293">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="69e6a-p122">作为排序依据的 [属性](#onenote-entity-properties)，具有可选的 **asc**（默认）或 **desc** 的排序顺序。您可以按请求集合中实体的任意属性进行排序。</span><span class="sxs-lookup"><span data-stu-id="69e6a-p122">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="69e6a-296">笔记本、节组和节的默认排序顺序为 `name asc`，页面的默认排序顺序为 `lastModifiedTime desc`（最后修改的页面排第一）。</span><span class="sxs-lookup"><span data-stu-id="69e6a-296">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="69e6a-297">用逗号隔开多个属性，并按想要应用属性的顺序列出它们。</span><span class="sxs-lookup"><span data-stu-id="69e6a-297">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="69e6a-298">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-298">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="69e6a-299">search</span><span class="sxs-lookup"><span data-stu-id="69e6a-299">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="69e6a-300">仅适用于消费者笔记本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-300">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="69e6a-p124">要在页面标题、页面正文、图像替换文字、图像 OCR 文本中搜索的术语或短语。默认情况下，搜索查询返回按相关性排序的结果。</span><span class="sxs-lookup"><span data-stu-id="69e6a-p124">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="69e6a-303">OneNote 使用必应全文搜索来支持短语搜索、词干分解、拼写宽容、相关性和排名、断字、多语言以及其他全文搜索功能。</span><span class="sxs-lookup"><span data-stu-id="69e6a-303">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="69e6a-304">搜索字符串不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-304">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="69e6a-305">仅适用于用户拥有的笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="69e6a-305">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="69e6a-306">已编入索引的内容具有私密性，只有所有者才能访问。</span><span class="sxs-lookup"><span data-stu-id="69e6a-306">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="69e6a-307">受密码保护的页面未编入索引。</span><span class="sxs-lookup"><span data-stu-id="69e6a-307">Password-protected pages are not indexed.</span></span> <span data-ttu-id="69e6a-308">仅适用于 `pages` 终结点。</span><span class="sxs-lookup"><span data-stu-id="69e6a-308">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="69e6a-309">select</span><span class="sxs-lookup"><span data-stu-id="69e6a-309">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="69e6a-310">要返回的[属性](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-310">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="69e6a-311">可用于单个实体或集合。</span><span class="sxs-lookup"><span data-stu-id="69e6a-311">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="69e6a-312">使用逗号分隔多个属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-312">Separate multiple properties with commas.</span></span> <span data-ttu-id="69e6a-313">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-313">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="69e6a-314">skip</span><span class="sxs-lookup"><span data-stu-id="69e6a-314">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="69e6a-315">结果集中要跳过的条目数量。</span><span class="sxs-lookup"><span data-stu-id="69e6a-315">The number of entries to skip in the result set.</span></span> <span data-ttu-id="69e6a-316">通常用于对结果分页。</span><span class="sxs-lookup"><span data-stu-id="69e6a-316">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="69e6a-317">top</span><span class="sxs-lookup"><span data-stu-id="69e6a-317">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="69e6a-318">结果集中要返回的条目数量，最多可达 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="69e6a-318">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="69e6a-319">默认值为 20。</span><span class="sxs-lookup"><span data-stu-id="69e6a-319">The default value is 20.</span></span></p> |  

<span data-ttu-id="69e6a-320">Microsoft Graph 还提供 `pagelevel` 查询字符串选项，可使用该选项获取父节内页面的级别和顺序。</span><span class="sxs-lookup"><span data-stu-id="69e6a-320">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="69e6a-321">仅适用于特定节中页面的查询或特定页面中的查询。</span><span class="sxs-lookup"><span data-stu-id="69e6a-321">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="69e6a-322">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-322">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="69e6a-323">受支持的 OData 运算符和函数</span><span class="sxs-lookup"><span data-stu-id="69e6a-323">Supported OData operators and functions</span></span>

<span data-ttu-id="69e6a-324">Microsoft Graph 支持 **filter** 表达式中的以下 OData 运算符和函数。</span><span class="sxs-lookup"><span data-stu-id="69e6a-324">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="69e6a-325">使用 OData 表达式时，请记住：</span><span class="sxs-lookup"><span data-stu-id="69e6a-325">When using OData expressions, remember:</span></span>

- <span data-ttu-id="69e6a-326">必须将 URL 查询字符串中的空格替换为 `%20` 编码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-326">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="69e6a-327">**示例：** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="69e6a-327">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="69e6a-328">属性名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-328">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="69e6a-329">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="69e6a-329">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="69e6a-330">**示例：** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="69e6a-330">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="69e6a-331">比较运算符</span><span class="sxs-lookup"><span data-stu-id="69e6a-331">Comparison operator</span></span> | <span data-ttu-id="69e6a-332">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-332">Example</span></span> |  
|------|------|  
| <span data-ttu-id="69e6a-333">eq</span><span class="sxs-lookup"><span data-stu-id="69e6a-333">eq</span></span><br /><span data-ttu-id="69e6a-334">（等于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-334">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="69e6a-335">ne</span><span class="sxs-lookup"><span data-stu-id="69e6a-335">ne</span></span><br /><span data-ttu-id="69e6a-336">（不等于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-336">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="69e6a-337">gt</span><span class="sxs-lookup"><span data-stu-id="69e6a-337">gt</span></span><br /><span data-ttu-id="69e6a-338">（大于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-338">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="69e6a-339">ge</span><span class="sxs-lookup"><span data-stu-id="69e6a-339">ge</span></span><br /><span data-ttu-id="69e6a-340">（大于或等于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-340">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="69e6a-341">lt</span><span class="sxs-lookup"><span data-stu-id="69e6a-341">lt</span></span><br /><span data-ttu-id="69e6a-342">（小于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-342">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="69e6a-343">le</span><span class="sxs-lookup"><span data-stu-id="69e6a-343">le</span></span><br /><span data-ttu-id="69e6a-344">（小于或等于）</span><span class="sxs-lookup"><span data-stu-id="69e6a-344">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="69e6a-345">逻辑运算符</span><span class="sxs-lookup"><span data-stu-id="69e6a-345">Logical operator</span></span> | <span data-ttu-id="69e6a-346">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-346">Example</span></span> |  
|------|------|  
| <span data-ttu-id="69e6a-347">和</span><span class="sxs-lookup"><span data-stu-id="69e6a-347">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="69e6a-348">或</span><span class="sxs-lookup"><span data-stu-id="69e6a-348">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="69e6a-349">
not</span><span class="sxs-lookup"><span data-stu-id="69e6a-349">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="69e6a-350">字符串函数</span><span class="sxs-lookup"><span data-stu-id="69e6a-350">String function</span></span> | <span data-ttu-id="69e6a-351">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-351">Example</span></span> |  
|------|------|   
| <span data-ttu-id="69e6a-352">contains</span><span class="sxs-lookup"><span data-stu-id="69e6a-352">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="69e6a-353">endswith</span><span class="sxs-lookup"><span data-stu-id="69e6a-353">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="69e6a-354">startswith</span><span class="sxs-lookup"><span data-stu-id="69e6a-354">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="69e6a-355">length</span><span class="sxs-lookup"><span data-stu-id="69e6a-355">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="69e6a-356">indexof</span><span class="sxs-lookup"><span data-stu-id="69e6a-356">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="69e6a-357">substring</span><span class="sxs-lookup"><span data-stu-id="69e6a-357">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="69e6a-358">tolower</span><span class="sxs-lookup"><span data-stu-id="69e6a-358">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="69e6a-359">toupper</span><span class="sxs-lookup"><span data-stu-id="69e6a-359">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="69e6a-360">trim</span><span class="sxs-lookup"><span data-stu-id="69e6a-360">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="69e6a-361">concat</span><span class="sxs-lookup"><span data-stu-id="69e6a-361">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="69e6a-362">OneNote 实体属性</span><span class="sxs-lookup"><span data-stu-id="69e6a-362">OneNote entity properties</span></span>

<span data-ttu-id="69e6a-363">**filter**、**select**、**expand** 和 **orderby** 查询表达式可以包含 OneNote 实体的属性。</span><span class="sxs-lookup"><span data-stu-id="69e6a-363">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="69e6a-364">示例</span><span class="sxs-lookup"><span data-stu-id="69e6a-364">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="69e6a-365">查询表达式中的属性名称区分大小写。</span><span class="sxs-lookup"><span data-stu-id="69e6a-365">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="69e6a-366">有关属性列表和属性类型，请参阅 Microsoft Graph API REST 引用中的以下资源：</span><span class="sxs-lookup"><span data-stu-id="69e6a-366">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="69e6a-367">GET 页面</span><span class="sxs-lookup"><span data-stu-id="69e6a-367">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-368">GET 节</span><span class="sxs-lookup"><span data-stu-id="69e6a-368">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-369">GET 节组</span><span class="sxs-lookup"><span data-stu-id="69e6a-369">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="69e6a-370">GET 笔记本</span><span class="sxs-lookup"><span data-stu-id="69e6a-370">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="69e6a-371">**expand** 查询字符串选项可与以下导航属性一起使用：</span><span class="sxs-lookup"><span data-stu-id="69e6a-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="69e6a-372">页面：**parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="69e6a-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="69e6a-373">节：**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="69e6a-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="69e6a-374">节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="69e6a-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="69e6a-375">笔记本：**sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="69e6a-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="69e6a-376">*GET* 请求的请求和响应信息</span><span class="sxs-lookup"><span data-stu-id="69e6a-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="69e6a-377">请求数据</span><span class="sxs-lookup"><span data-stu-id="69e6a-377">Request data</span></span> | <span data-ttu-id="69e6a-378">说明</span><span class="sxs-lookup"><span data-stu-id="69e6a-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="69e6a-379">协议</span><span class="sxs-lookup"><span data-stu-id="69e6a-379">Protocol</span></span> | <span data-ttu-id="69e6a-380">所有请求均使用 SSL/TLS HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="69e6a-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="69e6a-381">授权标头</span><span class="sxs-lookup"><span data-stu-id="69e6a-381">Authorization header</span></span> | <p><span data-ttu-id="69e6a-382">`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</span><span class="sxs-lookup"><span data-stu-id="69e6a-382">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="69e6a-383">如果缺少或无效，则请求失败，并显示 401 状态代码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="69e6a-384">请参阅[身份验证和权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-384">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="69e6a-385">接受标头</span><span class="sxs-lookup"><span data-stu-id="69e6a-385">Accept header</span></span> | <p> <span data-ttu-id="69e6a-386">`application/json` 适用于 OneNote 实体和实体集</span><span class="sxs-lookup"><span data-stu-id="69e6a-386">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="69e6a-387">`text/html` 适用于页面内容</span><span class="sxs-lookup"><span data-stu-id="69e6a-387">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="69e6a-388">响应数据</span><span class="sxs-lookup"><span data-stu-id="69e6a-388">Response data</span></span> | <span data-ttu-id="69e6a-389">说明</span><span class="sxs-lookup"><span data-stu-id="69e6a-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="69e6a-390">成功代码</span><span class="sxs-lookup"><span data-stu-id="69e6a-390">Success code</span></span> | <span data-ttu-id="69e6a-391">200 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-391">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="69e6a-392">响应正文</span><span class="sxs-lookup"><span data-stu-id="69e6a-392">Response body</span></span> | <span data-ttu-id="69e6a-393">JSON 格式、页面 HTML 或文件资源二进制数据中的实体或实体集的 OData 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69e6a-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="69e6a-394">错误</span><span class="sxs-lookup"><span data-stu-id="69e6a-394">Errors</span></span> | <span data-ttu-id="69e6a-395">如果请求失败，API 将在响应正文的 **\@api.diagnostics** 对象中返回 [错误](onenote-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-395">If the request fails, the API returns [errors](onenote-error-codes.md) in the **\@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="69e6a-396">X-CorrelationId 标头</span><span class="sxs-lookup"><span data-stu-id="69e6a-396">X-CorrelationId header</span></span> | <span data-ttu-id="69e6a-397">唯一标识该请求的 GUID。</span><span class="sxs-lookup"><span data-stu-id="69e6a-397">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="69e6a-398">在与 Microsoft 支持部门协作来解决问题时，可以使用此值和日期标头值。</span><span class="sxs-lookup"><span data-stu-id="69e6a-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="69e6a-399">构建 Microsoft Graph 笔记服务根 URL</span><span class="sxs-lookup"><span data-stu-id="69e6a-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="69e6a-400">Microsoft Graph 笔记根 URL 为 Microsoft Graph 笔记的所有调用使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="69e6a-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="69e6a-401">URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。</span><span class="sxs-lookup"><span data-stu-id="69e6a-401">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="69e6a-402">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="69e6a-403">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="69e6a-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="69e6a-404">Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。</span><span class="sxs-lookup"><span data-stu-id="69e6a-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="69e6a-405">为当前用户可以访问的 OneNote 内容（拥有和共享）使用 `me`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="69e6a-406">为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）使用 `users/{id}`。</span><span class="sxs-lookup"><span data-stu-id="69e6a-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="69e6a-407">使用 [Microsoft Graph](https://graph.microsoft.com/v1.0/users) 获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="69e6a-407">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="69e6a-408">GET 请求的权限</span><span class="sxs-lookup"><span data-stu-id="69e6a-408">Permissions for GET requests</span></span>

<span data-ttu-id="69e6a-409">若要获取 OneNote 内容或结构，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="69e6a-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="69e6a-410">以下范围允许对 Microsoft Graph 执行 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="69e6a-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="69e6a-411">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="69e6a-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="69e6a-412">从以下项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="69e6a-412">Choose from:</span></span>

- <span data-ttu-id="69e6a-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="69e6a-413">Notes.read</span></span>
- <span data-ttu-id="69e6a-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69e6a-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="69e6a-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69e6a-415">Notes.ReadWrite.All</span></span>

<span data-ttu-id="69e6a-416">有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="69e6a-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="69e6a-417">另请参阅</span><span class="sxs-lookup"><span data-stu-id="69e6a-417">See also</span></span>

- [<span data-ttu-id="69e6a-418">OneNote 页面的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="69e6a-418">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="69e6a-419">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="69e6a-419">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="69e6a-420">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="69e6a-420">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="69e6a-421">Microsoft Q&A 上的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="69e6a-421">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="69e6a-422">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="69e6a-422">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)