---
title: 在 OneNote 页中创建绝对定位的元素
description: OneNote 页面的正文可以包含多个直接 `div`、`img` 和 `object` 子元素，可在页面上对其独立定位。
ms.openlocfilehash: 8478f5ae0da4d8c4617573fb99f91646a67d9356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091787"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="5494d-103">在 OneNote 页中创建绝对定位的元素</span><span class="sxs-lookup"><span data-stu-id="5494d-103">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="5494d-104">OneNote 页面的正文可以包含多个直接 `div`、`img` 和 `object` 子元素，可在页面上对其独立定位。</span><span class="sxs-lookup"><span data-stu-id="5494d-104">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="5494d-105">属性和定位操作</span><span class="sxs-lookup"><span data-stu-id="5494d-105">Attributes and positioning behavior</span></span>

<span data-ttu-id="5494d-106">使用 `data-absolute-enabled` 和 [`style`](#supported-css-style-attributes) 属性在页面上创建绝对定位元素，如下所示：</span><span class="sxs-lookup"><span data-stu-id="5494d-106">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="5494d-107">主体元素必须指定`data-absolute-enabled="true"`。</span><span class="sxs-lookup"><span data-stu-id="5494d-107">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="5494d-108">如果省略或设置为 `false`，则所有正文内容在 API 创建的 `_default` 绝对定位 div 内呈现，所有位置设置将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5494d-108">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="5494d-109">只有 `div`， `img`，和 `object` 元素可以是绝对定位的元素。</span><span class="sxs-lookup"><span data-stu-id="5494d-109">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="5494d-110">绝对定位元素必须指定 `style="position:absolute"`。</span><span class="sxs-lookup"><span data-stu-id="5494d-110">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="5494d-111">绝对定位的元素必须是 `body` 元素的直接子元素。</span><span class="sxs-lookup"><span data-stu-id="5494d-111">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="5494d-112">任何非绝对定位的直接的子元素 `div`， `img`， 或`object`元素在绝对定位的`_default` div内呈现为静态内容。</span><span class="sxs-lookup"><span data-stu-id="5494d-112">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="5494d-113">绝对定位元素位于其指定的顶部和左侧坐标，与页面左上角（在标题区域上方）的 0:0 起始位置相关。</span><span class="sxs-lookup"><span data-stu-id="5494d-113">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="5494d-114">如果绝对定位元素忽略了顶部或左侧坐标，那么缺少的坐标将被设置为其默认值： `top:120px` 或者 `left:48px`。</span><span class="sxs-lookup"><span data-stu-id="5494d-114">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="5494d-115">这些默认坐标指定位于标题区域正下方的位置。</span><span class="sxs-lookup"><span data-stu-id="5494d-115">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="5494d-116">请注意，省略坐标可能会导致元素之间相互堆叠在彼此之上。</span><span class="sxs-lookup"><span data-stu-id="5494d-116">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="5494d-117">绝对定位的元素不能嵌套或包含定位元素。</span><span class="sxs-lookup"><span data-stu-id="5494d-117">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="5494d-118">API 忽略在绝对定位的 div 中嵌套元素上指定的任何位置设置，在绝对定位的父 div 中呈现此嵌套内容，并在响应中返回 **api.diagnostics** 属性中的警告。</span><span class="sxs-lookup"><span data-stu-id="5494d-118">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="5494d-119">示例</span><span class="sxs-lookup"><span data-stu-id="5494d-119">Example</span></span>

<span data-ttu-id="5494d-120">下面的示例包含直接 `p` 子级、绝对定位的 div 和非绝对定位的 div。</span><span class="sxs-lookup"><span data-stu-id="5494d-120">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="5494d-121">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="5494d-121">Input HTML</span></span>  

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

<span data-ttu-id="5494d-122">该API呈现默认div中的非绝对定位div。</span><span class="sxs-lookup"><span data-stu-id="5494d-122">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="5494d-123">请注意，嵌套的 `<div>` 标记已被弃用，因为它们无法定义任何语义信息（例如，`data-id`）。</span><span class="sxs-lookup"><span data-stu-id="5494d-123">Note that the nested `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="5494d-124">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="5494d-124">Output HTML</span></span> 

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

### <a name="example"></a><span data-ttu-id="5494d-125">示例</span><span class="sxs-lookup"><span data-stu-id="5494d-125">Example</span></span>

<span data-ttu-id="5494d-126">以下示例创建包含一个绝对定位的 div 和一个绝对定位的图像的页面。</span><span class="sxs-lookup"><span data-stu-id="5494d-126">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="5494d-127">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="5494d-127">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="5494d-128">OneNote API 评估输入 HTML 并保留所有语义内容和受 OneNote 支持的任何结构信息。</span><span class="sxs-lookup"><span data-stu-id="5494d-128">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="5494d-129">结果页面呈现如下图所示（但没有div和图像的可见边框）。</span><span class="sxs-lookup"><span data-stu-id="5494d-129">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![生成具有绝对定位div和图像的页面](images/abs-pos.png)

<span data-ttu-id="5494d-131">注意输入HTML中非贡献的嵌套div的更改。</span><span class="sxs-lookup"><span data-stu-id="5494d-131">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="5494d-132">API保留div的内容但弃置 `<div>` 标签，因为div没有定义语义信息（比如 `data-id`）。</span><span class="sxs-lookup"><span data-stu-id="5494d-132">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="5494d-133">有关 OneNote API 如何处理输入和输出 HTML 的详细信息，请参阅 [OneNote 页面的输入和输出 HTML](onenote-input-output-html.md)。</span><span class="sxs-lookup"><span data-stu-id="5494d-133">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote-input-output-html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="5494d-134">受支持的 CSS 样式属性</span><span class="sxs-lookup"><span data-stu-id="5494d-134">Supported CSS style attributes</span></span>

<span data-ttu-id="5494d-135">所有绝对定位元素都可以指定顶部和左侧位置。</span><span class="sxs-lookup"><span data-stu-id="5494d-135">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="5494d-136">div 和图像可以指定宽度，并且图像还可以指定高度。</span><span class="sxs-lookup"><span data-stu-id="5494d-136">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="5494d-137">例如：</span><span class="sxs-lookup"><span data-stu-id="5494d-137">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="5494d-138">属性</span><span class="sxs-lookup"><span data-stu-id="5494d-138">Attribute</span></span> | <span data-ttu-id="5494d-139">支持的元素</span><span class="sxs-lookup"><span data-stu-id="5494d-139">Supported element</span></span> | <span data-ttu-id="5494d-140">说明</span><span class="sxs-lookup"><span data-stu-id="5494d-140">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="5494d-141">top</span><span class="sxs-lookup"><span data-stu-id="5494d-141">top</span></span> | <span data-ttu-id="5494d-142">div，图像，对象</span><span class="sxs-lookup"><span data-stu-id="5494d-142">div, img, object</span></span> | <span data-ttu-id="5494d-143">仅以像素为单位的元素顶部边框的 y 轴坐标。</span><span class="sxs-lookup"><span data-stu-id="5494d-143">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="5494d-144">默认值是120像素。</span><span class="sxs-lookup"><span data-stu-id="5494d-144">Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="5494d-145">示例： `top:140px`</span><span class="sxs-lookup"><span data-stu-id="5494d-145">Example: `top:140px`</span></span> |  
| <span data-ttu-id="5494d-146">left</span><span class="sxs-lookup"><span data-stu-id="5494d-146">left</span></span> |  <span data-ttu-id="5494d-147">div，图像，对象</span><span class="sxs-lookup"><span data-stu-id="5494d-147">div, img, object</span></span>  | <span data-ttu-id="5494d-148">仅以像素为单位的元素左边框的 x 轴坐标。</span><span class="sxs-lookup"><span data-stu-id="5494d-148">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="5494d-149">默认值是48像素。</span><span class="sxs-lookup"><span data-stu-id="5494d-149">Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="5494d-150">示例： `left:95px`</span><span class="sxs-lookup"><span data-stu-id="5494d-150">Example: `left:95px`</span></span> |  
| <span data-ttu-id="5494d-151">width</span><span class="sxs-lookup"><span data-stu-id="5494d-151">width</span></span> |  <span data-ttu-id="5494d-152">div，图像</span><span class="sxs-lookup"><span data-stu-id="5494d-152">div, img</span></span>  | <span data-ttu-id="5494d-153">仅以像素为单位的元素的宽度。</span><span class="sxs-lookup"><span data-stu-id="5494d-153">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="5494d-154">示例： `width:480px`</span><span class="sxs-lookup"><span data-stu-id="5494d-154">Example: `width:480px`</span></span> |  
| <span data-ttu-id="5494d-155">height</span><span class="sxs-lookup"><span data-stu-id="5494d-155">height</span></span> | <span data-ttu-id="5494d-156">img</span><span class="sxs-lookup"><span data-stu-id="5494d-156">img</span></span> | <span data-ttu-id="5494d-157">仅以像素为单位的元素的高度。</span><span class="sxs-lookup"><span data-stu-id="5494d-157">The height of the element, in pixels only.</span></span> <span data-ttu-id="5494d-158">对于 div，高度是在运行时计算的，且任何指定的高度值都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5494d-158">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="5494d-159">示例： `height:665px`</span><span class="sxs-lookup"><span data-stu-id="5494d-159">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="5494d-160">其他位置属性（如 `z-index`）都将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5494d-160">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="5494d-161">绝对定位的图像可以使用 `data-render-src` 或者 `src` 的属性。</span><span class="sxs-lookup"><span data-stu-id="5494d-161">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="5494d-162">响应信息</span><span class="sxs-lookup"><span data-stu-id="5494d-162">Response information</span></span>

<span data-ttu-id="5494d-163">OneNote API 在响应中返回以下信息。</span><span class="sxs-lookup"><span data-stu-id="5494d-163">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="5494d-164">响应数据</span><span class="sxs-lookup"><span data-stu-id="5494d-164">Response data</span></span> | <span data-ttu-id="5494d-165">说明</span><span class="sxs-lookup"><span data-stu-id="5494d-165">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="5494d-166">成功代码</span><span class="sxs-lookup"><span data-stu-id="5494d-166">Success code</span></span> | <span data-ttu-id="5494d-167">成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。</span><span class="sxs-lookup"><span data-stu-id="5494d-167">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="5494d-168">错误</span><span class="sxs-lookup"><span data-stu-id="5494d-168">Errors</span></span> | <span data-ttu-id="5494d-169">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="5494d-169">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="5494d-170">权限</span><span class="sxs-lookup"><span data-stu-id="5494d-170">Permissions</span></span>

<span data-ttu-id="5494d-171">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="5494d-171">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="5494d-172">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="5494d-172">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="5494d-173">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="5494d-173">Permissions for POST pages</span></span> 

- <span data-ttu-id="5494d-174">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="5494d-174">Notes.Create</span></span>
- <span data-ttu-id="5494d-175">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5494d-175">Notes.ReadWrite</span></span>
- <span data-ttu-id="5494d-176">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5494d-176">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="5494d-177">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="5494d-177">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="5494d-178">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5494d-178">Notes.ReadWrite</span></span>
- <span data-ttu-id="5494d-179">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5494d-179">Notes.ReadWrite.All</span></span>

<span data-ttu-id="5494d-180">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="5494d-180">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="5494d-181">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5494d-181">See also</span></span>

- [<span data-ttu-id="5494d-182">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="5494d-182">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="5494d-183">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="5494d-183">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="5494d-184">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="5494d-184">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="5494d-185">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="5494d-185">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="5494d-186">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="5494d-186">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="5494d-187">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="5494d-187">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

