# <a name="update-onenote-page-content"></a><span data-ttu-id="74614-101">更新 OneNote 页面内容</span><span class="sxs-lookup"><span data-stu-id="74614-101">Update OneNote page content</span></span>

<span data-ttu-id="74614-102">*__适用于：__ OneDrive 上的消费者笔记本 | Office 365 上的企业级笔记本*</span><span class="sxs-lookup"><span data-stu-id="74614-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>


<span data-ttu-id="74614-103">若要更新 OneNote 页面的内容，请向此页面的 *content* 终结点发送 PATCH 请求：</span><span class="sxs-lookup"><span data-stu-id="74614-103">To retrieve the HTML content of a onnvshort page, you send a GET request to  the page's content endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="74614-104">在邮件正文中发送 JSON 更改对象。</span><span class="sxs-lookup"><span data-stu-id="74614-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="74614-105">如果请求成功，Microsoft Graph 将返回 204 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="74614-105">If the create request is successful, the onnvshort API returns a 201 HTTP status code.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="74614-106">构建请求 URI</span><span class="sxs-lookup"><span data-stu-id="74614-106">Construct the request</span></span>

<span data-ttu-id="74614-107">若要构建请求 URI，请从服务根 URL 开始：</span><span class="sxs-lookup"><span data-stu-id="74614-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="74614-108">然后，追加页面的 *content* 终结点：</span><span class="sxs-lookup"><span data-stu-id="74614-108">Then append the page's *content* endpoint:</span></span>

<span data-ttu-id="74614-109">**获取页面 HTML 和所有定义的 *data-id* 值**</span><span class="sxs-lookup"><span data-stu-id="74614-109">**Get the page HTML and all defined *data-id* values**</span></span></p>
`../pages/{id}/content`   

<span data-ttu-id="74614-110">**获取页面 HTML、所有定义的 *data-id* 值和所有生成的 *id* 值**</span><span class="sxs-lookup"><span data-stu-id="74614-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span>  
`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="74614-111">**data-id** 和 **id** 值均用作要更新的元素的 **target** 标识符。</span><span class="sxs-lookup"><span data-stu-id="74614-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="74614-112">完整的请求 URI 将如下所示：</span><span class="sxs-lookup"><span data-stu-id="74614-112">Your full request URI will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="74614-113">了解有关[服务根 URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="74614-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="74614-114">构造邮件正文</span><span class="sxs-lookup"><span data-stu-id="74614-114">Construct the message body</span></span>

<span data-ttu-id="74614-115">OneNote 页面的 HTML 包含文本、图像和组织到结构中的其他内容，如 **div**、**img** 和 **ol** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-115">The HTML of a onnvshort page contains text, images, and other content organized into structures such as div, img, and ol elements. To update page HTML, you send a PATCH request to the page's content endpoint:</span></span> <span data-ttu-id="74614-116">若要更新 OneNote 页面内容，请添加并替换页面上的 HTML 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="74614-117">所做的更改将以 JSON 更改对象数组的形式在邮件正文中发送。</span><span class="sxs-lookup"><span data-stu-id="74614-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="74614-118">每个对象指定目标元素、新 HTML 内容以及使用内容可完成的操作。</span><span class="sxs-lookup"><span data-stu-id="74614-118">Your changes are sent in the request body as an array of JSON objects. Each object specifies the target element,  new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="74614-p104">以下数组定义了两个更改。第一个更改在段落上方插入一张图像作为同级对象，第二个更改向列表中附加一个项目作为最后一个子元素。</span><span class="sxs-lookup"><span data-stu-id="74614-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="74614-121">请参阅[更多示例](#example-requests)。</span><span class="sxs-lookup"><span data-stu-id="74614-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="74614-122">JSON 更改对象的属性</span><span class="sxs-lookup"><span data-stu-id="74614-122">Attributes for JSON objects</span></span>

<span data-ttu-id="74614-123">使用 **target**、**action**、**position** 和 **content** 属性来定义用于 PATCH 请求的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="74614-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

<span data-ttu-id="74614-124">**target**</span><span class="sxs-lookup"><span data-stu-id="74614-124">**target**</span></span>  
<span data-ttu-id="74614-p105">要更新的元素。值必须是下列标识符之一：</span><span class="sxs-lookup"><span data-stu-id="74614-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="74614-127">标示符</span><span class="sxs-lookup"><span data-stu-id="74614-127">Identifier</span></span> | <span data-ttu-id="74614-128">说明</span><span class="sxs-lookup"><span data-stu-id="74614-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="74614-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="74614-129">data-id</span></span> | <p><span data-ttu-id="74614-130">在[创建页面](onenote-create-page.md)或[更新页面](onenote_update_page.md)时，可以选择在输入 HTML 中的元素上定义此 ID。</span><span class="sxs-lookup"><span data-stu-id="74614-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="74614-131">将 # 用作此值的前缀。</span><span class="sxs-lookup"><span data-stu-id="74614-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="74614-132">示例：`'target':'#intro'` 以元素 `<div data-id="intro" ...>` 为目标</span><span class="sxs-lookup"><span data-stu-id="74614-132">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="74614-133">id</span><span class="sxs-lookup"><span data-stu-id="74614-133">id</span></span> | <p><span data-ttu-id="74614-134">这是从 Microsoft Graph [生成的 ID](#generated-ids)，对大多数替换操作所都是必需的值。</span><span class="sxs-lookup"><span data-stu-id="74614-134">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="74614-135">不要使用 # 作为前缀。</span><span class="sxs-lookup"><span data-stu-id="74614-135">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="74614-136">示例：`'target':'div:{33f8a2...}{37}'` 以元素 `<div id="div:{33f8a2...}{37}" ...>` 为目标</span><span class="sxs-lookup"><span data-stu-id="74614-136">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="74614-137">不要将其与[输入 HTML](onenote_input_output_html.md) 中定义的任何 **id** 值混淆。</span><span class="sxs-lookup"><span data-stu-id="74614-137">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="74614-138">所有在输入 HTML 中发送的 **id** 值都将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="74614-138">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="74614-139">body</span><span class="sxs-lookup"><span data-stu-id="74614-139">body</span></span> | <span data-ttu-id="74614-140">针对页面上第一个 div 的关键字。</span><span class="sxs-lookup"><span data-stu-id="74614-140">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="74614-141">不要使用 # 作为前缀。</span><span class="sxs-lookup"><span data-stu-id="74614-141">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="74614-142">title</span><span class="sxs-lookup"><span data-stu-id="74614-142">title</span></span> | <span data-ttu-id="74614-143">针对页标题的关键字。</span><span class="sxs-lookup"><span data-stu-id="74614-143">The keyword that targets the page title.</span></span> <span data-ttu-id="74614-144">不要使用 # 作为前缀。</span><span class="sxs-lookup"><span data-stu-id="74614-144">Do not prefix with a #.</span></span> |  
 
<span data-ttu-id="74614-145">**action**</span><span class="sxs-lookup"><span data-stu-id="74614-145">**action**</span></span>  
<span data-ttu-id="74614-146">要在目标元素上执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74614-146">The action to perform on the target element. Possible values are: , , , , or .</span></span> <span data-ttu-id="74614-147">请参阅[元素支持的操作](#supported-elements-and-actions)。</span><span class="sxs-lookup"><span data-stu-id="74614-147">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="74614-148">操作</span><span class="sxs-lookup"><span data-stu-id="74614-148">Action</span></span> | <span data-ttu-id="74614-149">说明</span><span class="sxs-lookup"><span data-stu-id="74614-149">Description</span></span> |  
|------|------|  
| <span data-ttu-id="74614-150">append</span><span class="sxs-lookup"><span data-stu-id="74614-150">Append</span></span> | <p><span data-ttu-id="74614-151">将提供的内容作为第一个或最后一个子元素添加到由 **position** 属性所确定的目标。</span><span class="sxs-lookup"><span data-stu-id="74614-151">**append**Adds the supplied content to the target as a first or last child, as determined by the position attribute.Applies only to body, div, ol, and ul elements.</span></span></p><p><span data-ttu-id="74614-152">仅适用于 **body**、**div**、**ol** 和 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-152">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="74614-153">insert</span><span class="sxs-lookup"><span data-stu-id="74614-153">insert</span></span> | <span data-ttu-id="74614-154">将提供的内容作为同级元素添加到由 **position** 属性确定的目标之前或之后。</span><span class="sxs-lookup"><span data-stu-id="74614-154">**insert**Adds the supplied content as a sibling before or after the target, as determined by the position attribute.</span></span> |  
| <span data-ttu-id="74614-155">prepend</span><span class="sxs-lookup"><span data-stu-id="74614-155">prepend</span></span> | <p><span data-ttu-id="74614-156">将提供的内容作为第一个子元素添加到目标。</span><span class="sxs-lookup"><span data-stu-id="74614-156">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="74614-157">**append** + **before** 的快捷方式。</span><span class="sxs-lookup"><span data-stu-id="74614-157">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="74614-158">仅适用于 **body**、**div**、**ol** 和 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-158">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="74614-159">replace</span><span class="sxs-lookup"><span data-stu-id="74614-159">replace</span></span> | <p><span data-ttu-id="74614-160">使用提供的内容替换目标。</span><span class="sxs-lookup"><span data-stu-id="74614-160">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="74614-161">大多数**替换**操作需要为目标使用[生成的 ID](#generated-ids)（除 div 中的 **img** 和 **object** 元素之外，还支持使用 **data-id**）。</span><span class="sxs-lookup"><span data-stu-id="74614-161">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
<span data-ttu-id="74614-162">**position**</span><span class="sxs-lookup"><span data-stu-id="74614-162">**position**</span></span>  
<span data-ttu-id="74614-163">要添加所提供内容的位置，与目标元素相对。</span><span class="sxs-lookup"><span data-stu-id="74614-163">The location to add the supplied content, relative to the target element. Possible values are:  (default) or .</span></span> <span data-ttu-id="74614-164">如果省略，默认值为 **after**。</span><span class="sxs-lookup"><span data-stu-id="74614-164">Defaults to **render** if omitted.</span></span>

| <span data-ttu-id="74614-165">位置</span><span class="sxs-lookup"><span data-stu-id="74614-165">Position</span></span> | <span data-ttu-id="74614-166">说明</span><span class="sxs-lookup"><span data-stu-id="74614-166">Description</span></span> |  
|------|------|  
| <span data-ttu-id="74614-167">after（默认）</span><span class="sxs-lookup"><span data-stu-id="74614-167">after (default)</span></span> | <p><span data-ttu-id="74614-168">- 使用 **append**：目标元素的最后一个子元素。</span><span class="sxs-lookup"><span data-stu-id="74614-168">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="74614-169">- 使用 **insert**：目标元素的后续同级元素。</span><span class="sxs-lookup"><span data-stu-id="74614-169">**after** (default)- With append: The last child of the target element.- With insert: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="74614-170">before</span><span class="sxs-lookup"><span data-stu-id="74614-170">Before</span></span> | <p><span data-ttu-id="74614-171">- 使用 **append**：目标元素的第一个子元素。</span><span class="sxs-lookup"><span data-stu-id="74614-171">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="74614-172">- 使用 **insert**：目标元素的前导同级元素。</span><span class="sxs-lookup"><span data-stu-id="74614-172">**before**- With append: The first child of the target element.- With insert: The preceding sibling of the target element.</span></span></p> |

<span data-ttu-id="74614-173">**content**</span><span class="sxs-lookup"><span data-stu-id="74614-173">**content**</span></span>  
<span data-ttu-id="74614-174">要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。</span><span class="sxs-lookup"><span data-stu-id="74614-174">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the  content type with a "Commands" part.</span></span> <span data-ttu-id="74614-175">如果内容包含二进制数据，则必须使用包含“Commands”部件的 `multipart/form-data` 内容类型发送请求（请参阅[示例](#multipart-request-with-binary-content)）。</span><span class="sxs-lookup"><span data-stu-id="74614-175">A string of well-formed HTML to add to the page and any image or file binary data. If the content contains binary data, the request must be sent using the multipart/form-data`multipart/form-data` content type with a "Commands" part (see an  [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="74614-176">生成的 ID</span><span class="sxs-lookup"><span data-stu-id="74614-176">Generated IDs</span></span>
<span data-ttu-id="74614-177">Microsoft Graph 将为可更新页面上的元素生成 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="74614-177">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="74614-178">若要获取生成的 ID，请在 GET 请求中使用 `includeIDs=true` 查询字符串表达式：</span><span class="sxs-lookup"><span data-stu-id="74614-178">The onnvshort API generates id`includeIDs=true` values for page elements that can be updated. To get generated IDs, use the includeIDs=true query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="74614-179">**注意：** API 会放弃在创建页面和更新页面请求的[输入 HTML](onenote_input_output_html.md) 中定义的所有 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="74614-179">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="74614-180">以下示例显示了段落的生成 ID，以及页面的[输出 HTML](onenote_input_output_html.md) 中的图像。</span><span class="sxs-lookup"><span data-stu-id="74614-180">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="74614-181">页面更新后，生成的 **id** 值可能会更改，因此您应该在构建使用当前值的 PATCH 请求之前获取当前值。</span><span class="sxs-lookup"><span data-stu-id="74614-181">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="74614-182">可以使用 **data-id** 或 **id** 值指定目标元素，如下所示：</span><span class="sxs-lookup"><span data-stu-id="74614-182">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="74614-183">对于 **append** 和 **insert** 操作，可以使用任一 ID 作为目标值。</span><span class="sxs-lookup"><span data-stu-id="74614-183">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="74614-184">对于 **replace** 操作，必须为除页标题及 div 中的图像和对象之外的所有元素使用生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="74614-184">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div. To replace a title, use the title keyword. To replace images and objects that are within a div, use either data-id or id.</span></span> 
    - <span data-ttu-id="74614-185">若要替换标题，请使用 **title** 关键字。</span><span class="sxs-lookup"><span data-stu-id="74614-185">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="74614-186">若要替换 div 中的图像和对象，请使用 **data-id** 或 **id**。</span><span class="sxs-lookup"><span data-stu-id="74614-186">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="74614-187">以下示例为目标使用了 **id** 值。</span><span class="sxs-lookup"><span data-stu-id="74614-187">The following example uses the **id** value for the target . Don't use the # prefix with a generated ID.</span></span> <span data-ttu-id="74614-188">不要将 # 前缀用于生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="74614-188">The following example uses the id value for the target . Don't use the # prefix with a generated ID.</span></span>

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a><span data-ttu-id="74614-189">受支持的元素和操作</span><span class="sxs-lookup"><span data-stu-id="74614-189">Supported elements and actions</span></span>
<span data-ttu-id="74614-190">可以更新页面上的许多元素，但每个元素类型支持特定操作。</span><span class="sxs-lookup"><span data-stu-id="74614-190">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span> <span data-ttu-id="74614-191">下表显示了支持的目标元素和它们支持的更新操作。</span><span class="sxs-lookup"><span data-stu-id="74614-191">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="74614-192">元素</span><span class="sxs-lookup"><span data-stu-id="74614-192">Element</span></span> | <span data-ttu-id="74614-193">替换</span><span class="sxs-lookup"><span data-stu-id="74614-193">Replace</span></span> | <span data-ttu-id="74614-194">附加子元素</span><span class="sxs-lookup"><span data-stu-id="74614-194">Append child</span></span> | <span data-ttu-id="74614-195">插入同级元素</span><span class="sxs-lookup"><span data-stu-id="74614-195">Insert sibling</span></span> |  
|------|------|------|------|  
| <span data-ttu-id="74614-196">body</span><span class="sxs-lookup"><span data-stu-id="74614-196">body</span></span><br /> <span data-ttu-id="74614-197">（目标为页面上的第一个 div）</span><span class="sxs-lookup"><span data-stu-id="74614-197">body(targets first div on the page)</span></span> | <span data-ttu-id="74614-198">否</span><span class="sxs-lookup"><span data-stu-id="74614-198">no</span></span> | <span data-ttu-id="74614-199">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-199">**yes**</span></span> | <span data-ttu-id="74614-200">否</span><span class="sxs-lookup"><span data-stu-id="74614-200">no</span></span> |  
| <span data-ttu-id="74614-201">div</span><span class="sxs-lookup"><span data-stu-id="74614-201">div</span></span><br /> <span data-ttu-id="74614-202">（[绝对定位](onenote-abs-pos.md)）</span><span class="sxs-lookup"><span data-stu-id="74614-202">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="74614-203">否</span><span class="sxs-lookup"><span data-stu-id="74614-203">no</span></span> | <span data-ttu-id="74614-204">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-204">**yes**</span></span> | <span data-ttu-id="74614-205">否</span><span class="sxs-lookup"><span data-stu-id="74614-205">no</span></span> |  
| <span data-ttu-id="74614-206">div</span><span class="sxs-lookup"><span data-stu-id="74614-206">div</span></span><br /> <span data-ttu-id="74614-207">（在 div 中）</span><span class="sxs-lookup"><span data-stu-id="74614-207">(within a div)</span></span> | <span data-ttu-id="74614-208">**是**（仅 ID）</span><span class="sxs-lookup"><span data-stu-id="74614-208">**yes** (id only)</span></span> | <span data-ttu-id="74614-209">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-209">**Yes**</span></span> | <span data-ttu-id="74614-210">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-210">**Yes**</span></span> |   
| <span data-ttu-id="74614-211">img, object</span><span class="sxs-lookup"><span data-stu-id="74614-211">img, object</span></span><br /> <span data-ttu-id="74614-212">（在 div 中）</span><span class="sxs-lookup"><span data-stu-id="74614-212">(within a div)</span></span> | <span data-ttu-id="74614-213">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-213">**yes**</span></span> | <span data-ttu-id="74614-214">否</span><span class="sxs-lookup"><span data-stu-id="74614-214">no</span></span> | <span data-ttu-id="74614-215">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-215">**yes**</span></span> |   
| <span data-ttu-id="74614-216">ol, ul</span><span class="sxs-lookup"><span data-stu-id="74614-216">ol, ul</span></span> | <span data-ttu-id="74614-217">**是**（仅 ID）</span><span class="sxs-lookup"><span data-stu-id="74614-217">**yes** (id only)</span></span> | <span data-ttu-id="74614-218">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-218">**Yes**</span></span> | <span data-ttu-id="74614-219">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-219">**yes**</span></span> |   
| <span data-ttu-id="74614-220">table</span><span class="sxs-lookup"><span data-stu-id="74614-220">table</span></span> | <span data-ttu-id="74614-221">**是**（仅 ID）</span><span class="sxs-lookup"><span data-stu-id="74614-221">**yes** (id only)</span></span> | <span data-ttu-id="74614-222">否</span><span class="sxs-lookup"><span data-stu-id="74614-222">no</span></span> | <span data-ttu-id="74614-223">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-223">**yes**</span></span> |   
| <span data-ttu-id="74614-224">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="74614-224">p, li, h1-h6</span></span> | <span data-ttu-id="74614-225">**是**（仅 ID）</span><span class="sxs-lookup"><span data-stu-id="74614-225">**yes** (id only)</span></span> | <span data-ttu-id="74614-226">否</span><span class="sxs-lookup"><span data-stu-id="74614-226">no</span></span> | <span data-ttu-id="74614-227">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-227">**yes**</span></span> |   
| <span data-ttu-id="74614-228">title</span><span class="sxs-lookup"><span data-stu-id="74614-228">title</span></span> | <span data-ttu-id="74614-229">**是**</span><span class="sxs-lookup"><span data-stu-id="74614-229">**yes**</span></span> | <span data-ttu-id="74614-230">否</span><span class="sxs-lookup"><span data-stu-id="74614-230">no</span></span> | <span data-ttu-id="74614-231">否</span><span class="sxs-lookup"><span data-stu-id="74614-231">no</span></span> |  
 

<span data-ttu-id="74614-232">以下元素不支持任何更新操作。</span><span class="sxs-lookup"><span data-stu-id="74614-232">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="74614-233">img（[绝对定位](onenote-abs-pos.md)）</span><span class="sxs-lookup"><span data-stu-id="74614-233">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="74614-234">object（[绝对定位](onenote-abs-pos.md)）</span><span class="sxs-lookup"><span data-stu-id="74614-234">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="74614-235">tr, td</span><span class="sxs-lookup"><span data-stu-id="74614-235">tr, td</span></span>
- <span data-ttu-id="74614-236">meta</span><span class="sxs-lookup"><span data-stu-id="74614-236">meta</span></span>
- <span data-ttu-id="74614-237">head</span><span class="sxs-lookup"><span data-stu-id="74614-237">head</span></span>
- <span data-ttu-id="74614-238">span</span><span class="sxs-lookup"><span data-stu-id="74614-238">span</span></span>
- <span data-ttu-id="74614-239">a</span><span class="sxs-lookup"><span data-stu-id="74614-239">a</span></span>
- <span data-ttu-id="74614-240">style tags</span><span class="sxs-lookup"><span data-stu-id="74614-240">style tags</span></span>


<a name="examples"></a>
## <a name="example-requests"></a><span data-ttu-id="74614-241">示例请求</span><span class="sxs-lookup"><span data-stu-id="74614-241">Example requests</span></span>
<span data-ttu-id="74614-242">更新请求包含表示为 JSON 更改对象的一个或多个更改。</span><span class="sxs-lookup"><span data-stu-id="74614-242">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="74614-243">这些对象可以定义页面上的不同目标，以及定义目标的不同操作和内容。</span><span class="sxs-lookup"><span data-stu-id="74614-243">An update request contains one or more changes represented as JSON objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="74614-244">以下示例包括 PATCH 请求中使用的 JSON 对象和完整的 PATCH 请求：</span><span class="sxs-lookup"><span data-stu-id="74614-244">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

<span data-ttu-id="74614-245">[追加子元素](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[插入同级元素](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[替换元素](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[完整的 PATCH 请求](#complete-patch-request-examples)</span><span class="sxs-lookup"><span data-stu-id="74614-245">[Append child elements](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Insert sibling elements](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Replace elements](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Complete PATCH requests](#complete-patch-request-examples)</span></span>


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="74614-246">追加子元素</span><span class="sxs-lookup"><span data-stu-id="74614-246">Append  child elements</span></span>
<span data-ttu-id="74614-247">**append** 操作将子元素添加到 **body**、**div**（在 div 中）、**ol** 或 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-247">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The position attribute determines whether to append the child before or after the target. The default position is after.</span></span> <span data-ttu-id="74614-248">**position** 属性确定要将子元素追加到目标之前还是之后。</span><span class="sxs-lookup"><span data-stu-id="74614-248">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="74614-249">默认位置是 **after**。</span><span class="sxs-lookup"><span data-stu-id="74614-249">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="74614-250">追加到 div</span><span class="sxs-lookup"><span data-stu-id="74614-250">Append to a  div</span></span>

<span data-ttu-id="74614-251">以下示例将两个子节点添加到 **div1** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-251">The following example adds two child nodes  to the **div1** element. It adds an image as the first child and a paragraph as the last child.</span></span> <span data-ttu-id="74614-252">它添加图像作为第一个子元素，添加段落作为最后一个子元素。</span><span class="sxs-lookup"><span data-stu-id="74614-252">The following example adds two child nodes  to the div1 element. It adds an image as the first child and a paragraph as the last child.</span></span> 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="74614-253">追加到 *body* 元素</span><span class="sxs-lookup"><span data-stu-id="74614-253">Append to the body element</span></span>

<span data-ttu-id="74614-254">可以使用 **body** 快捷方式来追加任何页面上的第一个 div 内的子元素。</span><span class="sxs-lookup"><span data-stu-id="74614-254">You can use the body target as a shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="74614-255">以下示例将两个段落作为第一个子元素和最后一个子元素添加到页面上第一个 div。</span><span class="sxs-lookup"><span data-stu-id="74614-255">The following example adds two paragraphs as the first child and the last child to the first div on the page. Don't use a # with the body target. This example uses the prepend shortcut for append + before.</span></span> <span data-ttu-id="74614-256">不要将 # 用于 **body** 目标。</span><span class="sxs-lookup"><span data-stu-id="74614-256">Don't use a # with the **body** target.</span></span> <span data-ttu-id="74614-257">此示例使用 **prepend** 操作作为 **append** + **before** 的快捷方式。</span><span class="sxs-lookup"><span data-stu-id="74614-257">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a><span data-ttu-id="74614-258">追加到列表</span><span class="sxs-lookup"><span data-stu-id="74614-258">Append to a list</span></span>

<span data-ttu-id="74614-259">以下示例将列表项作为最后一个子元素添加到目标列表。</span><span class="sxs-lookup"><span data-stu-id="74614-259">The following example adds a list item as a last child to the target list. The list-style-type property is defined because the item uses a non-default list style.</span></span> <span data-ttu-id="74614-260">定义了 **list-style-type** 属性，因为项使用非默认列表样式。</span><span class="sxs-lookup"><span data-stu-id="74614-260">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a><span data-ttu-id="74614-261">插入同级元素</span><span class="sxs-lookup"><span data-stu-id="74614-261">Insert sibling elements</span></span>
<span data-ttu-id="74614-262">**insert** 操作将同级元素添加到目标元素。</span><span class="sxs-lookup"><span data-stu-id="74614-262">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="74614-263">**position** 属性确定要将同级元素插入到目标之前还是之后。</span><span class="sxs-lookup"><span data-stu-id="74614-263">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="74614-264">默认位置是 **after**。</span><span class="sxs-lookup"><span data-stu-id="74614-264">The default position is **after**.</span></span> <span data-ttu-id="74614-265">请参阅[支持**插入**](#supported-elements-and-actions)的元素。</span><span class="sxs-lookup"><span data-stu-id="74614-265">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

<span data-ttu-id="74614-266">**插入同级元素**</span><span class="sxs-lookup"><span data-stu-id="74614-266">**Insert siblings**</span></span>

<span data-ttu-id="74614-267">以下示例将两个同级节点添加到页面。</span><span class="sxs-lookup"><span data-stu-id="74614-267">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="74614-268">它会添加 **para1** 元素上面的图像和 **para2** 元素下面的段落。</span><span class="sxs-lookup"><span data-stu-id="74614-268">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="74614-269">替换元素</span><span class="sxs-lookup"><span data-stu-id="74614-269">Replace elements</span></span>

<span data-ttu-id="74614-270">可以使用 **data-id** 或生成的 **id** 作为目标值来替换 div 中的 **img** 和 **object** 元素。</span><span class="sxs-lookup"><span data-stu-id="74614-270">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div. To replace the page title, use the title keyword. For all other elements that support replace, you must use the generated ID.</span></span> <span data-ttu-id="74614-271">若要替换页标题，请使用 **title** 关键字。</span><span class="sxs-lookup"><span data-stu-id="74614-271">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="74614-272">对于所有其他[支持**替换**](#supported-elements-and-actions)的元素，必须使用生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="74614-272">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="74614-273">替换图像</span><span class="sxs-lookup"><span data-stu-id="74614-273">Replace an image</span></span>

<span data-ttu-id="74614-274">以下示例使用图像的 **data-id** 作为目标来替换 div 中的图像。</span><span class="sxs-lookup"><span data-stu-id="74614-274">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="74614-275">更新表格</span><span class="sxs-lookup"><span data-stu-id="74614-275">Update a table</span></span> 

<span data-ttu-id="74614-276">此示例说明如何使用其生成的 ID 来更新表格。</span><span class="sxs-lookup"><span data-stu-id="74614-276">This example shows how to update a table by using its generated ID. Replacing tr and td elements is not supported, but you can replace the entire table.</span></span> <span data-ttu-id="74614-277">不支持替换 **tr** 和 **td** 元素，但可以替换整个表。</span><span class="sxs-lookup"><span data-stu-id="74614-277">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a><span data-ttu-id="74614-278">更改标题</span><span class="sxs-lookup"><span data-stu-id="74614-278">Change the title</span></span> 

<span data-ttu-id="74614-279">此示例说明如何更改页面的标题。</span><span class="sxs-lookup"><span data-stu-id="74614-279">This example shows how to change the title of a page.</span></span> <span data-ttu-id="74614-280">若要更改标题，请使用 **title** 关键字作为目标值。</span><span class="sxs-lookup"><span data-stu-id="74614-280">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="74614-281">不要将 # 用于标题目标。</span><span class="sxs-lookup"><span data-stu-id="74614-281">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="74614-282">更新待办事项</span><span class="sxs-lookup"><span data-stu-id="74614-282">Update a to-do item</span></span>

<span data-ttu-id="74614-283">以下示例使用替换操作将待办事项复选框项更改为完成状态。</span><span class="sxs-lookup"><span data-stu-id="74614-283">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="74614-284">有关使用 **data-tag** 属性的详细信息，请参阅[使用注释标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="74614-284">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="74614-285">完整的 PATCH 请求示例</span><span class="sxs-lookup"><span data-stu-id="74614-285">Complete PATCH request examples</span></span>

<span data-ttu-id="74614-286">以下示例显示了完整的 PATCH 请求。</span><span class="sxs-lookup"><span data-stu-id="74614-286">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="74614-287">仅包含文本内容的请求</span><span class="sxs-lookup"><span data-stu-id="74614-287">Request with text content only</span></span>  
<span data-ttu-id="74614-288">以下示例显示使用 **application/json** 内容类型的 PATCH 请求。</span><span class="sxs-lookup"><span data-stu-id="74614-288">The following example shows a PATCH request that uses the   **application/json** content type. You can use this format when your content doesn't contain binary data.</span></span> <span data-ttu-id="74614-289">内容不包含二进制数据时，可使用此格式。</span><span class="sxs-lookup"><span data-stu-id="74614-289">The following example shows a PATCH request that uses the   application/json content type. You can use this format when your content doesn't contain binary data.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="74614-290">包含二进制内容的多部分请求</span><span class="sxs-lookup"><span data-stu-id="74614-290">Multipart request with binary content</span></span> 

<span data-ttu-id="74614-291">以下示例显示包含二进制数据的多部分 PATCH 请求。</span><span class="sxs-lookup"><span data-stu-id="74614-291">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="74614-292">多部分请求需要指定 **application/json** 内容类型并包含 JSON 更改对象数组的“Commands”部件。</span><span class="sxs-lookup"><span data-stu-id="74614-292">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="74614-293">其他数据部件可包含二进制数据。</span><span class="sxs-lookup"><span data-stu-id="74614-293">Other data parts can contain binary data.</span></span> <span data-ttu-id="74614-294">部件名称通常是附加有毫秒为单位或随机 GUID 当前时间的字符串。</span><span class="sxs-lookup"><span data-stu-id="74614-294">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="74614-295">PATCH 请求的请求和响应信息</span><span class="sxs-lookup"><span data-stu-id="74614-295">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="74614-296">请求数据</span><span class="sxs-lookup"><span data-stu-id="74614-296">Request data</span></span> | <span data-ttu-id="74614-297">说明</span><span class="sxs-lookup"><span data-stu-id="74614-297">Description</span></span> |  
|------|------|  
| <span data-ttu-id="74614-298">协议</span><span class="sxs-lookup"><span data-stu-id="74614-298">Protocol</span></span> | <span data-ttu-id="74614-299">所有请求均使用 SSL/TLS HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="74614-299">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="74614-300">授权标头</span><span class="sxs-lookup"><span data-stu-id="74614-300">Authorization header</span></span> | <p><span data-ttu-id="74614-301">`Bearer {token}`，其中 *{token}* 是已注册应用的一个有效 OAuth 2.0 访问令牌。</span><span class="sxs-lookup"><span data-stu-id="74614-301">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="74614-302">如果缺少或无效，则请求失败，并显示 401 状态代码。</span><span class="sxs-lookup"><span data-stu-id="74614-302">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="74614-303">请参阅[身份验证和权限](permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="74614-303">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="74614-304">Content-Type 标头</span><span class="sxs-lookup"><span data-stu-id="74614-304">content-type header</span></span> | <p><span data-ttu-id="74614-305">JSON 更改对象的数组的 `application/json`，确定是直接在邮件正文中发送还是在必须的[多部分请求](#multipart-request-with-binary-content)的“Commands”部件中发送。</span><span class="sxs-lookup"><span data-stu-id="74614-305">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="74614-306">发送二进制数据时，多部分请求是必需的，并使用 `multipart/form-data; boundary=part-boundary` 内容类型，其中 *{part-boundary}* 是一个字符串，表示每个数据部件的开始和结束。</span><span class="sxs-lookup"><span data-stu-id="74614-306">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
 

| <span data-ttu-id="74614-307">响应数据</span><span class="sxs-lookup"><span data-stu-id="74614-307">Response data</span></span> | <span data-ttu-id="74614-308">说明</span><span class="sxs-lookup"><span data-stu-id="74614-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="74614-309">成功代码</span><span class="sxs-lookup"><span data-stu-id="74614-309">Success code</span></span> | <span data-ttu-id="74614-p131">204 HTTP 状态代码。PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="74614-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="74614-312">错误</span><span class="sxs-lookup"><span data-stu-id="74614-312">Errors</span></span> | <span data-ttu-id="74614-313">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote_error_codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="74614-313">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="74614-314">构建 Microsoft Graph 服务根 URL</span><span class="sxs-lookup"><span data-stu-id="74614-314">Constructing the Microsoft Graph service root URL</span></span>

<a name="root-url"></a>

## <a name="root-url"></a><span data-ttu-id="74614-315">根 URL</span><span class="sxs-lookup"><span data-stu-id="74614-315">URL Root</span></span>
<span data-ttu-id="74614-316">OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。</span><span class="sxs-lookup"><span data-stu-id="74614-316">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="74614-317">URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。</span><span class="sxs-lookup"><span data-stu-id="74614-317">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>
- <span data-ttu-id="74614-318">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="74614-318">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="74614-319">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="74614-319">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="74614-320">Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。</span><span class="sxs-lookup"><span data-stu-id="74614-320">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>
- <span data-ttu-id="74614-321">`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。</span><span class="sxs-lookup"><span data-stu-id="74614-321">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="74614-322">`users/{id}` 用于为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。</span><span class="sxs-lookup"><span data-stu-id="74614-322">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="74614-323">使用 [Azure AD 图形 API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="74614-323">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="74614-324">**注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="74614-324">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="74614-325">权限</span><span class="sxs-lookup"><span data-stu-id="74614-325">Permissions</span></span>

<span data-ttu-id="74614-326">若要更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="74614-326">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="74614-327">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="74614-327">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="74614-328">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74614-328">Notes.ReadWrite</span></span>
- <span data-ttu-id="74614-329">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74614-329">Notes.ReadWrite.All</span></span>

<span data-ttu-id="74614-330">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="74614-330">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="additional-resources"></a><span data-ttu-id="74614-331">其他资源</span><span class="sxs-lookup"><span data-stu-id="74614-331">Additional resources</span></span>

- [<span data-ttu-id="74614-332">添加图像和文件</span><span class="sxs-lookup"><span data-stu-id="74614-332">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="74614-333">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="74614-333">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="74614-334">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="74614-334">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="74614-335">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="74614-335">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="74614-336">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="74614-336">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
