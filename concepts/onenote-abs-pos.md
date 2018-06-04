
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="60c39-101">在 OneNote 页中创建绝对定位的元素</span><span class="sxs-lookup"><span data-stu-id="60c39-101">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="60c39-102">OneNote 页面的正文可以包含多个直接 `div`、`img` 和 `object` 子元素，可在页面上对其独立定位。</span><span class="sxs-lookup"><span data-stu-id="60c39-102">The body of a onnvshort page can contain multiple direct child elements of type div, img, or object. These child elements can be positioned independently anywhere on the page.</span></span>

<a name="attributes"></a>
## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="60c39-103">属性和定位行为</span><span class="sxs-lookup"><span data-stu-id="60c39-103">Attributes and positioning behavior</span></span>

<span data-ttu-id="60c39-104">使用 `data-absolute-enabled` 和 [`style`](#supported-css-style-attributes) 属性在页面上创建绝对定位的元素，如下所示：</span><span class="sxs-lookup"><span data-stu-id="60c39-104">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="60c39-105">正文元素必须指定 `data-absolute-enabled="true"`。</span><span class="sxs-lookup"><span data-stu-id="60c39-105">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="60c39-106">如果省略或设置为 `false`，则所有正文内容在 API 创建的 `_default` 绝对定位 div 内呈现，所有位置设置将被忽略。</span><span class="sxs-lookup"><span data-stu-id="60c39-106">The body`false` element must specify data-absolute-enabled="true"`_default`. If omitted or set to false, all body content is rendered inside  a _default absolutely positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="60c39-107">只有 `div`、`img` 和 `object` 元素才能是绝对定位的元素。</span><span class="sxs-lookup"><span data-stu-id="60c39-107">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="60c39-108">绝对定位的元素必须指定 `style="position:absolute"`。</span><span class="sxs-lookup"><span data-stu-id="60c39-108">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="60c39-109">绝对定位的元素必须是 `body` 元素的直接子级。</span><span class="sxs-lookup"><span data-stu-id="60c39-109">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="60c39-110">不是绝对定位的 `div`、`img` 或 `object` 元素正文的任何直接子级都将被呈现为绝对定位 `_default` div 内的静态内容。</span><span class="sxs-lookup"><span data-stu-id="60c39-110">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="60c39-111">绝对定位元素位于其指定的顶部和左侧坐标，与页面左上角（在标题区域上方）的 0:0 起始位置相关。</span><span class="sxs-lookup"><span data-stu-id="60c39-111">Absolutely positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the absolute top, left corner of the page (above the title area).</span></span>

- <span data-ttu-id="60c39-112">如果绝对定位的元素省略了顶部或左侧坐标，则缺少的坐标将被设置为其默认值：`top:120px` 或 `left:48px`。</span><span class="sxs-lookup"><span data-stu-id="60c39-112">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="60c39-113">这些默认坐标指定标题区域正下方的位置。</span><span class="sxs-lookup"><span data-stu-id="60c39-113">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="60c39-114">请注意，省略坐标可能会导致元素彼此相互堆叠。</span><span class="sxs-lookup"><span data-stu-id="60c39-114">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="60c39-115">绝对定位元素无法进行嵌套或无法包含定位的元素。</span><span class="sxs-lookup"><span data-stu-id="60c39-115">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="60c39-116">API 忽略在绝对定位的 div 中嵌套元素上指定的任何位置设置，在绝对定位的父 div 中呈现此嵌套内容，并在响应中返回 **api.diagnostics** 属性中的警告。</span><span class="sxs-lookup"><span data-stu-id="60c39-116">Absolutely positioned elements cannot be nested or contain positioned elements. The API ignores any position settings specified on nested elements inside an absolutely positioned div, renders the nested content inside the absolutely positioned parent div, and returns a warning in the **api.diagnostics** property in the  response.</span></span>


# <a name="example"></a><span data-ttu-id="60c39-117">示例</span><span class="sxs-lookup"><span data-stu-id="60c39-117">Example</span></span>

 <span data-ttu-id="60c39-118">下面的示例包含直接 `p` 子级、绝对定位的 div 和非绝对定位的 div。</span><span class="sxs-lookup"><span data-stu-id="60c39-118">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

## <a name="input-html"></a><span data-ttu-id="60c39-119">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="60c39-119">Input HTML</span></span>  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

<span data-ttu-id="60c39-120">API 在默认 div 中呈现非绝对定位的 div。</span><span class="sxs-lookup"><span data-stu-id="60c39-120">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="60c39-121">请注意，嵌套的 `<div>` 标记已被丢弃，因为它们无法定义任何语义信息（例如，`data-id`）。</span><span class="sxs-lookup"><span data-stu-id="60c39-121">Note that the nested  `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

## <a name="output-html"></a><span data-ttu-id="60c39-122">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="60c39-122">Output HTML</span></span> 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

## <a name="example"></a><span data-ttu-id="60c39-123">示例</span><span class="sxs-lookup"><span data-stu-id="60c39-123">Example</span></span>

 <span data-ttu-id="60c39-124">以下示例创建包含一个绝对定位的 div 和一个绝对定位的图像的页面。</span><span class="sxs-lookup"><span data-stu-id="60c39-124">The following example creates a page that contains one absolutely positioned div and one absolutely positioned   image.</span></span>


### <a name="input-html"></a><span data-ttu-id="60c39-125">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="60c39-125">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="60c39-126">OneNote API 评估输入 HTML 并保留所有语义内容和受 OneNote 支持的任何结构信息。</span><span class="sxs-lookup"><span data-stu-id="60c39-126">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="60c39-127">呈现结果页面，如以下图像所示（但不呈现 div 和图像的可见边框）。</span><span class="sxs-lookup"><span data-stu-id="60c39-127">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![含有绝对定位的 div 和图像的结果页面](images/abs-pos.PNG)

<span data-ttu-id="60c39-129">请注意，对来自输入 HTML 的非贡献嵌套 div 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="60c39-129">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="60c39-130">API 保留 div 的内容，但丢弃 `<div>` 标记，因为 div 无法定义语义信息（如 `data-id`）。</span><span class="sxs-lookup"><span data-stu-id="60c39-130">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="60c39-131">有关 OneNote API 如何处理输入和输出 HTML 的详细信息，请参阅 [OneNote 页面的输入和输出 HTML](onenote_input_output_html.md)。</span><span class="sxs-lookup"><span data-stu-id="60c39-131">For more information about how the onnvshort API handles input and output HTML, see Input and output HTML for OneNote pages.</span></span>

<a name="style-attributes"></a>
### <a name="supported-css-style-attributes"></a><span data-ttu-id="60c39-132">受支持的 CSS 样式属性</span><span class="sxs-lookup"><span data-stu-id="60c39-132">Supported CSS style attributes</span></span>

<span data-ttu-id="60c39-133">所有绝对定位的元素都可以指定顶部和左侧位置。</span><span class="sxs-lookup"><span data-stu-id="60c39-133">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="60c39-134">div 和图像可以指定宽度，并且图像还可以指定高度。</span><span class="sxs-lookup"><span data-stu-id="60c39-134">All absolutely positioned elements can  specify top and left positions. Divs and images can specify width, and images can also specify height. For example:</span></span> <span data-ttu-id="60c39-135">例如：</span><span class="sxs-lookup"><span data-stu-id="60c39-135">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="60c39-136">属性</span><span class="sxs-lookup"><span data-stu-id="60c39-136">Attribute</span></span> | <span data-ttu-id="60c39-137">支持的元素</span><span class="sxs-lookup"><span data-stu-id="60c39-137">Supported element</span></span> | <span data-ttu-id="60c39-138">说明</span><span class="sxs-lookup"><span data-stu-id="60c39-138">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="60c39-139">top</span><span class="sxs-lookup"><span data-stu-id="60c39-139">top</span></span> | <span data-ttu-id="60c39-140">div, img, object</span><span class="sxs-lookup"><span data-stu-id="60c39-140">div, img, object</span></span> | <span data-ttu-id="60c39-141">仅以像素为单位的元素顶部边框的 y 轴坐标。</span><span class="sxs-lookup"><span data-stu-id="60c39-141">The y-axis coordinate of the div, img, or object element's top border, in pixels only. Default is 120 pixels.</span></span> <span data-ttu-id="60c39-142">默认值为 120 个像素。</span><span class="sxs-lookup"><span data-stu-id="60c39-142">Default is 120 pixels.</span></span><p><span data-ttu-id="60c39-143">示例：`top:140px`</span><span class="sxs-lookup"><span data-stu-id="60c39-143">Example: `top:140px`</span></span></p> |  
| <span data-ttu-id="60c39-144">left</span><span class="sxs-lookup"><span data-stu-id="60c39-144">left</span></span> |  <span data-ttu-id="60c39-145">div, img, object</span><span class="sxs-lookup"><span data-stu-id="60c39-145">div, img, object</span></span>  | <span data-ttu-id="60c39-146">仅以像素为单位的元素左边框的 x 轴坐标。</span><span class="sxs-lookup"><span data-stu-id="60c39-146">The x-axis coordinate of the div, img, or object element's left border, in pixels only. Default is 48 pixels.</span></span> <span data-ttu-id="60c39-147">默认值为 48 个像素。</span><span class="sxs-lookup"><span data-stu-id="60c39-147">Default is 48 pixels.</span></span><p><span data-ttu-id="60c39-148">示例：`left:95px`</span><span class="sxs-lookup"><span data-stu-id="60c39-148">Example: `left:95px`</span></span></p> |  
| <span data-ttu-id="60c39-149">width</span><span class="sxs-lookup"><span data-stu-id="60c39-149">width</span></span> |  <span data-ttu-id="60c39-150">div, img</span><span class="sxs-lookup"><span data-stu-id="60c39-150">div, img</span></span>  | <span data-ttu-id="60c39-151">仅以像素为单位的元素的宽度。</span><span class="sxs-lookup"><span data-stu-id="60c39-151">The width of the div or img element, in pixels only.</span></span><p><span data-ttu-id="60c39-152">示例：`width:480px`</span><span class="sxs-lookup"><span data-stu-id="60c39-152">Example: `width:480px`</span></span></p> |  
| <span data-ttu-id="60c39-153">height</span><span class="sxs-lookup"><span data-stu-id="60c39-153">height</span></span> | <span data-ttu-id="60c39-154">img</span><span class="sxs-lookup"><span data-stu-id="60c39-154">img</span></span> | <span data-ttu-id="60c39-155">仅以像素为单位的元素的高度。</span><span class="sxs-lookup"><span data-stu-id="60c39-155">The height of the thumbnail, in pixels.</span></span> <span data-ttu-id="60c39-156">对于 div，高度是在运行时计算的，且任何指定的高度值都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="60c39-156">The height of the img element, in pixels only.  For div elements, height is calculated at runtime and any specified height value is ignored.</span></span><p><span data-ttu-id="60c39-157">示例：`height:665px`</span><span class="sxs-lookup"><span data-stu-id="60c39-157">Example: `height:665px`</span></span></p> |  
 
<span data-ttu-id="60c39-158">其他位置属性（如 `z-index`）都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="60c39-158">Other position attributes, such as z-index`z-index`, are ignored.</span></span> <span data-ttu-id="60c39-159">绝对定位的图像可以使用 `data-render-src` 或 `src` 属性。</span><span class="sxs-lookup"><span data-stu-id="60c39-159">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="60c39-160">响应信息</span><span class="sxs-lookup"><span data-stu-id="60c39-160">Response information</span></span>
<span data-ttu-id="60c39-161">OneNote API 在响应中返回以下信息。</span><span class="sxs-lookup"><span data-stu-id="60c39-161">The onnvshort API returns the following information in the response.</span></span>

| <span data-ttu-id="60c39-162">响应数据</span><span class="sxs-lookup"><span data-stu-id="60c39-162">Response data</span></span> | <span data-ttu-id="60c39-163">说明</span><span class="sxs-lookup"><span data-stu-id="60c39-163">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="60c39-164">成功代码</span><span class="sxs-lookup"><span data-stu-id="60c39-164">Success code</span></span> | <span data-ttu-id="60c39-165">成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。</span><span class="sxs-lookup"><span data-stu-id="60c39-165">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="60c39-166">错误</span><span class="sxs-lookup"><span data-stu-id="60c39-166">Errors</span></span> | <span data-ttu-id="60c39-167">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote_error_codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="60c39-167">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="60c39-168">权限</span><span class="sxs-lookup"><span data-stu-id="60c39-168">Permissions</span></span>

<span data-ttu-id="60c39-169">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="60c39-169">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="60c39-170">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="60c39-170">Choose the lowest level of permissions that your app needs to do its work.</span></span>

### <a name="permissions-for-post-pages"></a><span data-ttu-id="60c39-171">_POST 页面_的权限</span><span class="sxs-lookup"><span data-stu-id="60c39-171">Permissions for _POST pages_</span></span> 
- <span data-ttu-id="60c39-172">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="60c39-172">Notes.Create</span></span>
- <span data-ttu-id="60c39-173">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60c39-173">Notes.ReadWrite</span></span>
- <span data-ttu-id="60c39-174">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60c39-174">Notes.ReadWrite.All</span></span>  


### <a name="permissions-for-patch-pages"></a><span data-ttu-id="60c39-175">_PATCH 页面_的权限。</span><span class="sxs-lookup"><span data-stu-id="60c39-175">Permissions for _PATCH pages_</span></span> 

- <span data-ttu-id="60c39-176">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60c39-176">Notes.ReadWrite</span></span>
- <span data-ttu-id="60c39-177">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60c39-177">Notes.ReadWrite.All</span></span>

<span data-ttu-id="60c39-178">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions_reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="60c39-178">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="60c39-179">其他资源</span><span class="sxs-lookup"><span data-stu-id="60c39-179">Additional resources</span></span>

- [<span data-ttu-id="60c39-180">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="60c39-180">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="60c39-181">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="60c39-181">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="60c39-182">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="60c39-182">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="60c39-183">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="60c39-183">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="60c39-184">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="60c39-184">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="60c39-185">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="60c39-185">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

