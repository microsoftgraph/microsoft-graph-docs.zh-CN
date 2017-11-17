# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="5ab73-101">OneNote 页中的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="5ab73-101">Input and output HTML for OneNote pages</span></span>

<span data-ttu-id="5ab73-102">[创建](../api-reference/v1.0/api/section_post_pages.md)或[更新](../api-reference/v1.0/api/page_update.md) OneNote 页时定义页面内容和结构的 HTML 被称为*输入 HTML*。</span><span class="sxs-lookup"><span data-stu-id="5ab73-102">The HTML that defines the page content and structure when you [create](../api-reference/v1.0/api/section_post_pages.md) or [update](../api-reference/v1.0/api/page_update.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="5ab73-103">[获取页面内容](../api-reference/v1.0/api/page_get.md)时返回的 HTML 被称为*输出 HTML*。</span><span class="sxs-lookup"><span data-stu-id="5ab73-103">The HTML that's returned when you [get page content](../api-reference/v1.0/api/page_get.md) is called *output HTML*.</span></span> <span data-ttu-id="5ab73-104">输出 HTML 与输入 HTML 存在差别。</span><span class="sxs-lookup"><span data-stu-id="5ab73-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="5ab73-105">Microsoft Graph 中的 OneNote API 保留输入 HTML 的语义内容和基本结构，但会将其转换为一组[受支持的 HTML 元素和 CSS 属性](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span></span> <span data-ttu-id="5ab73-106">API 还添加支持 OneNote 功能的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="5ab73-107">本文介绍输入和输出 HTML 的主体元素和属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="5ab73-108">它可以帮助你理解创建或更新页面内容时的输入 HTML 以及分析返回的页面内容时的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="5ab73-109">Body 元素</span><span class="sxs-lookup"><span data-stu-id="5ab73-109">Body element</span></span>
<span data-ttu-id="5ab73-110">页面正文中的 HTML 内容表示页面内容和结构，其中包括图像和文件资源。</span><span class="sxs-lookup"><span data-stu-id="5ab73-110">The HTML content in the page body represents  the page content and structure, including image and file resources. The body element can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="5ab73-111">**body** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-111">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="5ab73-112">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-112">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-113">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-113">Input attribute</span></span>|<span data-ttu-id="5ab73-114">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="5ab73-115">data-absolute-enabled</span></span> | <span data-ttu-id="5ab73-116">指示输入正文是否支持[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)元素。</span><span class="sxs-lookup"><span data-stu-id="5ab73-116">Indicates whether the input body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> |
| <span data-ttu-id="5ab73-117">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-117">style</span></span> | <p><span data-ttu-id="5ab73-118">正文的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="5ab73-119">在输出 HTML 中，可能在相应的子元素上内嵌返回输入设置。</span><span class="sxs-lookup"><span data-stu-id="5ab73-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="5ab73-120">**body** 元素当前不支持背景色。</span><span class="sxs-lookup"><span data-stu-id="5ab73-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

<span data-ttu-id="5ab73-121">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-121">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-122">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-122">Output attribute</span></span>|<span data-ttu-id="5ab73-123">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="5ab73-124">data-absolute-enabled</span></span> | <span data-ttu-id="5ab73-125">指示正文是否支持[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)元素。</span><span class="sxs-lookup"><span data-stu-id="5ab73-125">Indicates whether the body supports absolutely positioned elements. Always true in output HTML.</span></span> <span data-ttu-id="5ab73-126">在输出 HTML 中始终为 **true**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="5ab73-127">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-127">style</span></span> | <span data-ttu-id="5ab73-128">正文的 **font-family** 和 **font-size** 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="5ab73-129">Div 元素</span><span class="sxs-lookup"><span data-stu-id="5ab73-129">Div elements</span></span>
<span data-ttu-id="5ab73-130">**Div** 元素包含文本、图像和其他内容。</span><span class="sxs-lookup"><span data-stu-id="5ab73-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="5ab73-131">**div** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-131">Divs contain text, images, and other content. A **div** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="5ab73-132">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-132">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-133">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-133">Input attribute</span></span>|<span data-ttu-id="5ab73-134">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-135">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-135">data-id</span></span> | <span data-ttu-id="5ab73-136">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-136">A reference for the element.</span></span> <span data-ttu-id="5ab73-137">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-137">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="5ab73-138">data-render-fallback</span></span> | <span data-ttu-id="5ab73-139">[提取](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)失败时的回退操作：**render**（默认）或 **none**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-139">The fallback action if the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="5ab73-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="5ab73-140">data-render-method</span></span> | <span data-ttu-id="5ab73-141">要执行的[提取](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)方法，例如：`extract.businesscard` 或 `extract.recipe`。</span><span class="sxs-lookup"><span data-stu-id="5ab73-141">The [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) method to perform, for example: `extract.businesscard`extract.businesscard`extract.recipe`

or extract.recipe.</span></span> |
| <span data-ttu-id="5ab73-142">data-render-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-142">data-render-src</span></span> | <span data-ttu-id="5ab73-143">[提取](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)的内容源。</span><span class="sxs-lookup"><span data-stu-id="5ab73-143">The content source for the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span> |
| <span data-ttu-id="5ab73-144">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-144">style</span></span> | <p><span data-ttu-id="5ab73-145">div 的位置、大小、字体和颜色属性：</span><span class="sxs-lookup"><span data-stu-id="5ab73-145">The position, size, font, and color properties for the div:</span></span></p><p> <span data-ttu-id="5ab73-146">- **位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-146">- **position** (**absolute** only), **left**, **top**, and **width**.</span></span> <span data-ttu-id="5ab73-147">（div 的高度是自动配置的。）</span><span class="sxs-lookup"><span data-stu-id="5ab73-147">(Height is auto-configured for divs.)</span></span><br /><span data-ttu-id="5ab73-148">用于创建[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div（仅在正文设置 `data-absolute-enabled="true"` 且 div 是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="5ab73-148">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="5ab73-149">示例：`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5ab73-149">Example`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></p><p> <span data-ttu-id="5ab73-150">- 此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-150">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="5ab73-151">在输出 HTML 中，可能在相应的子元素上内嵌返回这些值。</span><span class="sxs-lookup"><span data-stu-id="5ab73-151">The CSS style properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></p> |
 

<span data-ttu-id="5ab73-152">Microsoft Graph 中的 OneNote API 至少在一个 div 中包装所有正文内容。</span><span class="sxs-lookup"><span data-stu-id="5ab73-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="5ab73-153">在以下情况下，API 创建一个默认 div（使用 `data-id="_default"` 设定属性）以包含正文内容：</span><span class="sxs-lookup"><span data-stu-id="5ab73-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="5ab73-154">输入 body 元素的 **data-absolute-enabled** 属性被省略或被设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-154">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span> <span data-ttu-id="5ab73-155">在此情况下，所有正文内容都被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="5ab73-155">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="5ab73-156">输入 body 元素的 **data-absolute-enabled** 属性为 **true**，但输入 HTML 包含的直接子级不是[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp; **div**、**img** 或 **object** 元素。</span><span class="sxs-lookup"><span data-stu-id="5ab73-156">The input body element's data-absolute-enabled attribute is true, but the input HTML  contains direct children that aren't absolutely positioned div, img, or object elements. In this case, direct children that aren't absolutely positioned div, img, or object elements are put in the default div.</span></span> <span data-ttu-id="5ab73-157">在此情况下，不是[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp; **div**、**img** 或 **object** 元素的直接子级被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="5ab73-157">In this case, direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


<span data-ttu-id="5ab73-158">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-158">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-159">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-159">Output attribute</span></span>|<span data-ttu-id="5ab73-160">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-161">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-161">data-id</span></span> | <span data-ttu-id="5ab73-162">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-162">A reference for the element.</span></span> <span data-ttu-id="5ab73-163">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-163">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-164">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-164">id</span></span> | <span data-ttu-id="5ab73-165">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-165">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-166">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-166">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-167">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-167">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-168">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-168">style</span></span> | <span data-ttu-id="5ab73-169">div 的位置和大小属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="5ab73-170">非贡献 div</span><span class="sxs-lookup"><span data-stu-id="5ab73-170">Non-contributing divs</span></span>
<span data-ttu-id="5ab73-171">当输入 HTML 中的 **div** 元素不对页面结构做出贡献或带有 OneNote 所使用的信息时，此 API 将 div 的内容移动到父 div 或默认 div。</span><span class="sxs-lookup"><span data-stu-id="5ab73-171">When a div element in the input HTML does not contribute to the page structure or carry information that onnvshort uses,  the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="5ab73-172">下面的示例对此进行了说明。</span><span class="sxs-lookup"><span data-stu-id="5ab73-172">This is illustrated in the following examples.</span></span>

<span data-ttu-id="5ab73-173">包含非贡献嵌套 div 的**输入 HTML**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-173">**Input HTML**  that contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

<span data-ttu-id="5ab73-174">**输出 HTML**</span><span class="sxs-lookup"><span data-stu-id="5ab73-174">**Output HTML**</span></span>

><span data-ttu-id="5ab73-175">**注意：**div 的内容已被移至父 div 且嵌套 `<div>` 标记已被删除。</span><span class="sxs-lookup"><span data-stu-id="5ab73-175">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="5ab73-176">如果 div 定义了任何语义信息，例如 **data-id**（示例：`<div data-id="keep-me">`），则保留该 div。</span><span class="sxs-lookup"><span data-stu-id="5ab73-176">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="5ab73-177">Img 元素</span><span class="sxs-lookup"><span data-stu-id="5ab73-177">Img elements</span></span>
<span data-ttu-id="5ab73-178">OneNote 页上的图像由 **img** 元素表示。</span><span class="sxs-lookup"><span data-stu-id="5ab73-178">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="5ab73-179">**img** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-179">Images on onnvshort pages are represented by **img** elements. An img element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="5ab73-180">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-180">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-181">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-181">Input attribute</span></span>|<span data-ttu-id="5ab73-182">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-182">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-183">alt</span><span class="sxs-lookup"><span data-stu-id="5ab73-183">alt</span></span> | <span data-ttu-id="5ab73-184">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="5ab73-184">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="5ab73-185">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-185">data-id</span></span> | <span data-ttu-id="5ab73-186">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-186">A reference for the element.</span></span> <span data-ttu-id="5ab73-187">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-187">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-188">data-render-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-188">data-render-src</span></span> |<span data-ttu-id="5ab73-189">需要 **data-render-src** 或 **src**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-189">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="5ab73-190">在 OneNote 页上显示为位图图像的网页：</span><span class="sxs-lookup"><span data-stu-id="5ab73-190">The webpage to render as a bit-mapped image on the onnvshort page:</span></span><br /> <span data-ttu-id="5ab73-191">- `data-render-src="http://..."` 表示公共 URL。</span><span class="sxs-lookup"><span data-stu-id="5ab73-191">- `data-render-src="http://..."` for a public URL.</span></span><br /> <span data-ttu-id="5ab73-192">- `data-render-src="name:BlockName"` 表示[多部分请求](../api-reference/v1.0/api/section_post_pages.md#example)的“演示文稿”块中的图像部分。</span><span class="sxs-lookup"><span data-stu-id="5ab73-192">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="5ab73-193">如果网页比 OneNote 页能够忠实呈现的内容更为复杂，或者页面需要登录凭据，则此方法很有用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-193">data-render-src="name:BlockName" for an image part in the Presentation block of a multi-part request. This method is useful when the webpage is more complex than the onnvshort page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="5ab73-194">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-194">data-tag</span></span> | <span data-ttu-id="5ab73-195">元素上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-195">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="5ab73-196">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-196">style</span></span> |<span data-ttu-id="5ab73-197">图像的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**、**宽度**和**高度**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-197">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="5ab73-198">可在任何图像上设置大小。</span><span class="sxs-lookup"><span data-stu-id="5ab73-198">Size can be set on any image.</span></span> <span data-ttu-id="5ab73-199">位置属性用于创建[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)图像（仅在正文设置 `data-absolute-enabled="true"` 且图像是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="5ab73-199">Position properties are used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="5ab73-200">示例：`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5ab73-200">Example`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="5ab73-201">在输出 HTML 中，图像大小分别以 **width** 和 **height** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-201">In the output HTML, the image size is returned separately in  **width** and **height** attributes.</span></span> |
| <span data-ttu-id="5ab73-202">src</span><span class="sxs-lookup"><span data-stu-id="5ab73-202">src</span></span> |<span data-ttu-id="5ab73-203">需要 **src** 或 **data-render-src**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-203">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="5ab73-204">要在 OneNote 页上呈现的图像：</span><span class="sxs-lookup"><span data-stu-id="5ab73-204">The image to render on the onnvshort page:</span></span><br /> <span data-ttu-id="5ab73-205">- `src="http://..."` 表示 Internet 上公开可用图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="5ab73-205">src="http://..." for a URL to a publicly available image on the internet.</span></span><br /> <span data-ttu-id="5ab73-206">- `src="name:BlockName"` 表示代表此图像的多部分请求中的已命名部分。</span><span class="sxs-lookup"><span data-stu-id="5ab73-206">src="name:BlockName" for a named part in a multi-part request that represents the image.</span></span>|
| <span data-ttu-id="5ab73-207">width，height</span><span class="sxs-lookup"><span data-stu-id="5ab73-207">width, height</span></span> | <span data-ttu-id="5ab73-208">图像的宽度或高度，以不带 px 的像素为单位。</span><span class="sxs-lookup"><span data-stu-id="5ab73-208">The width or height of the image, in pixels but without the px. Example: width="400"</span></span> <span data-ttu-id="5ab73-209">示例：`width="400"`</span><span class="sxs-lookup"><span data-stu-id="5ab73-209">Example`width="400"`</span></span> |
 
><span data-ttu-id="5ab73-210">**注意：**OneNote API 自动检测输入图像类型，并在输出 HTML 中将其返回为 **data-fullres-src-type**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-210">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="5ab73-211">此外，API 还会在 **data-src-type** 中返回优化的图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="5ab73-211">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

<span data-ttu-id="5ab73-212">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-212">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-213">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-213">Output attribute</span></span>|<span data-ttu-id="5ab73-214">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-214">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-215">alt</span><span class="sxs-lookup"><span data-stu-id="5ab73-215">alt</span></span> | <span data-ttu-id="5ab73-216">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="5ab73-216">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="5ab73-217">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-217">data-id</span></span> | <span data-ttu-id="5ab73-218">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-218">A reference for the element.</span></span> <span data-ttu-id="5ab73-219">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-219">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-220">data-index</span><span class="sxs-lookup"><span data-stu-id="5ab73-220">data-index</span></span> | <span data-ttu-id="5ab73-221">图像的位置。</span><span class="sxs-lookup"><span data-stu-id="5ab73-221">The position properties of the image.</span></span> <span data-ttu-id="5ab73-222">支持[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-222">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="5ab73-223">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-223">data-fullres-src</span></span> | <span data-ttu-id="5ab73-224">最初嵌入在页面中的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="5ab73-224">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="5ab73-225">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="5ab73-225">data-fullres-src-type</span></span> | <span data-ttu-id="5ab73-226">**data-fullres-src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="5ab73-226">The MIME type of the **data-fullres-src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="5ab73-227">data-options</span><span class="sxs-lookup"><span data-stu-id="5ab73-227">data-options</span></span> | <span data-ttu-id="5ab73-228">源类型：PDF 文件的 **printout** 或所有其他文件的 **splitimage**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-228">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to split images created with the data-render-src attribute.</span></span> <span data-ttu-id="5ab73-229">仅适用于使用 **data-render-src** 属性创建的[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-229">The source type: **printout** for PDF files or splitimage for all others. Applies only to [split images](#split-images) created with the data-render-src attribute.</span></span> |
| <span data-ttu-id="5ab73-230">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-230">data-render-original-src</span></span> | <span data-ttu-id="5ab73-231">此图像的原始源 URL，前提是该源图像来自公共 Internet，且使用 **data-render-src** 属性创建。</span><span class="sxs-lookup"><span data-stu-id="5ab73-231">The original source URL of the image, if the source image  is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="5ab73-232">data-src-type</span><span class="sxs-lookup"><span data-stu-id="5ab73-232">data-src-type</span></span> | <span data-ttu-id="5ab73-233">**src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="5ab73-233">The MIME type of the **src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="5ab73-234">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-234">data-tag</span></span> | <span data-ttu-id="5ab73-235">元素上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-235">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="5ab73-236">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-236">id</span></span> | <span data-ttu-id="5ab73-237">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-237">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-238">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-238">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-239">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-239">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-240">src</span><span class="sxs-lookup"><span data-stu-id="5ab73-240">src</span></span> | <span data-ttu-id="5ab73-241">已针对 Web 浏览器以及移动设备和平板电脑外形规格进行优化的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="5ab73-241">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="5ab73-242">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-242">style</span></span> | <span data-ttu-id="5ab73-243">此图像的位置属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-243">The position properties of the image.</span></span> |
| <span data-ttu-id="5ab73-244">width、height</span><span class="sxs-lookup"><span data-stu-id="5ab73-244">width, height</span></span> | <span data-ttu-id="5ab73-245">此图像的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="5ab73-245">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="5ab73-246">图像的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="5ab73-246">Output HTML examples for images</span></span>
<span data-ttu-id="5ab73-247">输出 **img** 元素包含图像文件资源的终结点和图像类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="5ab73-247">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="5ab73-248">可以发出单独的[图像资源终结点的 GET 请求](../api-reference/v1.0/api/resource_get.md)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="5ab73-248">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```http
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="5ab73-249">默认情况下，图像并不会直接在浏览器中显示，因为它们具有私密性，需要授权才能对其检索，这与页面其他内容一样。</span><span class="sxs-lookup"><span data-stu-id="5ab73-249">Images won’t render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="5ab73-250">若要获取页面上的图像资源的公共 URL，请在检索页面内容时，在查询字符串中添加 **preAuthenticated=true**（例如：`GET ../pages/{page-id}/content?preAuthenticated=true`）。</span><span class="sxs-lookup"><span data-stu-id="5ab73-250">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="5ab73-251">返回的公共 URL 的有效期为一小时。</span><span class="sxs-lookup"><span data-stu-id="5ab73-251">The public URLs that are returned are valid for one hour.</span></span> 

<span data-ttu-id="5ab73-252">**在请求中添加 _preAuthenticated=true_ 时带有公共 URL 的图像**</span><span class="sxs-lookup"><span data-stu-id="5ab73-252">**Image with public URL when _preAuthenticated=true_ is included in the request**</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}" />
```

<span data-ttu-id="5ab73-253">以下示例说明 **img** 元素在输出 HTML 中可能包含的信息。</span><span class="sxs-lookup"><span data-stu-id="5ab73-253">The following examples show the information an **img** element might contain in the output HTML.</span></span>

<span data-ttu-id="5ab73-254">**带有 Web 安全和高分辨率资源的图像**</span><span class="sxs-lookup"><span data-stu-id="5ab73-254">**Image with web-ready and high resolution resources**</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

<span data-ttu-id="5ab73-255">**通过使用 *data-render-src* 属性创建的图像**</span><span class="sxs-lookup"><span data-stu-id="5ab73-255">**Image created by using the *data-render-src* attribute**</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="5ab73-256">拆分图像</span><span class="sxs-lookup"><span data-stu-id="5ab73-256">Split images</span></span>

<span data-ttu-id="5ab73-257">出于性能和呈现的考虑，使用 **data-render-src** 属性（从网页 URL 或已命名的部分）创建的图像可能被拆分为多个组件图像。</span><span class="sxs-lookup"><span data-stu-id="5ab73-257">Images that are created using the **data-render-src** attribute from a webpage URL or a named part might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same data-id value.  Each component image has a zero-based data-index attribute that defines the  original vertical layout.</span></span> <span data-ttu-id="5ab73-258">向所有组件映像分配同一 **data-id** 值。</span><span class="sxs-lookup"><span data-stu-id="5ab73-258">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="5ab73-259">每个组件图像均具有从零开始的数据索引属性，该属性定义原始垂直布局。</span><span class="sxs-lookup"><span data-stu-id="5ab73-259">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

<span data-ttu-id="5ab73-260">**带有三个组件图像的拆分图像**</span><span class="sxs-lookup"><span data-stu-id="5ab73-260">**Split image with three component images**</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="5ab73-261">用户可以在页面上移动图像，因此返回的索引可能是无序的。</span><span class="sxs-lookup"><span data-stu-id="5ab73-261">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span> <span data-ttu-id="5ab73-262">排序方法是从上到下的 Y 轴排序，如果 y 轴顺序存在冲突，则从左到右按 x 轴进行排序。</span><span class="sxs-lookup"><span data-stu-id="5ab73-262">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="5ab73-263">iframe 元素</span><span class="sxs-lookup"><span data-stu-id="5ab73-263">iframe elements</span></span>
<span data-ttu-id="5ab73-264">OneNote 页可包含由 **iframe** 元素所表示的嵌入的视频。</span><span class="sxs-lookup"><span data-stu-id="5ab73-264">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

><span data-ttu-id="5ab73-265">**注意：**也可以[使用 **object** 元素附加视频文件](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-265">**Note:** You can also [attach a video file using an **object** element](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span></span>

<span data-ttu-id="5ab73-266">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-266">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-267">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-267">Input attribute</span></span>|<span data-ttu-id="5ab73-268">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-268">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-269">data-original-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-269">data-original-src</span></span> | <span data-ttu-id="5ab73-270">必需。</span><span class="sxs-lookup"><span data-stu-id="5ab73-270">Required.</span></span> <span data-ttu-id="5ab73-271">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="5ab73-271">The URL of the video source.</span></span> <span data-ttu-id="5ab73-272">请参阅[受支持的视频源的列表](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-272">See the [list of supported video sources](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span></span> <span data-ttu-id="5ab73-273">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="5ab73-273">Example`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="5ab73-274">width，height</span><span class="sxs-lookup"><span data-stu-id="5ab73-274">width, height</span></span> | <span data-ttu-id="5ab73-275">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="5ab73-275">The width or height of the image, in pixels.</span></span> <span data-ttu-id="5ab73-276">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="5ab73-276">Example`width=300`</span></span> |

<span data-ttu-id="5ab73-277">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-277">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-278">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-278">Output attribute</span></span>|<span data-ttu-id="5ab73-279">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-279">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-280">data-original-src</span><span class="sxs-lookup"><span data-stu-id="5ab73-280">data-original-src</span></span> | <span data-ttu-id="5ab73-281">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="5ab73-281">The URL of the video source.</span></span> |
| <span data-ttu-id="5ab73-282">src</span><span class="sxs-lookup"><span data-stu-id="5ab73-282">src</span></span> | <span data-ttu-id="5ab73-283">在 OneNote 页中嵌入的视频的链接。</span><span class="sxs-lookup"><span data-stu-id="5ab73-283">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="5ab73-284">width，height</span><span class="sxs-lookup"><span data-stu-id="5ab73-284">width, height</span></span> | <span data-ttu-id="5ab73-285">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="5ab73-285">The width or height of the image, in pixels.</span></span> <span data-ttu-id="5ab73-286">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="5ab73-286">Example`width=300`</span></span> |
 
<span data-ttu-id="5ab73-287">视频的**输出 HTML** 示例</span><span class="sxs-lookup"><span data-stu-id="5ab73-287">Output HTML example for objects</span></span>

<span data-ttu-id="5ab73-288">输出 **iframe** 元素包含链接到源页面和视频的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="5ab73-288">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="5ab73-289">Object 元素</span><span class="sxs-lookup"><span data-stu-id="5ab73-289">Object elements</span></span>
<span data-ttu-id="5ab73-290">OneNote 页可包含由 **object** 元素表示的文件附件。</span><span class="sxs-lookup"><span data-stu-id="5ab73-290">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="5ab73-291">**object** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-291">onnvshort pages can contain file attachments  represented by **object** elements. An object element can contain the following attributes in the input and output HTML.</span></span>

><span data-ttu-id="5ab73-292">**注意：**将文件发送为图像并使用 **data-render-src** 属性时，OneNote API 还可以将此文件的内容呈现为页面中的图像。</span><span class="sxs-lookup"><span data-stu-id="5ab73-292">The onnvshort API can also render file content as images in a page when the file is sent as an image and uses the data-render-src attribute.  Example: <img data-render-src="name:BlockName" ... /></span></span> <span data-ttu-id="5ab73-293">示例：`<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="5ab73-293">Example`<img data-render-src="name:part-name" ... />`</span></span>
 

<span data-ttu-id="5ab73-294">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-294">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-295">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-295">Input attribute</span></span>|<span data-ttu-id="5ab73-296">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-296">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-297">data</span><span class="sxs-lookup"><span data-stu-id="5ab73-297">data</span></span> | <span data-ttu-id="5ab73-298">必需。</span><span class="sxs-lookup"><span data-stu-id="5ab73-298">Required.</span></span> <span data-ttu-id="5ab73-299">表示[多部分请求](../api-reference/v1.0/api/section_post_pages.md#example)中文件的部分的名称。</span><span class="sxs-lookup"><span data-stu-id="5ab73-299">Required. The name of the part that represents the file in the multi-part request.</span></span> |
| <span data-ttu-id="5ab73-300">data-attachment</span><span class="sxs-lookup"><span data-stu-id="5ab73-300">data-attachment</span></span> | <span data-ttu-id="5ab73-p137">必需。文件名。</span><span class="sxs-lookup"><span data-stu-id="5ab73-p137">Required. The file name.</span></span> |
| <span data-ttu-id="5ab73-303">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-303">data-id</span></span> | <span data-ttu-id="5ab73-304">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-304">A reference for the element.</span></span> <span data-ttu-id="5ab73-305">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-305">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-306">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-306">style</span></span> | <p><span data-ttu-id="5ab73-307">对象的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-307">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span></p><p><span data-ttu-id="5ab73-308">用于创建[绝对定位](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)对象（仅在正文设置 `data-absolute-enabled="true"` 且对象是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="5ab73-308">position (absolute only), left, top, and width properties. Used to create an absolutely positioned object, only if the object is a direct child of the body when the  body sets data-absolute-enabled="true". Learn more about absolutely positioned elements. Example: <object style="position:absolute;top:350px;left:300px" ... /></span></span><br /><span data-ttu-id="5ab73-309">示例：`<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="5ab73-309">Example`<object style="position:absolute;top:350px;left:300px" ... />`</span></span></p> |
| <span data-ttu-id="5ab73-310">type</span><span class="sxs-lookup"><span data-stu-id="5ab73-310">type</span></span> | <span data-ttu-id="5ab73-311">必需。</span><span class="sxs-lookup"><span data-stu-id="5ab73-311">Required.</span></span> <span data-ttu-id="5ab73-312">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="5ab73-312">The standard MIME file type.</span></span> <span data-ttu-id="5ab73-313">已知文件类型显示与 OneNote 页上的文件类型相关联的图标。</span><span class="sxs-lookup"><span data-stu-id="5ab73-313">Required. The standard MIME file type.  Known file types display the icon associated with the file type on the onnvshort page. Unknown file types display a generic file icon.</span></span> <span data-ttu-id="5ab73-314">已知文件类型显示通用文件图标。</span><span class="sxs-lookup"><span data-stu-id="5ab73-314">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

<span data-ttu-id="5ab73-315">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-315">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-316">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-316">Output attribute</span></span>|<span data-ttu-id="5ab73-317">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-317">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-318">data</span><span class="sxs-lookup"><span data-stu-id="5ab73-318">data</span></span> | <span data-ttu-id="5ab73-319">文件资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="5ab73-319">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="5ab73-320">data-attachment</span><span class="sxs-lookup"><span data-stu-id="5ab73-320">data-attachment</span></span> | <span data-ttu-id="5ab73-321">文件名。</span><span class="sxs-lookup"><span data-stu-id="5ab73-321">The file name.</span></span> |
| <span data-ttu-id="5ab73-322">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-322">data-id</span></span> | <span data-ttu-id="5ab73-323">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-323">A reference for the element.</span></span> <span data-ttu-id="5ab73-324">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-324">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-325">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-325">id</span></span> | <span data-ttu-id="5ab73-326">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-326">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-327">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-327">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-328">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-328">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-329">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-329">style</span></span> | <span data-ttu-id="5ab73-330">此对象的位置属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-330">The position properties of the object.</span></span> |
| <span data-ttu-id="5ab73-331">type</span><span class="sxs-lookup"><span data-stu-id="5ab73-331">type</span></span> | <span data-ttu-id="5ab73-332">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="5ab73-332">The standard MIME file type.</span></span> |
 

<span data-ttu-id="5ab73-333">对象的**输出 HTML** 示例</span><span class="sxs-lookup"><span data-stu-id="5ab73-333">Output HTML example for objects</span></span>

<span data-ttu-id="5ab73-334">输出 **object** 元素包含链接到页面中的文件资源的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="5ab73-334">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="5ab73-335">可以发出单独的[文件资源终结点的 GET 请求](../api-reference/v1.0/api/resource_get.md)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="5ab73-335">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="5ab73-336">段落和标题</span><span class="sxs-lookup"><span data-stu-id="5ab73-336">Paragraphs and headings</span></span>

<span data-ttu-id="5ab73-337">段落、标题和其他文本容器可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-337">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="5ab73-338">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-338">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-339">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-339">Input attribute</span></span>|<span data-ttu-id="5ab73-340">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-340">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-341">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-341">data-id</span></span> | <span data-ttu-id="5ab73-342">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-342">A reference for the element.</span></span> <span data-ttu-id="5ab73-343">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-343">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-344">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-344">data-tag</span></span> | <span data-ttu-id="5ab73-345">**p** 或 **h1** - **h6** 元素上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-345">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="5ab73-346">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-346">style</span></span> | <span data-ttu-id="5ab73-347">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-347">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="5ab73-348">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-348">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-349">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-349">Output attribute</span></span>|<span data-ttu-id="5ab73-350">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-350">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-351">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-351">data-id</span></span> | <span data-ttu-id="5ab73-352">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-352">A reference for the element.</span></span> <span data-ttu-id="5ab73-353">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-353">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-354">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-354">data-tag</span></span> | <span data-ttu-id="5ab73-355">**p** 或 **h1** - **h6** 元素上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-355">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="5ab73-356">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-356">id</span></span> | <span data-ttu-id="5ab73-357">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-357">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-358">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-358">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-359">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-359">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-360">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-360">style</span></span> | <span data-ttu-id="5ab73-361">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-361">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="5ab73-362">在输出 HTML 中，可能在相应的子元素或 **span** 元素上内嵌返回这些值。</span><span class="sxs-lookup"><span data-stu-id="5ab73-362">The CSS style properties of the element. In the output HTML, these values may be returned on inline on appropriate child elements or span elements.</span></span> |
 

<span data-ttu-id="5ab73-363">以下示例显示使用不同方法定义文本容器样式的输入 HTML 和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-363">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

<span data-ttu-id="5ab73-364">在 **span** 元素的起始标记中使用内联字符样式定义样式的**输入 HTML**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-364">**Input HTML** with styles defined using inline character styles, in the start tag,  and within a **span** element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

<span data-ttu-id="5ab73-365">带有 `<i>` 字符样式以及 `<p>` 起始标记中的字体设置的**输出 HTML** 作为 **span** 元素上的内联 CSS 样式返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-365">**Output HTML** with the **<i>`<i>` character style and the font settings in the <p>`<p>` start tag returned as inline CSS styles on span** elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="5ab73-366">列表</span><span class="sxs-lookup"><span data-stu-id="5ab73-366">Lists</span></span>
<span data-ttu-id="5ab73-367">列表表示为包含由 **li** 元素所表示的列表项的 **ol** 或 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="5ab73-367">
 


Lists are represented as ol or ul elements that can contain li elements.</span></span>

<span data-ttu-id="5ab73-368">列表和列表项可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-368">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="5ab73-369">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-369">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-370">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-370">Input attribute</span></span>|<span data-ttu-id="5ab73-371">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-371">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-372">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-372">data-id</span></span> | <span data-ttu-id="5ab73-373">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-373">A reference for the element.</span></span> <span data-ttu-id="5ab73-374">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-374">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-375">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-375">data-tag</span></span> | <span data-ttu-id="5ab73-376">**ul**、**ol** 或 **li** 元素上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-376">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="5ab73-377">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-377">style</span></span> | <span data-ttu-id="5ab73-378">列表或列表项的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-378">The **list-style-type** and the  CSS [style](#styles) properties for the list or list item.</span></span> |
 

<span data-ttu-id="5ab73-379">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-379">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-380">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-380">Output attribute</span></span>|<span data-ttu-id="5ab73-381">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-381">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-382">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-382">data-id</span></span> | <span data-ttu-id="5ab73-383">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-383">A reference for the element.</span></span> <span data-ttu-id="5ab73-384">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-384">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-385">data-tag</span><span class="sxs-lookup"><span data-stu-id="5ab73-385">data-tag</span></span> |  <span data-ttu-id="5ab73-386">**li** 元素中的 span 上的[笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-386">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **span** in a li element.</span></span> |
| <span data-ttu-id="5ab73-387">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-387">id</span></span> | <span data-ttu-id="5ab73-388">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-388">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-389">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-389">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-390">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-390">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-391">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-391">style</span></span> | <span data-ttu-id="5ab73-392">元素的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-392">The CSS [style](#styles) properties of the element, and also:</span></span> <span data-ttu-id="5ab73-393">在输出 HTML 中，在列表项上返回列表级别设置。</span><span class="sxs-lookup"><span data-stu-id="5ab73-393">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="5ab73-394">不会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-394">The following properties are not returned:</span></span> |
 

<span data-ttu-id="5ab73-395">Microsoft Graph 中的 OneNote API 支持以下列表样式：</span><span class="sxs-lookup"><span data-stu-id="5ab73-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="5ab73-396">已排序列表</span><span class="sxs-lookup"><span data-stu-id="5ab73-396">Ordered list</span></span>|<span data-ttu-id="5ab73-397">未排序列表</span><span class="sxs-lookup"><span data-stu-id="5ab73-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-398">无</span><span class="sxs-lookup"><span data-stu-id="5ab73-398">none</span></span> | <span data-ttu-id="5ab73-399">无</span><span class="sxs-lookup"><span data-stu-id="5ab73-399">none</span></span> |
| <span data-ttu-id="5ab73-400">
decimal (default)</span><span class="sxs-lookup"><span data-stu-id="5ab73-400">decimal (default)</span></span> | <span data-ttu-id="5ab73-401">
disc (default)</span><span class="sxs-lookup"><span data-stu-id="5ab73-401">disc (default)</span></span> |
| <span data-ttu-id="5ab73-402">
lower-alpha</span><span class="sxs-lookup"><span data-stu-id="5ab73-402">lower-alpha</span></span> | <span data-ttu-id="5ab73-403">
circle</span><span class="sxs-lookup"><span data-stu-id="5ab73-403">circle</span></span> |
| <span data-ttu-id="5ab73-404">
lower-roman</span><span class="sxs-lookup"><span data-stu-id="5ab73-404">lower-roman</span></span> | <span data-ttu-id="5ab73-405">

square</span><span class="sxs-lookup"><span data-stu-id="5ab73-405">square</span></span> |
| <span data-ttu-id="5ab73-406">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="5ab73-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="5ab73-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="5ab73-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="5ab73-408">您可以在输入 HTML 中对 **ol** 或 **ul** 元素上的列表应用全局样式，但样式在 **li** 元素上返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

<span data-ttu-id="5ab73-409">**同源列表样式**</span><span class="sxs-lookup"><span data-stu-id="5ab73-409">**Homogenous list style**</span></span>

<span data-ttu-id="5ab73-410">本示例显示了在 **ol** 元素上设置列表样式类型以及在单独列表项上设置 CSS 样式的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="5ab73-411">这是输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-411">This is the output HTML.</span></span> <span data-ttu-id="5ab73-412">请注意，这些样式在单独的 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-412">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

<span data-ttu-id="5ab73-413">**变量列表样式**</span><span class="sxs-lookup"><span data-stu-id="5ab73-413">**Variable list styles**</span></span>

<span data-ttu-id="5ab73-414">本示例显示了在 **li** 元素上设置不同列表样式类型的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="5ab73-415">这是输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-415">This is the output HTML.</span></span> <span data-ttu-id="5ab73-416">请注意，这些样式在单独的 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-416">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="5ab73-417">Table</span><span class="sxs-lookup"><span data-stu-id="5ab73-417">Tables</span></span>
<span data-ttu-id="5ab73-418">这些表表示为可以包含 **tr** 和 **td** 元素的 **table** 元素。</span><span class="sxs-lookup"><span data-stu-id="5ab73-418">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span> <span data-ttu-id="5ab73-419">支持嵌套表。</span><span class="sxs-lookup"><span data-stu-id="5ab73-419">Nested tables are supported.</span></span>

<span data-ttu-id="5ab73-420">表可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-420">Lists and list items can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="5ab73-421">OneNote API 不支持 **rowspan** 或 **colspan** 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

<span data-ttu-id="5ab73-422">**输入属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-422">**Input attributes**</span></span>

|<span data-ttu-id="5ab73-423">输入属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-423">Input attribute</span></span>|<span data-ttu-id="5ab73-424">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-425">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-425">data-id</span></span> | <span data-ttu-id="5ab73-426">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-426">A reference for the element.</span></span> <span data-ttu-id="5ab73-427">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-427">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-428">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-428">style</span></span> | <span data-ttu-id="5ab73-429">此元素的 CSS [style](#styles) 属性，以及：</span><span class="sxs-lookup"><span data-stu-id="5ab73-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="5ab73-430">- **Border**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-430">Border</span></span> <span data-ttu-id="5ab73-431">可以是 0px，也可以是 1px。</span><span class="sxs-lookup"><span data-stu-id="5ab73-431">border. Can be either 0px or 1px.</span></span><br /> <span data-ttu-id="5ab73-432">- **width**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-432">width</span></span> <span data-ttu-id="5ab73-433">受 **table** 和 **td** 支持作为页面宽度的像素或百分比。</span><span class="sxs-lookup"><span data-stu-id="5ab73-433">**width**. Supported by **table** and td as pixels or percentage of page width. Example: width="100px" or width="60%"</span></span><br /><span data-ttu-id="5ab73-434">示例：`width="100px"` 或 `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="5ab73-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

<span data-ttu-id="5ab73-435">**输出属性**</span><span class="sxs-lookup"><span data-stu-id="5ab73-435">**Output attributes**</span></span>

|<span data-ttu-id="5ab73-436">输出属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-436">Output attribute</span></span>|<span data-ttu-id="5ab73-437">说明</span><span class="sxs-lookup"><span data-stu-id="5ab73-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-438">data-id</span><span class="sxs-lookup"><span data-stu-id="5ab73-438">data-id</span></span> | <span data-ttu-id="5ab73-439">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="5ab73-439">A reference for the element.</span></span> <span data-ttu-id="5ab73-440">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-440">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-441">id</span><span class="sxs-lookup"><span data-stu-id="5ab73-441">id</span></span> | <span data-ttu-id="5ab73-442">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ab73-442">A unique ID for the group.</span></span> <span data-ttu-id="5ab73-443">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](../api-reference/v1.0/api/page_get.md)返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-443">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="5ab73-444">用于[更新页面内容](../api-reference/v1.0/api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="5ab73-444">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="5ab73-445">style</span><span class="sxs-lookup"><span data-stu-id="5ab73-445">style</span></span> | <span data-ttu-id="5ab73-446">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="5ab73-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="5ab73-447">以下示例显示使用不同方法定义表样式的输入 HTML和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

<span data-ttu-id="5ab73-448">具有不同级别可选设置的**输入 HTML**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-448">**Input HTML** with optional settings at different levels.</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
<span data-ttu-id="5ab73-449">具有 CSS 样式的**输出 HTML** 在 **td** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="5ab73-449">**Output HTML** with CSS styles returned inline on the **td** elements.</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="5ab73-450">样式</span><span class="sxs-lookup"><span data-stu-id="5ab73-450">Styles</span></span>
<span data-ttu-id="5ab73-451">Microsoft Graph 中的 OneNote API 支持页面正文中元素的以下内联 CSS **style** 属性，如 **body**、**div**、**p**、**li** 和 **span**。</span><span class="sxs-lookup"><span data-stu-id="5ab73-451">The onnvshort API supports the following inline CSS style properties for elements in the page body, such as body, div, p, li, and span.</span></span>

|<span data-ttu-id="5ab73-452">属性</span><span class="sxs-lookup"><span data-stu-id="5ab73-452">Property</span></span>|<span data-ttu-id="5ab73-453">示例</span><span class="sxs-lookup"><span data-stu-id="5ab73-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="5ab73-454">background-color</span><span class="sxs-lookup"><span data-stu-id="5ab73-454">background-color</span></span> | <span data-ttu-id="5ab73-455">`style="background-color:#66cc66"`（默认为白色）</span><span class="sxs-lookup"><span data-stu-id="5ab73-455">style="background-color:#66cc66"`style="background-color:#66cc66"` (defaults to  white)</span></span><br /><span data-ttu-id="5ab73-456">支持十六进制格式和命名颜色。</span><span class="sxs-lookup"><span data-stu-id="5ab73-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="5ab73-457">color</span><span class="sxs-lookup"><span data-stu-id="5ab73-457">color</span></span> | <span data-ttu-id="5ab73-458">`style="color:#ffffff"`（默认为黑色）</span><span class="sxs-lookup"><span data-stu-id="5ab73-458">style="color:#ffffff"`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="5ab73-459">font-family</span><span class="sxs-lookup"><span data-stu-id="5ab73-459">font-family</span></span> | <span data-ttu-id="5ab73-460">`style="font-family:Courier"`（默认为 Calibri）</span><span class="sxs-lookup"><span data-stu-id="5ab73-460">style="font-family:Courier"`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="5ab73-461">font-size</span><span class="sxs-lookup"><span data-stu-id="5ab73-461">font-size</span></span> | <span data-ttu-id="5ab73-462">`style="font-size:10pt"`（默认为 11pt）</span><span class="sxs-lookup"><span data-stu-id="5ab73-462">style="font-size:10pt"`style="font-size:10pt"` (defaults to 11pt)</span></span><br /><span data-ttu-id="5ab73-463">API 接受 *pt* 或 *px* 的字体大小，但会将 *px* 转换为 *pt*。</span><span class="sxs-lookup"><span data-stu-id="5ab73-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="5ab73-464">十进制值被四舍五入为最接近的 n.0pt 或 n.5pt。</span><span class="sxs-lookup"><span data-stu-id="5ab73-464">The onnvshort API accepts font size in pt or px, but converts px to pt. Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="5ab73-465">font-style</span><span class="sxs-lookup"><span data-stu-id="5ab73-465">font-style</span></span> | <span data-ttu-id="5ab73-466">`style="font-style:italic"`（正常或仅倾斜）</span><span class="sxs-lookup"><span data-stu-id="5ab73-466">style="font-style:italic"`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="5ab73-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="5ab73-467">font-weight</span></span> | <span data-ttu-id="5ab73-468">`style="font-weight:bold"`（正常或仅加粗）</span><span class="sxs-lookup"><span data-stu-id="5ab73-468">style="font-weight:bold"`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="5ab73-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="5ab73-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="5ab73-470">text-align</span><span class="sxs-lookup"><span data-stu-id="5ab73-470">text-align</span></span> | <span data-ttu-id="5ab73-471">`style="text-align:center"`（仅适用于块元素）</span><span class="sxs-lookup"><span data-stu-id="5ab73-471">style="text-align:center"`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="5ab73-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="5ab73-472">text-decoration</span></span> | <span data-ttu-id="5ab73-473">`style="text-decoration:underline"`（无或仅加下划线）</span><span class="sxs-lookup"><span data-stu-id="5ab73-473">style="text-decoration:underline"`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="5ab73-474">另外，还支持下列内联字符样式：</span><span class="sxs-lookup"><span data-stu-id="5ab73-474">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="5ab73-475">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-475">B</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-476">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-476">&lt;i&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-477">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-477">/u</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5ab73-478">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-478">
EM 
</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-479">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-479">Strong.</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-480">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-480">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5ab73-481">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-481">Scr sup.</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-482">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-482">&lt;Sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="5ab73-483">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-483">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="5ab73-484">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="5ab73-484">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="5ab73-485">输入和输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="5ab73-485">Input and output HTML example</span></span>
<span data-ttu-id="5ab73-486">下图显示了使用 Microsoft Graph 创建的简单页面。</span><span class="sxs-lookup"><span data-stu-id="5ab73-486">The following image shows a simple page that was created with the onnvshort API.</span></span>

![包含维基百科中的内容的学习笔记的 OneNote 页的图像](images/onenote-sample-image.png)

<span data-ttu-id="5ab73-488">这是在创建页面的邮件正文中发送的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-488">This is the input HTML that was sent in the request body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="http://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<span data-ttu-id="5ab73-489">这是[获取页面内容](../api-reference/v1.0/api/page_get.md)时 Microsoft Graph 返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="5ab73-489">This is the output HTML that the onnvshort API returns when you get the page content.</span></span>

><span data-ttu-id="5ab73-490">**注意：**[创建页面](../api-reference/v1.0/api/section_post_pages.md)或[获取页面元数据](../api-reference/v1.0/api/page_get.md)时，API 返回 **contentUrl** 属性中的页面的 *content* 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="5ab73-490">**Note:** When you [create a page](../api-reference/v1.0/api/section_post_pages.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="5ab73-491">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5ab73-491">See also</span></span>

- [<span data-ttu-id="5ab73-492">获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="5ab73-492">Get OneNote content and structure</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="5ab73-493">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="5ab73-493">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
- [<span data-ttu-id="5ab73-494">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="5ab73-494">Update page content</span></span>](../api-reference/v1.0/api/page_update.md)
- [<span data-ttu-id="5ab73-495">添加图像和文件</span><span class="sxs-lookup"><span data-stu-id="5ab73-495">Add images and files</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)
