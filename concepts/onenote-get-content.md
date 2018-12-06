---
title: 使用 Microsoft Graph 获取 OneNote 内容和结构
description: " 在 Office 365 的企业笔记本"
ms.openlocfilehash: d5a1b382535988e48b5b710d3685a344c5f5a40d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091889"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="e60c5-103">使用 Microsoft Graph 获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="e60c5-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="e60c5-104">**适用于**：OneDrive 上的消费者笔记本 | Office 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="e60c5-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="e60c5-105">若要获取 OneNote 内容和结构，请向目标终结点发送 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="e60c5-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="e60c5-106">例如：</span><span class="sxs-lookup"><span data-stu-id="e60c5-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="e60c5-107">如果请求成功，Microsoft Graph 将返回一个 200 HTTP 状态代码以及请求的实体或内容。</span><span class="sxs-lookup"><span data-stu-id="e60c5-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="e60c5-108">OneNote 实体作为符合 OData 版本 4.0 规范的 JSON 对象返回。</span><span class="sxs-lookup"><span data-stu-id="e60c5-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="e60c5-109">通过使用查询字符串选项，可以过滤查询并提高性能。</span><span class="sxs-lookup"><span data-stu-id="e60c5-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="e60c5-110">构建请求 URI</span><span class="sxs-lookup"><span data-stu-id="e60c5-110">Construct the request URI</span></span>

<span data-ttu-id="e60c5-111">若要构建请求 URI，请从服务根 URL 开始：</span><span class="sxs-lookup"><span data-stu-id="e60c5-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="e60c5-112">然后附加想要检索的资源端点。</span><span class="sxs-lookup"><span data-stu-id="e60c5-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="e60c5-113">（[资源路径](#resource-paths-for-get-requests) 将在下一节中介绍。）</span><span class="sxs-lookup"><span data-stu-id="e60c5-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="e60c5-114">完整的请求 URI 类似于以下示例之一：</span><span class="sxs-lookup"><span data-stu-id="e60c5-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="e60c5-115">**注意：** 了解有关[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e60c5-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="e60c5-116">GET 请求的资源路径</span><span class="sxs-lookup"><span data-stu-id="e60c5-116">Resource paths for GET requests</span></span>

<span data-ttu-id="e60c5-117">使用以下资源路径获取页面、节、节组、笔记本和图像或文件资源。</span><span class="sxs-lookup"><span data-stu-id="e60c5-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="e60c5-118">页面集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="e60c5-119">页面实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="e60c5-120">页面预览</span><span class="sxs-lookup"><span data-stu-id="e60c5-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="e60c5-121">页面 HTML 内容</span><span class="sxs-lookup"><span data-stu-id="e60c5-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="e60c5-122">节集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="e60c5-123">节实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="e60c5-124">SectionGroup 集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="e60c5-125">SectionGroup 实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="e60c5-126">笔记本集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="e60c5-127">笔记本实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="e60c5-128">图像或其他文件资源</span><span class="sxs-lookup"><span data-stu-id="e60c5-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="e60c5-129">页面集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-129">Page collection</span></span>

<span data-ttu-id="e60c5-130">获取所有笔记本的页面（元数据）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="e60c5-131">从特定节获取页面（元数据）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="e60c5-132">`search` 查询字符串选项仅适用于消费者笔记本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="e60c5-133">页面的默认排序顺序是 `lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="e60c5-134">默认查询展开父节并选择节 `id`、 `name`和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="e60c5-135">默认情况下，为 *GET 页面*请求返回仅前 20 个实体。</span><span class="sxs-lookup"><span data-stu-id="e60c5-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="e60c5-136">未指定 **top** 查询字符串选项的请求将在响应中返回 `@odata.nextLink` 链接，该链接可用于获取接下来的 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="e60c5-137">对于节中的页面集合，使用 **pagelevel** 返回页面的缩进级别及其在节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="e60c5-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="e60c5-138">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="e60c5-139">页面实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-139">Page entity</span></span>

<span data-ttu-id="e60c5-140">获取特定页面的元数据。</span><span class="sxs-lookup"><span data-stu-id="e60c5-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="e60c5-141">页面可以扩展 **parentNotebook** 和 **parentSection** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="e60c5-142">默认查询展开父节并选择节 `id`、 `name`和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="e60c5-143">使用 **pagelevel** 返回页面的缩进级别及其在父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="e60c5-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="e60c5-144">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="e60c5-145">页面预览</span><span class="sxs-lookup"><span data-stu-id="e60c5-145">Page preview</span></span>

<span data-ttu-id="e60c5-146">获取页面的文字和图像预览内容。</span><span class="sxs-lookup"><span data-stu-id="e60c5-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="e60c5-147">JSON 响应包含预览内容，可用于帮助用户标识页面中的内容。</span><span class="sxs-lookup"><span data-stu-id="e60c5-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="e60c5-148">**previewText** 属性包含来自页面的文本片段。</span><span class="sxs-lookup"><span data-stu-id="e60c5-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="e60c5-149">Microsoft Graph 返回完整短语，最多 300 个字符。</span><span class="sxs-lookup"><span data-stu-id="e60c5-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="e60c5-150">如果页面包含可用于生成预览 UI 的图像，则 **previewImageUrl** 对象中的 **href** 属性包含指向公共、预验证[图像资源](#image-or-other-file-resource)的链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="e60c5-151">可以在 HTML 中使用此链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-151">You can use this link in HTML.</span></span> <span data-ttu-id="e60c5-152">否则，**href** 返回 null。</span><span class="sxs-lookup"><span data-stu-id="e60c5-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="e60c5-153">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="e60c5-154">页面 HTML 内容</span><span class="sxs-lookup"><span data-stu-id="e60c5-154">Page HTML content</span></span>

<span data-ttu-id="e60c5-155">获取页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="e60c5-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

<span data-ttu-id="e60c5-156">（*了解有关[返回的 HTML 内容](onenote-input-output-html.md)* 的详细信息）</span><span class="sxs-lookup"><span data-stu-id="e60c5-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="e60c5-157">使用 **includeIDs=true** 查询字符串选项获取生成的 ID，用于[更新页面](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>

<span data-ttu-id="e60c5-158">使用 **preAuthenticated=true** 查询字符串选项以获取页面上的 [图像资源](#image-or-other-file-resource) 公共 URL。</span><span class="sxs-lookup"><span data-stu-id="e60c5-158">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="e60c5-159">公共 URL 的有效期为 1 小时。</span><span class="sxs-lookup"><span data-stu-id="e60c5-159">The public URLs are valid for one hour.</span></span> 



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="e60c5-160">节集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-160">Section collection</span></span>

<span data-ttu-id="e60c5-161">获取用户拥有的所有笔记本的所有节，包括嵌套节组中的节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-161">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-162">获取直接位于特定节组下的所有节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-162">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-163">获取直接位于特定笔记本下的所有节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-163">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-164">节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-164">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e60c5-165">节的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-165">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="e60c5-166">默认查询扩展父笔记本和父节组，并选择它们的 `id`、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-166">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="e60c5-167">节实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-167">Section entity</span></span>

<span data-ttu-id="e60c5-168">获取特定节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-168">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="e60c5-169">节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-169">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e60c5-170">默认查询扩展父笔记本和父节组，并选择它们的 `id`、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-170">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="e60c5-171">SectionGroup 集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-171">SectionGroup collection</span></span>

<span data-ttu-id="e60c5-172">获取用户拥有的所有笔记本的所有节组，包括嵌套节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-172">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-173">获取直接位于特定笔记本下的所有节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-173">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-174">节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-174">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e60c5-175">部分组的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-175">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="e60c5-176">默认查询扩展父笔记本和父节组，并选择它们的 `id`、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-176">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="e60c5-177">SectionGroup 实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-177">SectionGroup entity</span></span>

<span data-ttu-id="e60c5-178">获取特定节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-178">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="e60c5-179">节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-179">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="e60c5-180">默认查询扩展父笔记本和父节组，并选择它们的 `id`、 `name` 和 `self` 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-180">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="e60c5-181">笔记本集合</span><span class="sxs-lookup"><span data-stu-id="e60c5-181">Notebook collection</span></span>

<span data-ttu-id="e60c5-182">获取用户拥有的所有笔记本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-182">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="e60c5-183">笔记本可以展开 **sections** 和 **sectionGroups** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-183">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="e60c5-184">笔记本的默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-184">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="e60c5-185">笔记本实体</span><span class="sxs-lookup"><span data-stu-id="e60c5-185">Notebook entity</span></span>

<span data-ttu-id="e60c5-186">获取特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-186">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="e60c5-187">笔记本可以展开 **sections** 和 **sectionGroups** 属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-187">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="e60c5-188">图像或其他文件资源</span><span class="sxs-lookup"><span data-stu-id="e60c5-188">Image or other file resource</span></span>

<span data-ttu-id="e60c5-189">获取特定资源的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="e60c5-189">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="e60c5-190">可以在页面的[输出 HTML](onenote-input-output-html.md) 中找到文件的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="e60c5-190">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="e60c5-191">例如，**img** 标记包含 **data-fullres-src** 属性中原始图像的终结点和 **src** 属性中经优化图像的终结点。</span><span class="sxs-lookup"><span data-stu-id="e60c5-191">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="e60c5-192">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-192">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="e60c5-193">**object** 标记包含 **data** 属性中文件资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="e60c5-193">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="e60c5-194">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-194">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="e60c5-195">若要获取页面上图像资源的公共、预验证 URL，请在[检索页面内容](#page-html-content)时，在查询字符串中添加 `preAuthenticated=true`（**示例：**  `GET ../pages/{page-id}/content?preAuthenticated=true`）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-195">To get public, pre-authenticated URLs to the image resources on a page, include `preAuthenticated=true` in the query string when you [retrieve the page content](#page-html-content) (**example:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="e60c5-196">[输出 HTML](onenote-input-output-html.md#output-html-examples-for-images) 中返回的公共 URL 的有效期为 1 小时。</span><span class="sxs-lookup"><span data-stu-id="e60c5-196">The public URLs that are returned in the [output HTML](onenote-input-output-html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="e60c5-197">没有此标记时，检索的图像并不会直接在浏览器中显示，因为它们具有私密性，需要授权才能对其检索，这与页面其他内容一样。</span><span class="sxs-lookup"><span data-stu-id="e60c5-197">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="e60c5-198">**注意：** 不支持获取资源的集合。</span><span class="sxs-lookup"><span data-stu-id="e60c5-198">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="e60c5-199">在获取文件资源时，无需在请求中包含 **Accept** 内容类型。</span><span class="sxs-lookup"><span data-stu-id="e60c5-199">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="e60c5-200">有关 GET 请求的详细信息，请参阅 Microsoft Graph API REST 引用中的以下资源：</span><span class="sxs-lookup"><span data-stu-id="e60c5-200">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="e60c5-201">GET 页面</span><span class="sxs-lookup"><span data-stu-id="e60c5-201">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-202">GET 节</span><span class="sxs-lookup"><span data-stu-id="e60c5-202">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-203">GET 节组</span><span class="sxs-lookup"><span data-stu-id="e60c5-203">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-204">GET 笔记本</span><span class="sxs-lookup"><span data-stu-id="e60c5-204">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="e60c5-205">示例 GET 请求</span><span class="sxs-lookup"><span data-stu-id="e60c5-205">Example GET requests</span></span>

<span data-ttu-id="e60c5-206">可以查询 OneNote 实体和搜索页面内容以仅获取所需的信息。</span><span class="sxs-lookup"><span data-stu-id="e60c5-206">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="e60c5-207">以下示例演示了一些方法，可以在对 Microsoft Graph 的 GET 请求中使用[支持的查询字符串选项](#supported-odata-query-string-options)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-207">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="e60c5-208">**请注意：**</span><span class="sxs-lookup"><span data-stu-id="e60c5-208">**Remember:**</span></span>

- <span data-ttu-id="e60c5-209">所有的 GET 请求都以[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 开头。</span><span class="sxs-lookup"><span data-stu-id="e60c5-209">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="e60c5-210">**示例**：`https://www.onenote.com/api/v1.0/me/notes` 和 `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span><span class="sxs-lookup"><span data-stu-id="e60c5-210">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="e60c5-211">URL 查询字符串中的空格必须使用 %20 编码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-211">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="e60c5-212">**示例**：`filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="e60c5-212">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="e60c5-213">属性名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-213">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="e60c5-214">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="e60c5-214">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="e60c5-215">**示例**：`filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e60c5-215">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="e60c5-216">search & filter</span><span class="sxs-lookup"><span data-stu-id="e60c5-216">search & filter</span></span>  

<span data-ttu-id="e60c5-217">获取包含由特定应用创建的术语 *recipe* 的所有页面（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-217">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="e60c5-218">search & select</span><span class="sxs-lookup"><span data-stu-id="e60c5-218">search & select</span></span>  

<span data-ttu-id="e60c5-219">获取包含术语 *golgi app* 的所有页面的标题、OneNote 客户端链接和 **contentUrl** 链接（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-219">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="e60c5-220">expand</span><span class="sxs-lookup"><span data-stu-id="e60c5-220">expand</span></span> 

<span data-ttu-id="e60c5-221">获取所有笔记本，并展开它的节和节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-221">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="e60c5-222">获取某个特定的节组，并展开它的节和节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-222">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="e60c5-223">获取一个页面并展开其父节和父笔记本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-223">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="e60c5-224">expand（多个级别）</span><span class="sxs-lookup"><span data-stu-id="e60c5-224">expand (multiple levels)</span></span>  

<span data-ttu-id="e60c5-225">获取所有笔记本，展开其节和节组，并在每个节组中展开所有节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-225">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="e60c5-226">**注意：** 展开子实体的父项或展开父实体的子项来创建循环引用，这并不受支持。</span><span class="sxs-lookup"><span data-stu-id="e60c5-226">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="e60c5-227">expand & select（多个级别）</span><span class="sxs-lookup"><span data-stu-id="e60c5-227">expand & select (multiple levels)</span></span>  

<span data-ttu-id="e60c5-228">获取特定节组的名称和 **self** 链接，并获取其所有节的名称和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-228">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="e60c5-229">获取所有节的名称和 **self** 链接，并获取每个节的父笔记本的名称和创建时间。</span><span class="sxs-lookup"><span data-stu-id="e60c5-229">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="e60c5-230">获取所有页面的标题和 ID，并获取父节和父笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="e60c5-230">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="e60c5-231">expand & levels（多个级别）</span><span class="sxs-lookup"><span data-stu-id="e60c5-231">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="e60c5-232">获取所有笔记本、节和节组。</span><span class="sxs-lookup"><span data-stu-id="e60c5-232">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="e60c5-233">filter</span><span class="sxs-lookup"><span data-stu-id="e60c5-233">filter</span></span>

<span data-ttu-id="e60c5-234">获取 2014 年 10 月创建的所有节。</span><span class="sxs-lookup"><span data-stu-id="e60c5-234">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="e60c5-235">获取某个特定应用自 2015 年 1 月 1 日以来所创建的页面。</span><span class="sxs-lookup"><span data-stu-id="e60c5-235">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="e60c5-236">filter & expand</span><span class="sxs-lookup"><span data-stu-id="e60c5-236">filter & expand</span></span>  

<span data-ttu-id="e60c5-237">获取特定笔记本中的所有页面。</span><span class="sxs-lookup"><span data-stu-id="e60c5-237">Get all pages in a specific notebook.</span></span> <span data-ttu-id="e60c5-238">该 API 默认返回 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-238">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="e60c5-239">获取 *School* 笔记本的所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-239">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="e60c5-240">OData 字符串比较区分大小写，因此，作为最佳做法将使用 **tolower** 函数。</span><span class="sxs-lookup"><span data-stu-id="e60c5-240">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="e60c5-241">filter & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e60c5-241">filter & select & orderby</span></span>   

<span data-ttu-id="e60c5-242">获取在节名中包含术语 *spring* 的所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-242">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="e60c5-243">按照最后修改日期对节进行排序。</span><span class="sxs-lookup"><span data-stu-id="e60c5-243">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="e60c5-244">orderby</span><span class="sxs-lookup"><span data-stu-id="e60c5-244">orderby</span></span>

<span data-ttu-id="e60c5-245">获取先按照 **createdByAppId** 属性排序再按照最近创建时间排序的前 20 个页面。</span><span class="sxs-lookup"><span data-stu-id="e60c5-245">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="e60c5-246">默认情况下，API 返回 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-246">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="e60c5-247">search & filter & top</span><span class="sxs-lookup"><span data-stu-id="e60c5-247">search & filter & top</span></span> 

<span data-ttu-id="e60c5-248">获取自 2015 年 1 月 1 日以来创建的包含短语 *cell division* 的 5 个最新页面。</span><span class="sxs-lookup"><span data-stu-id="e60c5-248">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="e60c5-249">默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-249">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="e60c5-250">页面的默认排序顺序为 `lastModifiedTime desc`（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-250">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="e60c5-251">search & filter & top & skip</span><span class="sxs-lookup"><span data-stu-id="e60c5-251">search & filter & top & skip</span></span>  

<span data-ttu-id="e60c5-252">获取结果集中接下来的五个页面（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-252">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="e60c5-253">以及接下来的五页（`search` 仅适用于消费者笔记本）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-253">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="e60c5-254">**注意：** 如果 **search** 和 **filter** 都应用于同一请求，则结果只包含与这两个条件都匹配的实体。</span><span class="sxs-lookup"><span data-stu-id="e60c5-254">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="e60c5-255">select</span><span class="sxs-lookup"><span data-stu-id="e60c5-255">select</span></span>

<span data-ttu-id="e60c5-256">获取用户笔记本中所有节的名称、创建时间和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-256">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="e60c5-257">获取特定页面的标题、创建时间和 OneNote 客户端链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-257">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="e60c5-258">select & expand & filter（多个级别）</span><span class="sxs-lookup"><span data-stu-id="e60c5-258">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="e60c5-259">获取用户的默认笔记本中所有节的名称和 **pagesUrl** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-259">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="e60c5-260">top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e60c5-260">top & select & orderby</span></span> 

<span data-ttu-id="e60c5-261">获取按标题字母顺序排序的前 50 个页面的标题和 **self** 链接。</span><span class="sxs-lookup"><span data-stu-id="e60c5-261">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="e60c5-262">默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-262">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="e60c5-263">页面的默认排序顺序是 `lastModifiedTime desc`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-263">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="e60c5-264">skip & top & select & orderby</span><span class="sxs-lookup"><span data-stu-id="e60c5-264">skip & top & select & orderby</span></span>  

<span data-ttu-id="e60c5-p117">获取第 51 至 100 页。默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-p117">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="e60c5-267">**注意：** 检索条目默认数量（即，它们不指定 **top** 表达式）的页面的 GET 请求在响应中将返回一个 **@odata.nextLink** 链接，你可使用此链接获取接下来的 20 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-267">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="e60c5-268">受支持的 OData 查询字符串选项</span><span class="sxs-lookup"><span data-stu-id="e60c5-268">Supported OData query string options</span></span>

<span data-ttu-id="e60c5-269">向 Microsoft Graph 发送 GET 请求时，可以使用 OData 查询字符串选项来自定义查询并仅获取所需的信息。</span><span class="sxs-lookup"><span data-stu-id="e60c5-269">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="e60c5-270">它们可以通过减少对该服务的调用数量以及响应有效负载的大小来提高性能。</span><span class="sxs-lookup"><span data-stu-id="e60c5-270">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="e60c5-271">**注意：** 为了增强可读性，本文中的示例不使用 URL 查询字符串中空格所需的 %20 百分比编码：`filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="e60c5-271">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="e60c5-272">查询选项</span><span class="sxs-lookup"><span data-stu-id="e60c5-272">Query option</span></span> | <span data-ttu-id="e60c5-273">示例和说明</span><span class="sxs-lookup"><span data-stu-id="e60c5-273">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="e60c5-274">count</span><span class="sxs-lookup"><span data-stu-id="e60c5-274">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="e60c5-p119">集合中的实体计数。在响应的 **@odata.count** 属性中返回此值。</span><span class="sxs-lookup"><span data-stu-id="e60c5-p119">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="e60c5-277">expand</span><span class="sxs-lookup"><span data-stu-id="e60c5-277">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="e60c5-278">要在响应中返回内联的导航属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-278">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="e60c5-279">**expand** 表达式支持以下属性：</span><span class="sxs-lookup"><span data-stu-id="e60c5-279">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="e60c5-280">- 页面：**parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="e60c5-280">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="e60c5-281">- 节：**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e60c5-281">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="e60c5-282">- 节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e60c5-282">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="e60c5-283">- 笔记本：**sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="e60c5-283">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="e60c5-p121">默认情况下，页面的 GET 请求同时展开 **parentSection** 并选择该节的 **id**、**name** 和 **self** 属性。节和节组的默认 GET 请求扩展 **parentNotebook** 和 **parentSectionGroup**，并选择父项的**id**、**name** 和 **self** 属性。 </span><span class="sxs-lookup"><span data-stu-id="e60c5-p121">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="e60c5-286">可用于单个实体或集合。</span><span class="sxs-lookup"><span data-stu-id="e60c5-286">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="e60c5-287">使用逗号分隔多个属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-287">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="e60c5-288">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-288">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="e60c5-289">filter</span><span class="sxs-lookup"><span data-stu-id="e60c5-289">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="e60c5-290">是否在结果集中包含条目的布尔表达式。</span><span class="sxs-lookup"><span data-stu-id="e60c5-290">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="e60c5-291">支持以下 OData 运算符和函数：</span><span class="sxs-lookup"><span data-stu-id="e60c5-291">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="e60c5-292">- 比较运算符： **EQ**， **NE**， **GT**， **ge**， **LT**， **le**</span><span class="sxs-lookup"><span data-stu-id="e60c5-292">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="e60c5-293">- 逻辑运算符： **and**， **or**， **not**</span><span class="sxs-lookup"><span data-stu-id="e60c5-293">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="e60c5-294">- 字符串函数：**contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</span><span class="sxs-lookup"><span data-stu-id="e60c5-294">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="e60c5-295">[属性](#onenote-entity-properties)名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-295">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="e60c5-296">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="e60c5-296">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="e60c5-297">**示例**：`filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e60c5-297">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="e60c5-298">orderby</span><span class="sxs-lookup"><span data-stu-id="e60c5-298">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="e60c5-p124">作为排序依据的[属性](#onenote-entity-properties)，具有可选的 **asc**（默认）或 **desc** 的排序顺序。您可以按请求集合中实体的任意属性进行排序。</span><span class="sxs-lookup"><span data-stu-id="e60c5-p124">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="e60c5-301">笔记本、节组和节的默认排序顺序为 `name asc`，页面的默认排序顺序为 `lastModifiedTime desc`（最后修改的页面排第一）。</span><span class="sxs-lookup"><span data-stu-id="e60c5-301">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="e60c5-302">用逗号隔开多个属性，并按想要应用属性的顺序列出它们。</span><span class="sxs-lookup"><span data-stu-id="e60c5-302">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="e60c5-303">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-303">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="e60c5-304">search</span><span class="sxs-lookup"><span data-stu-id="e60c5-304">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="e60c5-305">仅适用于消费者笔记本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-305">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="e60c5-p126">要在页面标题、页面正文、图像替换文字、图像 OCR 文本中搜索的术语或短语。默认情况下，搜索查询返回按相关性排序的结果。</span><span class="sxs-lookup"><span data-stu-id="e60c5-p126">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="e60c5-308">OneNote 使用必应全文搜索来支持短语搜索、词干分解、拼写宽容、相关性和排名、断字、多语言以及其他全文搜索功能。</span><span class="sxs-lookup"><span data-stu-id="e60c5-308">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="e60c5-309">搜索字符串不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-309">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="e60c5-310">仅适用于用户拥有的笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="e60c5-310">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="e60c5-311">已编入索引的内容具有私密性，只有所有者才能访问。</span><span class="sxs-lookup"><span data-stu-id="e60c5-311">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="e60c5-312">受密码保护的页面未被编入索引。</span><span class="sxs-lookup"><span data-stu-id="e60c5-312">Password-protected pages are not indexed.</span></span> <span data-ttu-id="e60c5-313">仅适用于 `pages` 端点。</span><span class="sxs-lookup"><span data-stu-id="e60c5-313">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="e60c5-314">select</span><span class="sxs-lookup"><span data-stu-id="e60c5-314">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="e60c5-315">要返回的[属性](#onenote-entity-properties)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-315">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="e60c5-316">可用于单个实体或集合。</span><span class="sxs-lookup"><span data-stu-id="e60c5-316">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="e60c5-317">使用逗号分隔多个属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-317">Separate multiple properties with commas.</span></span> <span data-ttu-id="e60c5-318">属性名区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-318">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="e60c5-319">skip</span><span class="sxs-lookup"><span data-stu-id="e60c5-319">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="e60c5-320">结果集中要跳过的条目数量。</span><span class="sxs-lookup"><span data-stu-id="e60c5-320">The number of entries to skip in the result set.</span></span> <span data-ttu-id="e60c5-321">通常用于分页结果。</span><span class="sxs-lookup"><span data-stu-id="e60c5-321">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="e60c5-322">top</span><span class="sxs-lookup"><span data-stu-id="e60c5-322">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="e60c5-323">结果集中要返回的条目数量，最多可达 100 个条目。</span><span class="sxs-lookup"><span data-stu-id="e60c5-323">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="e60c5-324">默认值为 20。</span><span class="sxs-lookup"><span data-stu-id="e60c5-324">The default value is 20.</span></span></p> |  

<span data-ttu-id="e60c5-325">Microsoft Graph 还提供 `pagelevel` 查询字符串选项，可使用该选项获取父节内页面的级别和顺序。</span><span class="sxs-lookup"><span data-stu-id="e60c5-325">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="e60c5-326">仅适用于特定节中页面的查询或特定页面中的查询。</span><span class="sxs-lookup"><span data-stu-id="e60c5-326">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="e60c5-327">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-327">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="e60c5-328">受支持的 OData 运算符和函数</span><span class="sxs-lookup"><span data-stu-id="e60c5-328">Supported OData operators and functions</span></span>

<span data-ttu-id="e60c5-329">Microsoft Graph 支持 **filter** 表达式中的以下 OData 运算符和函数。</span><span class="sxs-lookup"><span data-stu-id="e60c5-329">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="e60c5-330">使用 OData 表达式时，请记住：</span><span class="sxs-lookup"><span data-stu-id="e60c5-330">When using OData expressions, remember:</span></span>

- <span data-ttu-id="e60c5-331">必须将 URL 查询字符串中的空格替换为 `%20` 编码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-331">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="e60c5-332">**示例：** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="e60c5-332">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="e60c5-333">属性名和 OData 字符串比较均区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-333">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="e60c5-334">建议使用 OData **tolower** 函数进行字符串比较。</span><span class="sxs-lookup"><span data-stu-id="e60c5-334">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="e60c5-335">**示例：** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="e60c5-335">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="e60c5-336">比较运算符</span><span class="sxs-lookup"><span data-stu-id="e60c5-336">Comparison operator</span></span> | <span data-ttu-id="e60c5-337">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-337">Example</span></span> |  
|------|------|  
| <span data-ttu-id="e60c5-338">eq</span><span class="sxs-lookup"><span data-stu-id="e60c5-338">eq</span></span><br /><span data-ttu-id="e60c5-339">（等于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-339">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="e60c5-340">ne</span><span class="sxs-lookup"><span data-stu-id="e60c5-340">ne</span></span><br /><span data-ttu-id="e60c5-341">（不等于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-341">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="e60c5-342">gt</span><span class="sxs-lookup"><span data-stu-id="e60c5-342">gt</span></span><br /><span data-ttu-id="e60c5-343">（大于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-343">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="e60c5-344">ge</span><span class="sxs-lookup"><span data-stu-id="e60c5-344">ge</span></span><br /><span data-ttu-id="e60c5-345">（大于或等于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-345">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="e60c5-346">lt</span><span class="sxs-lookup"><span data-stu-id="e60c5-346">lt</span></span><br /><span data-ttu-id="e60c5-347">（小于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-347">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="e60c5-348">le</span><span class="sxs-lookup"><span data-stu-id="e60c5-348">le</span></span><br /><span data-ttu-id="e60c5-349">（小于或等于）</span><span class="sxs-lookup"><span data-stu-id="e60c5-349">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="e60c5-350">逻辑运算符</span><span class="sxs-lookup"><span data-stu-id="e60c5-350">Logical operator</span></span> | <span data-ttu-id="e60c5-351">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-351">Example</span></span> |  
|------|------|  
| <span data-ttu-id="e60c5-352">和</span><span class="sxs-lookup"><span data-stu-id="e60c5-352">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="e60c5-353">或</span><span class="sxs-lookup"><span data-stu-id="e60c5-353">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="e60c5-354">not</span><span class="sxs-lookup"><span data-stu-id="e60c5-354">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="e60c5-355">字符串函数</span><span class="sxs-lookup"><span data-stu-id="e60c5-355">String function</span></span> | <span data-ttu-id="e60c5-356">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-356">Example</span></span> |  
|------|------|   
| <span data-ttu-id="e60c5-357">contains</span><span class="sxs-lookup"><span data-stu-id="e60c5-357">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="e60c5-358">endswith</span><span class="sxs-lookup"><span data-stu-id="e60c5-358">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="e60c5-359">startswith</span><span class="sxs-lookup"><span data-stu-id="e60c5-359">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="e60c5-360">length</span><span class="sxs-lookup"><span data-stu-id="e60c5-360">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="e60c5-361">indexof</span><span class="sxs-lookup"><span data-stu-id="e60c5-361">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="e60c5-362">substring</span><span class="sxs-lookup"><span data-stu-id="e60c5-362">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="e60c5-363">tolower</span><span class="sxs-lookup"><span data-stu-id="e60c5-363">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="e60c5-364">toupper</span><span class="sxs-lookup"><span data-stu-id="e60c5-364">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="e60c5-365">trim</span><span class="sxs-lookup"><span data-stu-id="e60c5-365">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="e60c5-366">concat</span><span class="sxs-lookup"><span data-stu-id="e60c5-366">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="e60c5-367">OneNote 实体属性</span><span class="sxs-lookup"><span data-stu-id="e60c5-367">OneNote entity properties</span></span>

<span data-ttu-id="e60c5-368">**filter**、**select**、**expand** 和 **orderby** 查询表达式可以包含 OneNote 实体的属性。</span><span class="sxs-lookup"><span data-stu-id="e60c5-368">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="e60c5-369">示例</span><span class="sxs-lookup"><span data-stu-id="e60c5-369">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="e60c5-370">查询表达式中的属性名称区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e60c5-370">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="e60c5-371">有关属性列表和属性类型，请参阅 Microsoft Graph API REST 引用中的以下资源：</span><span class="sxs-lookup"><span data-stu-id="e60c5-371">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="e60c5-372">GET 页面</span><span class="sxs-lookup"><span data-stu-id="e60c5-372">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-373">GET 节</span><span class="sxs-lookup"><span data-stu-id="e60c5-373">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-374">GET 节组</span><span class="sxs-lookup"><span data-stu-id="e60c5-374">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="e60c5-375">GET 笔记本</span><span class="sxs-lookup"><span data-stu-id="e60c5-375">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="e60c5-376">**expand** 查询字符串选项可与以下导航属性一起使用：</span><span class="sxs-lookup"><span data-stu-id="e60c5-376">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="e60c5-377">页面：**parentNotebook**、**parentSection**</span><span class="sxs-lookup"><span data-stu-id="e60c5-377">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="e60c5-378">节：**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e60c5-378">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="e60c5-379">节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**</span><span class="sxs-lookup"><span data-stu-id="e60c5-379">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="e60c5-380">笔记本：**sections**、**sectionGroups**</span><span class="sxs-lookup"><span data-stu-id="e60c5-380">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="e60c5-381">*GET* 请求的请求和响应信息</span><span class="sxs-lookup"><span data-stu-id="e60c5-381">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="e60c5-382">请求数据</span><span class="sxs-lookup"><span data-stu-id="e60c5-382">Request data</span></span> | <span data-ttu-id="e60c5-383">说明</span><span class="sxs-lookup"><span data-stu-id="e60c5-383">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e60c5-384">协议</span><span class="sxs-lookup"><span data-stu-id="e60c5-384">Protocol</span></span> | <span data-ttu-id="e60c5-385">所有请求均使用 SSL/TLS HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="e60c5-385">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="e60c5-386">授权标头</span><span class="sxs-lookup"><span data-stu-id="e60c5-386">Authorization header</span></span> | <p><span data-ttu-id="e60c5-387">`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</span><span class="sxs-lookup"><span data-stu-id="e60c5-387">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="e60c5-388">如果缺少或无效，则请求失败，并显示 401 状态代码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-388">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="e60c5-389">请参阅 [身份验证和权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-389">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="e60c5-390">接受标头</span><span class="sxs-lookup"><span data-stu-id="e60c5-390">Accept header</span></span> | <p> <span data-ttu-id="e60c5-391">`application/json` 适用于 OneNote 实体和实体集</span><span class="sxs-lookup"><span data-stu-id="e60c5-391">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="e60c5-392">`text/html` 适用于页面内容</span><span class="sxs-lookup"><span data-stu-id="e60c5-392">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="e60c5-393">响应数据</span><span class="sxs-lookup"><span data-stu-id="e60c5-393">Response data</span></span> | <span data-ttu-id="e60c5-394">说明</span><span class="sxs-lookup"><span data-stu-id="e60c5-394">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e60c5-395">成功代码</span><span class="sxs-lookup"><span data-stu-id="e60c5-395">Success code</span></span> | <span data-ttu-id="e60c5-396">200 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-396">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="e60c5-397">响应正文</span><span class="sxs-lookup"><span data-stu-id="e60c5-397">Response body</span></span> | <span data-ttu-id="e60c5-398">以 JSON 格式设置的实体或实体的 OData 表示，页面 HTML 或文件资源二进制数据。</span><span class="sxs-lookup"><span data-stu-id="e60c5-398">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="e60c5-399">错误</span><span class="sxs-lookup"><span data-stu-id="e60c5-399">Errors</span></span> | <span data-ttu-id="e60c5-400">如果请求失败，API 将在响应正文的 **@api.diagnostics** 对象中返回[错误](onenote-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-400">If the request fails, the API returns [errors](onenote-error-codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="e60c5-401">X-CorrelationId 标头</span><span class="sxs-lookup"><span data-stu-id="e60c5-401">X-CorrelationId header</span></span> | <span data-ttu-id="e60c5-402">唯一标识该请求的 GUID。</span><span class="sxs-lookup"><span data-stu-id="e60c5-402">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="e60c5-403">在与 Microsoft 支持部门协作来解决问题时，可以使用此值和日期标头值。</span><span class="sxs-lookup"><span data-stu-id="e60c5-403">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="e60c5-404">构建 Microsoft Graph 笔记服务根 URL</span><span class="sxs-lookup"><span data-stu-id="e60c5-404">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="e60c5-405">Microsoft Graph 笔记根 URL 为 Microsoft Graph 笔记的所有调用使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="e60c5-405">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="e60c5-406">URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。</span><span class="sxs-lookup"><span data-stu-id="e60c5-406">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="e60c5-407">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-407">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="e60c5-408">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="e60c5-408">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="e60c5-409">Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。</span><span class="sxs-lookup"><span data-stu-id="e60c5-409">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="e60c5-410">为当前用户可以访问的 OneNote 内容（拥有和共享）使用 `me`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-410">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="e60c5-411">为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）使用 `users/{id}`。</span><span class="sxs-lookup"><span data-stu-id="e60c5-411">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="e60c5-412">使用 [Microsoft Graph](https://graph.microsoft.com/v1.0/users) 获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="e60c5-412">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="e60c5-413">GET 请求的权限</span><span class="sxs-lookup"><span data-stu-id="e60c5-413">Permissions for GET requests</span></span>

<span data-ttu-id="e60c5-414">若要获取 OneNote 内容或结构，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="e60c5-414">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="e60c5-415">以下范围允许对 Microsoft Graph 执行 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="e60c5-415">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="e60c5-416">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="e60c5-416">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="e60c5-417">从以下项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="e60c5-417">Choose from:</span></span>

- <span data-ttu-id="e60c5-418">Notes.read</span><span class="sxs-lookup"><span data-stu-id="e60c5-418">Notes.read</span></span>
- <span data-ttu-id="e60c5-419">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e60c5-419">Notes.ReadWrite</span></span>
- <span data-ttu-id="e60c5-420">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e60c5-420">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e60c5-421">有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e60c5-421">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="e60c5-422">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e60c5-422">See also</span></span>

- [<span data-ttu-id="e60c5-423">OneNote 页面的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="e60c5-423">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="e60c5-424">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="e60c5-424">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="e60c5-425">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="e60c5-425">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e60c5-426">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="e60c5-426">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="e60c5-427">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="e60c5-427">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
