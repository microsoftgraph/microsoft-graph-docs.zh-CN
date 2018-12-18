---
title: OneNote 页中的输入和输出 HTML
description: '创建或更新 OneNote 页时定义页面内容和结构的 HTML 被称为*输入 HTML*。 '
author: Jewan-microsoft
ms.openlocfilehash: e169cf17804794d5120b2e968328b06d29a0a5a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351252"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="23db0-103">OneNote 页中的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="23db0-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="23db0-104">[创建](onenote-create-page.md)或[更新](onenote-update-page.md) OneNote 页时定义页面内容和结构的 HTML 被称为*输入 HTML*。</span><span class="sxs-lookup"><span data-stu-id="23db0-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="23db0-105">[获取页面内容](onenote-get-content.md)时返回的 HTML 被称为*输出 HTML*。</span><span class="sxs-lookup"><span data-stu-id="23db0-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="23db0-106">输出 HTML 与输入 HTML 存在差别。</span><span class="sxs-lookup"><span data-stu-id="23db0-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="23db0-107">Microsoft Graph 中的 OneNote API 保留输入 HTML 的语义内容和基本结构，但会将其转换为一组[受支持的 HTML 元素和 CSS 属性](onenote-create-page.md#supported-html-and-css-for-onenote-pages)。</span><span class="sxs-lookup"><span data-stu-id="23db0-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="23db0-108">API 还添加支持 OneNote 功能的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="23db0-109">本文介绍输入和输出 HTML 的主体元素和属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="23db0-110">它可以帮助你理解创建或更新页面内容时的输入 HTML 以及分析返回的页面内容时的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="23db0-111">body 元素</span><span class="sxs-lookup"><span data-stu-id="23db0-111">body element</span></span>

<span data-ttu-id="23db0-112">页面正文中的 HTML 内容表示页面内容和结构，其中包括图像和文件资源。</span><span class="sxs-lookup"><span data-stu-id="23db0-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="23db0-113">**body** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-114">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-114">Input attributes</span></span>

|<span data-ttu-id="23db0-115">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-115">Input attribute</span></span>|<span data-ttu-id="23db0-116">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="23db0-117">data-absolute-enabled</span></span> | <span data-ttu-id="23db0-118">指示输入正文是否支持[绝对定位](onenote-abs-pos.md)元素。</span><span class="sxs-lookup"><span data-stu-id="23db0-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="23db0-119">style</span><span class="sxs-lookup"><span data-stu-id="23db0-119">style</span></span> | <p><span data-ttu-id="23db0-120">正文的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="23db0-121">在输出 HTML 中，可能在相应的子元素上内嵌返回输入设置。</span><span class="sxs-lookup"><span data-stu-id="23db0-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="23db0-122">**body** 元素当前不支持背景色。</span><span class="sxs-lookup"><span data-stu-id="23db0-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-123">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-123">Output attributes</span></span>

|<span data-ttu-id="23db0-124">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-124">Output attribute</span></span>|<span data-ttu-id="23db0-125">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="23db0-126">data-absolute-enabled</span></span> | <span data-ttu-id="23db0-127">指示正文是否支持[绝对定位](onenote-abs-pos.md)元素。</span><span class="sxs-lookup"><span data-stu-id="23db0-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="23db0-128">在输出 HTML 中始终为 **true**。</span><span class="sxs-lookup"><span data-stu-id="23db0-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="23db0-129">style</span><span class="sxs-lookup"><span data-stu-id="23db0-129">style</span></span> | <span data-ttu-id="23db0-130">正文的 **font-family** 和 **font-size** 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="23db0-131">div 元素</span><span class="sxs-lookup"><span data-stu-id="23db0-131">div elements</span></span>

<span data-ttu-id="23db0-132">**Div** 元素包含文本、图像和其他内容。</span><span class="sxs-lookup"><span data-stu-id="23db0-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="23db0-133">**div** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-134">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-134">Input attributes</span></span>

|<span data-ttu-id="23db0-135">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-135">Input attribute</span></span>|<span data-ttu-id="23db0-136">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-137">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-137">data-id</span></span> | <span data-ttu-id="23db0-138">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-139">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="23db0-140">data-render-fallback</span></span> | <span data-ttu-id="23db0-141">[提取](onenote-extract-data.md)失败时的回退操作：**render**（默认）或 **none**</span><span class="sxs-lookup"><span data-stu-id="23db0-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="23db0-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="23db0-142">data-render-method</span></span> | <span data-ttu-id="23db0-143">要执行的[提取](onenote-extract-data.md)方法，例如：</span><span class="sxs-lookup"><span data-stu-id="23db0-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="23db0-144">`extract.businesscard` 或 `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="23db0-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="23db0-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="23db0-145">data-render-src</span></span> | <span data-ttu-id="23db0-146">[提取](onenote-extract-data.md)的内容源。</span><span class="sxs-lookup"><span data-stu-id="23db0-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="23db0-147">style</span><span class="sxs-lookup"><span data-stu-id="23db0-147">style</span></span> | <span data-ttu-id="23db0-148">div 的位置、大小、字体和颜色属性：</span><span class="sxs-lookup"><span data-stu-id="23db0-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="23db0-149">**位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**（会为 div 自动配置高度）</span><span class="sxs-lookup"><span data-stu-id="23db0-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="23db0-150">用于创建[绝对定位](onenote-abs-pos.md) div（仅在正文设置 `data-absolute-enabled="true"` 且 div 是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="23db0-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="23db0-151">示例：`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="23db0-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="23db0-p108">元素的 CSS [样式](#styles)属性。在输出 HTML 中，这些值在适当的子元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="23db0-154">Microsoft Graph 中的 OneNote API 至少在一个 div 中包装所有正文内容。</span><span class="sxs-lookup"><span data-stu-id="23db0-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="23db0-155">在以下情况下，API 创建一个默认 div（使用 `data-id="_default"` 设定属性）以包含正文内容：</span><span class="sxs-lookup"><span data-stu-id="23db0-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="23db0-156">输入 body 元素的 **data-absolute-enabled** 属性被省略或被设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="23db0-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="23db0-157">在此情况下，所有正文内容都被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="23db0-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="23db0-158">输入 body 元素的 **data-absolute-enabled** 属性为 **true**，但输入 HTML 包含的直接子级不是[绝对定位](onenote-abs-pos.md)&nbsp; **div**、**img** 或 **object** 元素。</span><span class="sxs-lookup"><span data-stu-id="23db0-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="23db0-159">在此情况下，不是[绝对定位](onenote-abs-pos.md)&nbsp; **div**、**img** 或 **object** 元素的直接子级被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="23db0-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="23db0-160">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-160">Output attributes</span></span>

|<span data-ttu-id="23db0-161">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-161">Output attribute</span></span>|<span data-ttu-id="23db0-162">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-163">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-163">data-id</span></span> | <span data-ttu-id="23db0-164">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-165">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-166">id</span><span class="sxs-lookup"><span data-stu-id="23db0-166">id</span></span> | <span data-ttu-id="23db0-167">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-168">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-169">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-170">style</span><span class="sxs-lookup"><span data-stu-id="23db0-170">style</span></span> | <span data-ttu-id="23db0-171">div 的位置和大小属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="23db0-172">非贡献 div</span><span class="sxs-lookup"><span data-stu-id="23db0-172">Non-contributing divs</span></span>

<span data-ttu-id="23db0-173">当输入 HTML 中的 **div** 元素不对页面结构做出贡献或带有 OneNote 所使用的信息时，此 API 将 div 的内容移动到父 div 或默认 div。</span><span class="sxs-lookup"><span data-stu-id="23db0-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="23db0-174">下面的示例对此进行了说明。</span><span class="sxs-lookup"><span data-stu-id="23db0-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="23db0-175">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="23db0-175">Input HTML</span></span>

<span data-ttu-id="23db0-176">包含非贡献嵌套 div。</span><span class="sxs-lookup"><span data-stu-id="23db0-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="23db0-177">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="23db0-177">Output HTML</span></span>

> <span data-ttu-id="23db0-178">**注意**：div 的内容已被移至父 div 且嵌套的 `<div>` 标记已被删除。</span><span class="sxs-lookup"><span data-stu-id="23db0-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="23db0-179">如果 div 定义了任何语义信息，例如 **data-id**（示例：`<div data-id="keep-me">`），则保留该 div。</span><span class="sxs-lookup"><span data-stu-id="23db0-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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


## <a name="img-elements"></a><span data-ttu-id="23db0-180">img 元素</span><span class="sxs-lookup"><span data-stu-id="23db0-180">img elements</span></span>

<span data-ttu-id="23db0-181">OneNote 页上的图像由 **img** 元素表示。</span><span class="sxs-lookup"><span data-stu-id="23db0-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="23db0-182">**img** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-183">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-183">Input attributes</span></span>

|<span data-ttu-id="23db0-184">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-184">Input attribute</span></span>|<span data-ttu-id="23db0-185">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-186">alt</span><span class="sxs-lookup"><span data-stu-id="23db0-186">alt</span></span> | <span data-ttu-id="23db0-187">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="23db0-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="23db0-188">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-188">data-id</span></span> | <span data-ttu-id="23db0-189">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-190">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="23db0-191">data-render-src</span></span> |<span data-ttu-id="23db0-192">需要 **data-render-src** 或 **src**。</span><span class="sxs-lookup"><span data-stu-id="23db0-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="23db0-193">在 OneNote 页上显示为位图图像的网页：</span><span class="sxs-lookup"><span data-stu-id="23db0-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="23db0-194">- `data-render-src="https://..."` 表示公共 URL。</span><span class="sxs-lookup"><span data-stu-id="23db0-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="23db0-195">- `data-render-src="name:BlockName"` 表示[多部分请求](/graph/api/section-post-pages?view=graph-rest-1.0#example)的“演示文稿”块中的图像部分。</span><span class="sxs-lookup"><span data-stu-id="23db0-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="23db0-196">如果网页比 OneNote 页能够忠实呈现的内容更为复杂，或者页面需要登录凭据，则此方法很有用。</span><span class="sxs-lookup"><span data-stu-id="23db0-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="23db0-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-197">data-tag</span></span> | <span data-ttu-id="23db0-198">元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="23db0-199">style</span><span class="sxs-lookup"><span data-stu-id="23db0-199">style</span></span> |<span data-ttu-id="23db0-200">图像的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**、**宽度**和**高度**。</span><span class="sxs-lookup"><span data-stu-id="23db0-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="23db0-201">可在任何图像上设置大小。</span><span class="sxs-lookup"><span data-stu-id="23db0-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="23db0-202">位置属性用于创建[绝对定位](onenote-abs-pos.md)图像（仅在正文设置 `data-absolute-enabled="true"` 且图像是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="23db0-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="23db0-203">示例：`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="23db0-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="23db0-204">在输出 HTML 中，图像大小分别以 **width** 和 **height** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="23db0-205">src</span><span class="sxs-lookup"><span data-stu-id="23db0-205">src</span></span> |<span data-ttu-id="23db0-206">需要 **src** 或 **data-render-src**。</span><span class="sxs-lookup"><span data-stu-id="23db0-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="23db0-207">要在 OneNote 页上呈现的图像：</span><span class="sxs-lookup"><span data-stu-id="23db0-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="23db0-208">- `src="https://..."` 表示 Internet 上公开可用图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="23db0-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="23db0-209">- `src="name:BlockName"` 表示代表此图像的多部分请求中的已命名部分。</span><span class="sxs-lookup"><span data-stu-id="23db0-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="23db0-210">width，height</span><span class="sxs-lookup"><span data-stu-id="23db0-210">width, height</span></span> | <span data-ttu-id="23db0-211">图像的宽度或高度，以不带 px 的像素为单位。</span><span class="sxs-lookup"><span data-stu-id="23db0-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="23db0-212">示例：`width="400"`</span><span class="sxs-lookup"><span data-stu-id="23db0-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="23db0-213">**注意：** OneNote API 自动检测输入图像类型，并在输出 HTML 中将其返回为 **data-fullres-src-type**。</span><span class="sxs-lookup"><span data-stu-id="23db0-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="23db0-214">此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="23db0-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-215">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-215">Output attributes</span></span>

|<span data-ttu-id="23db0-216">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-216">Output attribute</span></span>|<span data-ttu-id="23db0-217">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-218">alt</span><span class="sxs-lookup"><span data-stu-id="23db0-218">alt</span></span> | <span data-ttu-id="23db0-219">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="23db0-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="23db0-220">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-220">data-id</span></span> | <span data-ttu-id="23db0-221">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-222">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-223">data-index</span><span class="sxs-lookup"><span data-stu-id="23db0-223">data-index</span></span> | <span data-ttu-id="23db0-p118">此图像的位置。用于支持[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="23db0-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="23db0-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="23db0-226">data-fullres-src</span></span> | <span data-ttu-id="23db0-227">最初嵌入在页面中的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="23db0-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="23db0-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="23db0-228">data-fullres-src-type</span></span> | <span data-ttu-id="23db0-229">**data-fullres-src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="23db0-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="23db0-230">data-options</span><span class="sxs-lookup"><span data-stu-id="23db0-230">data-options</span></span> | <span data-ttu-id="23db0-p119">源类型：PDF 文件的源类型为 **printout**，而所有其他文件的源类型为 **splitimage**。仅适用于使用 **data-render-src** 属性创建的[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="23db0-p119">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="23db0-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="23db0-233">data-render-original-src</span></span> | <span data-ttu-id="23db0-234">此图像的原始源 URL，前提是该源图像来自公共 Internet，且使用 **data-render-src** 属性创建。</span><span class="sxs-lookup"><span data-stu-id="23db0-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="23db0-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="23db0-235">data-src-type</span></span> | <span data-ttu-id="23db0-236">**src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="23db0-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="23db0-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-237">data-tag</span></span> | <span data-ttu-id="23db0-238">元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="23db0-239">id</span><span class="sxs-lookup"><span data-stu-id="23db0-239">id</span></span> | <span data-ttu-id="23db0-240">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-241">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-242">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-243">src</span><span class="sxs-lookup"><span data-stu-id="23db0-243">src</span></span> | <span data-ttu-id="23db0-244">已针对 Web 浏览器以及移动设备和平板电脑外形规格进行优化的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="23db0-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="23db0-245">style</span><span class="sxs-lookup"><span data-stu-id="23db0-245">style</span></span> | <span data-ttu-id="23db0-246">此图像的位置属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-246">The position properties of the image.</span></span> |
| <span data-ttu-id="23db0-247">width、height</span><span class="sxs-lookup"><span data-stu-id="23db0-247">width, height</span></span> | <span data-ttu-id="23db0-248">此图像的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="23db0-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="23db0-249">图像的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="23db0-249">Output HTML examples for images</span></span>

<span data-ttu-id="23db0-250">输出 **img** 元素包含图像文件资源的终结点和图像类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="23db0-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="23db0-251">可以发出单独的[图像资源终结点的 GET 请求](/graph/api/resource-get?view=graph-rest-1.0)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="23db0-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="23db0-252">默认情况下，图像并不会直接在浏览器中显示，因为它们具有私密性，需要授权才能对其检索，这与页面其他内容一样。</span><span class="sxs-lookup"><span data-stu-id="23db0-252">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="23db0-253">若要获取页面上的图像资源的公共 URL，请在检索页面内容时，在查询字符串中添加 **preAuthenticated=true**（例如：`GET ../pages/{page-id}/content?preAuthenticated=true`）。</span><span class="sxs-lookup"><span data-stu-id="23db0-253">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="23db0-254">返回的公共 URL 的有效期为一小时。</span><span class="sxs-lookup"><span data-stu-id="23db0-254">The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="23db0-255">在请求中添加 _preAuthenticated=true_ 时带有公共 URL 的图像</span><span class="sxs-lookup"><span data-stu-id="23db0-255">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="23db0-256">以下示例说明 **img** 元素在输出 HTML 中可能包含的信息。</span><span class="sxs-lookup"><span data-stu-id="23db0-256">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="23db0-257">带有 Web 安全和高分辨率资源的图像</span><span class="sxs-lookup"><span data-stu-id="23db0-257">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="23db0-258">通过使用 *data-render-src* 属性创建的图像</span><span class="sxs-lookup"><span data-stu-id="23db0-258">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="23db0-259">拆分图像</span><span class="sxs-lookup"><span data-stu-id="23db0-259">Split images</span></span>

<span data-ttu-id="23db0-260">出于性能和呈现的考虑，使用 **data-render-src** 属性（从网页 URL 或已命名的部分）创建的图像可能被拆分为多个组件图像。</span><span class="sxs-lookup"><span data-stu-id="23db0-260">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="23db0-261">向所有组件映像分配同一 **data-id** 值。</span><span class="sxs-lookup"><span data-stu-id="23db0-261">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="23db0-262">每个组件图像均具有从零开始的数据索引属性，该属性定义原始垂直布局。</span><span class="sxs-lookup"><span data-stu-id="23db0-262">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="23db0-263">带有三个组件图像的拆分图像</span><span class="sxs-lookup"><span data-stu-id="23db0-263">Split image with three component images</span></span>

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

<span data-ttu-id="23db0-264">用户可以在页面上移动图像，因此返回的索引可能是无序的。</span><span class="sxs-lookup"><span data-stu-id="23db0-264">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="23db0-265">排序方法应采用从上到下的 Y 轴排序，如果 Y 轴顺序存在冲突，则从左到右按 X 轴进行排序。</span><span class="sxs-lookup"><span data-stu-id="23db0-265">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="23db0-266">iframe 元素</span><span class="sxs-lookup"><span data-stu-id="23db0-266">iframe elements</span></span>

<span data-ttu-id="23db0-267">OneNote 页可包含由 **iframe** 元素所表示的嵌入的视频。</span><span class="sxs-lookup"><span data-stu-id="23db0-267">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="23db0-268">**注意：** 也可以[使用 **object** 元素附加视频文件](onenote-images-files.md#adding-files)。</span><span class="sxs-lookup"><span data-stu-id="23db0-268">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-269">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-269">Input attributes</span></span>

|<span data-ttu-id="23db0-270">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-270">Input attribute</span></span>|<span data-ttu-id="23db0-271">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-271">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-272">data-original-src</span><span class="sxs-lookup"><span data-stu-id="23db0-272">data-original-src</span></span> | <span data-ttu-id="23db0-273">必需。</span><span class="sxs-lookup"><span data-stu-id="23db0-273">Required.</span></span> <span data-ttu-id="23db0-274">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="23db0-274">The URL of the video source.</span></span> <span data-ttu-id="23db0-275">请参阅[受支持的视频源的列表](onenote-images-files.md#adding-videos)。</span><span class="sxs-lookup"><span data-stu-id="23db0-275">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="23db0-276">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="23db0-276">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="23db0-277">width，height</span><span class="sxs-lookup"><span data-stu-id="23db0-277">width, height</span></span> | <span data-ttu-id="23db0-278">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="23db0-278">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="23db0-279">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="23db0-279">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="23db0-280">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-280">Output attributes</span></span>

|<span data-ttu-id="23db0-281">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-281">Output attribute</span></span>|<span data-ttu-id="23db0-282">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-282">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-283">data-original-src</span><span class="sxs-lookup"><span data-stu-id="23db0-283">data-original-src</span></span> | <span data-ttu-id="23db0-284">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="23db0-284">The URL of the video source.</span></span> |
| <span data-ttu-id="23db0-285">src</span><span class="sxs-lookup"><span data-stu-id="23db0-285">src</span></span> | <span data-ttu-id="23db0-286">在 OneNote 页中嵌入的视频的链接。</span><span class="sxs-lookup"><span data-stu-id="23db0-286">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="23db0-287">width，height</span><span class="sxs-lookup"><span data-stu-id="23db0-287">width, height</span></span> | <span data-ttu-id="23db0-288">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="23db0-288">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="23db0-289">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="23db0-289">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="23db0-290">视频的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="23db0-290">Output HTML example for videos</span></span>

<span data-ttu-id="23db0-291">输出 **iframe** 元素包含链接到源页面和视频的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="23db0-291">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="23db0-292">object 元素</span><span class="sxs-lookup"><span data-stu-id="23db0-292">object elements</span></span>

<span data-ttu-id="23db0-293">OneNote 页可包含由 **object** 元素表示的文件附件。</span><span class="sxs-lookup"><span data-stu-id="23db0-293">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="23db0-294">**object** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-294">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="23db0-295">**注意：** 将文件发送为图像并使用 **data-render-src** 属性时，OneNote API 还可以将此文件的内容呈现为页面中的图像。</span><span class="sxs-lookup"><span data-stu-id="23db0-295">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="23db0-296">示例：`<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="23db0-296">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="23db0-297">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-297">Input attributes</span></span>

|<span data-ttu-id="23db0-298">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-298">Input attribute</span></span>|<span data-ttu-id="23db0-299">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-299">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-300">data</span><span class="sxs-lookup"><span data-stu-id="23db0-300">data</span></span> | <span data-ttu-id="23db0-301">必需。</span><span class="sxs-lookup"><span data-stu-id="23db0-301">Required.</span></span> <span data-ttu-id="23db0-302">表示[多部分请求](/graph/api/section-post-pages?view=graph-rest-1.0#example)中文件的部分的名称。</span><span class="sxs-lookup"><span data-stu-id="23db0-302">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="23db0-303">data-attachment</span><span class="sxs-lookup"><span data-stu-id="23db0-303">data-attachment</span></span> | <span data-ttu-id="23db0-p130">必需。文件名。</span><span class="sxs-lookup"><span data-stu-id="23db0-p130">Required. The file name.</span></span> |
| <span data-ttu-id="23db0-306">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-306">data-id</span></span> | <span data-ttu-id="23db0-307">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-307">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-308">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-308">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-309">style</span><span class="sxs-lookup"><span data-stu-id="23db0-309">style</span></span> | <span data-ttu-id="23db0-310">对象的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**。</span><span class="sxs-lookup"><span data-stu-id="23db0-310">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="23db0-311">用于创建[绝对定位](onenote-abs-pos.md)对象（仅在正文设置 `data-absolute-enabled="true"` 且对象是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="23db0-311">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="23db0-312">示例：`<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="23db0-312">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="23db0-313">type</span><span class="sxs-lookup"><span data-stu-id="23db0-313">type</span></span> | <span data-ttu-id="23db0-314">必需。</span><span class="sxs-lookup"><span data-stu-id="23db0-314">Required.</span></span><br/><br/><span data-ttu-id="23db0-315">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="23db0-315">The standard media file type.</span></span> <span data-ttu-id="23db0-316">已知文件类型显示与 OneNote 页上的文件类型相关联的图标。</span><span class="sxs-lookup"><span data-stu-id="23db0-316">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="23db0-317">已知文件类型显示通用文件图标。</span><span class="sxs-lookup"><span data-stu-id="23db0-317">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-318">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-318">Output attributes</span></span>

|<span data-ttu-id="23db0-319">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-319">Output attribute</span></span>|<span data-ttu-id="23db0-320">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-320">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-321">data</span><span class="sxs-lookup"><span data-stu-id="23db0-321">data</span></span> | <span data-ttu-id="23db0-322">文件资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="23db0-322">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="23db0-323">data-attachment</span><span class="sxs-lookup"><span data-stu-id="23db0-323">data-attachment</span></span> | <span data-ttu-id="23db0-324">文件名。</span><span class="sxs-lookup"><span data-stu-id="23db0-324">The file name.</span></span> |
| <span data-ttu-id="23db0-325">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-325">data-id</span></span> | <span data-ttu-id="23db0-326">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-326">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-327">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-328">id</span><span class="sxs-lookup"><span data-stu-id="23db0-328">id</span></span> | <span data-ttu-id="23db0-329">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-329">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-330">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-330">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-331">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-331">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-332">style</span><span class="sxs-lookup"><span data-stu-id="23db0-332">style</span></span> | <span data-ttu-id="23db0-333">此对象的位置属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-333">The position properties of the object.</span></span> |
| <span data-ttu-id="23db0-334">type</span><span class="sxs-lookup"><span data-stu-id="23db0-334">type</span></span> | <span data-ttu-id="23db0-335">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="23db0-335">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="23db0-336">对象的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="23db0-336">Output HTML example for objects</span></span>

<span data-ttu-id="23db0-337">输出 **object** 元素包含链接到页面中的文件资源的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="23db0-337">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="23db0-338">可以发出单独的[文件资源终结点的 GET 请求](/graph/api/resource-get?view=graph-rest-1.0)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="23db0-338">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="23db0-339">段落和标题</span><span class="sxs-lookup"><span data-stu-id="23db0-339">Paragraphs and headings</span></span>

<span data-ttu-id="23db0-340">段落、标题和其他文本容器可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-340">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-341">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-341">Input attributes</span></span>

|<span data-ttu-id="23db0-342">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-342">Input attribute</span></span>|<span data-ttu-id="23db0-343">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-343">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-344">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-344">data-id</span></span> | <span data-ttu-id="23db0-345">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-345">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-346">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-346">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-347">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-347">data-tag</span></span> | <span data-ttu-id="23db0-348">**p** 或 **h1** - **h6** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-348">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="23db0-349">style</span><span class="sxs-lookup"><span data-stu-id="23db0-349">style</span></span> | <span data-ttu-id="23db0-350">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-350">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-351">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-351">Output attributes</span></span>

|<span data-ttu-id="23db0-352">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-352">Output attribute</span></span>|<span data-ttu-id="23db0-353">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-353">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-354">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-354">data-id</span></span> | <span data-ttu-id="23db0-355">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-355">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-356">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-356">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-357">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-357">data-tag</span></span> | <span data-ttu-id="23db0-358">**p** 或 **h1** - **h6** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-358">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="23db0-359">id</span><span class="sxs-lookup"><span data-stu-id="23db0-359">id</span></span> | <span data-ttu-id="23db0-360">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-360">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-361">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-361">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-362">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-362">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-363">style</span><span class="sxs-lookup"><span data-stu-id="23db0-363">style</span></span> | <span data-ttu-id="23db0-364">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-364">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="23db0-365">在输出 HTML 中，可能在相应的子元素或 **span** 元素上内嵌返回这些值。</span><span class="sxs-lookup"><span data-stu-id="23db0-365">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="23db0-366">以下示例显示使用不同方法定义文本容器样式的输入 HTML 和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-366">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="23db0-367">在 span 元素的起始标记中使用内联字符样式定义样式的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-367">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="23db0-368">带有 `<i>` 字符样式以及 `<p>` 起始标记中的字体设置的输出 HTML 作为 span 元素上的内联 CSS 样式返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-368">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="23db0-369">列表</span><span class="sxs-lookup"><span data-stu-id="23db0-369">Lists</span></span>

<span data-ttu-id="23db0-370">列表表示为包含由 **li** 元素所表示的列表项的 **ol** 或 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="23db0-370">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="23db0-371">列表和列表项可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-371">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="23db0-372">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-372">Input attributes</span></span>

|<span data-ttu-id="23db0-373">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-373">Input attribute</span></span>|<span data-ttu-id="23db0-374">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-374">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-375">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-375">data-id</span></span> | <span data-ttu-id="23db0-376">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-376">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-377">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-377">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-378">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-378">data-tag</span></span> | <span data-ttu-id="23db0-379">**ul**、**ol** 或 **li** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-379">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="23db0-380">style</span><span class="sxs-lookup"><span data-stu-id="23db0-380">style</span></span> | <span data-ttu-id="23db0-381">列表或列表项的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-381">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-382">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-382">Output attributes</span></span>

|<span data-ttu-id="23db0-383">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-383">Output attribute</span></span>|<span data-ttu-id="23db0-384">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-384">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-385">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-385">data-id</span></span> | <span data-ttu-id="23db0-386">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-386">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-387">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-387">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-388">data-tag</span><span class="sxs-lookup"><span data-stu-id="23db0-388">data-tag</span></span> |  <span data-ttu-id="23db0-389">**li** 元素中的 span 上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-389">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="23db0-390">id</span><span class="sxs-lookup"><span data-stu-id="23db0-390">id</span></span> | <span data-ttu-id="23db0-391">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-391">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-392">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-392">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-393">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-393">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-394">style</span><span class="sxs-lookup"><span data-stu-id="23db0-394">style</span></span> | <span data-ttu-id="23db0-395">元素的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-395">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="23db0-396">在输出 HTML 中，在列表项上返回列表级别设置。</span><span class="sxs-lookup"><span data-stu-id="23db0-396">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="23db0-397">不会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-397">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="23db0-398">列表样式</span><span class="sxs-lookup"><span data-stu-id="23db0-398">List styles</span></span>

<span data-ttu-id="23db0-399">Microsoft Graph 中的 OneNote API 支持以下列表样式：</span><span class="sxs-lookup"><span data-stu-id="23db0-399">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="23db0-400">已排序列表</span><span class="sxs-lookup"><span data-stu-id="23db0-400">Ordered list</span></span>|<span data-ttu-id="23db0-401">未排序列表</span><span class="sxs-lookup"><span data-stu-id="23db0-401">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-402">无</span><span class="sxs-lookup"><span data-stu-id="23db0-402">none</span></span> | <span data-ttu-id="23db0-403">无</span><span class="sxs-lookup"><span data-stu-id="23db0-403">none</span></span> |
| <span data-ttu-id="23db0-404">
decimal (default)</span><span class="sxs-lookup"><span data-stu-id="23db0-404">decimal (default)</span></span> | <span data-ttu-id="23db0-405">
disc (default)</span><span class="sxs-lookup"><span data-stu-id="23db0-405">disc (default)</span></span> |
| <span data-ttu-id="23db0-406">
lower-alpha</span><span class="sxs-lookup"><span data-stu-id="23db0-406">lower-alpha</span></span> | <span data-ttu-id="23db0-407">
circle</span><span class="sxs-lookup"><span data-stu-id="23db0-407">circle</span></span> |
| <span data-ttu-id="23db0-408">
lower-roman</span><span class="sxs-lookup"><span data-stu-id="23db0-408">lower-roman</span></span> | <span data-ttu-id="23db0-409">

square</span><span class="sxs-lookup"><span data-stu-id="23db0-409">square</span></span> |
| <span data-ttu-id="23db0-410">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="23db0-410">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="23db0-411">upper-roman</span><span class="sxs-lookup"><span data-stu-id="23db0-411">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="23db0-412">您可以在输入 HTML 中对 **ol** 或 **ul** 元素上的列表应用全局样式，但样式在 **li** 元素上返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-412">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="23db0-413">同源列表样式</span><span class="sxs-lookup"><span data-stu-id="23db0-413">Homogenous list style</span></span>

<span data-ttu-id="23db0-414">本示例显示了在 **ol** 元素上设置列表样式类型以及在单独列表项上设置 CSS 样式的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-414">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="23db0-p138">这是输出 HTML。请注意，这些样式在单独 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="23db0-417">变量列表样式</span><span class="sxs-lookup"><span data-stu-id="23db0-417">Variable list styles</span></span>

<span data-ttu-id="23db0-418">本示例显示了在 **li** 元素上设置不同列表样式类型的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-418">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="23db0-p139">这是输出 HTML。请注意，这些样式在单独 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-p139">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="23db0-421">表</span><span class="sxs-lookup"><span data-stu-id="23db0-421">Tables</span></span>

<span data-ttu-id="23db0-p140">这些表表示为可以包含 **tr** 和 **td** 元素的 **table** 元素。支持嵌套表。</span><span class="sxs-lookup"><span data-stu-id="23db0-p140">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="23db0-424">表可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-424">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="23db0-425">OneNote API 不支持 **rowspan** 或 **colspan** 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-425">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="23db0-426">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-426">Input attributes</span></span>

|<span data-ttu-id="23db0-427">输入属性</span><span class="sxs-lookup"><span data-stu-id="23db0-427">Input attribute</span></span>|<span data-ttu-id="23db0-428">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-428">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-429">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-429">data-id</span></span> | <span data-ttu-id="23db0-430">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-430">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-431">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-431">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-432">style</span><span class="sxs-lookup"><span data-stu-id="23db0-432">style</span></span> | <span data-ttu-id="23db0-433">此元素的 CSS [style](#styles) 属性，以及：</span><span class="sxs-lookup"><span data-stu-id="23db0-433">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="23db0-434">- **Border**。</span><span class="sxs-lookup"><span data-stu-id="23db0-434">- **border**.</span></span> <span data-ttu-id="23db0-435">可以是 0px，也可以是 1px。</span><span class="sxs-lookup"><span data-stu-id="23db0-435">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="23db0-436">- **width**。</span><span class="sxs-lookup"><span data-stu-id="23db0-436">- **width**.</span></span> <span data-ttu-id="23db0-437">受 **table** 和 **td** 支持作为页面宽度的像素或百分比。</span><span class="sxs-lookup"><span data-stu-id="23db0-437">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="23db0-438">示例：`width="100px"` 或 `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="23db0-438">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="23db0-439">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-439">Output attributes</span></span>

|<span data-ttu-id="23db0-440">输出属性</span><span class="sxs-lookup"><span data-stu-id="23db0-440">Output attribute</span></span>|<span data-ttu-id="23db0-441">说明</span><span class="sxs-lookup"><span data-stu-id="23db0-441">Description</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-442">data-id</span><span class="sxs-lookup"><span data-stu-id="23db0-442">data-id</span></span> | <span data-ttu-id="23db0-443">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="23db0-443">A reference for the element.</span></span><br/><br/><span data-ttu-id="23db0-444">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-445">id</span><span class="sxs-lookup"><span data-stu-id="23db0-445">id</span></span> | <span data-ttu-id="23db0-446">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="23db0-446">A unique, generated ID for the element.</span></span> <span data-ttu-id="23db0-447">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="23db0-447">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="23db0-448">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="23db0-448">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="23db0-449">style</span><span class="sxs-lookup"><span data-stu-id="23db0-449">style</span></span> | <span data-ttu-id="23db0-450">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="23db0-450">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="23db0-451">以下示例显示使用不同方法定义表样式的输入 HTML和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-451">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="23db0-452">具有不同级别可选设置的输入 HTML</span><span class="sxs-lookup"><span data-stu-id="23db0-452">Input HTML with optional settings at different levels</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="23db0-453">具有 CSS 样式的输出 HTML 在 td 元素上内嵌返回</span><span class="sxs-lookup"><span data-stu-id="23db0-453">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="23db0-454">样式</span><span class="sxs-lookup"><span data-stu-id="23db0-454">Styles</span></span>

<span data-ttu-id="23db0-455">Microsoft Graph 中的 OneNote API 支持页面正文中元素的以下内联 CSS **style** 属性，如 **body**、**div**、**p**、**li** 和 **span**。</span><span class="sxs-lookup"><span data-stu-id="23db0-455">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="23db0-456">属性</span><span class="sxs-lookup"><span data-stu-id="23db0-456">Property</span></span>|<span data-ttu-id="23db0-457">示例</span><span class="sxs-lookup"><span data-stu-id="23db0-457">Example</span></span>|
|:------|:------|
| <span data-ttu-id="23db0-458">background-color</span><span class="sxs-lookup"><span data-stu-id="23db0-458">background-color</span></span> | <span data-ttu-id="23db0-459">`style="background-color:#66cc66"`（默认为白色）</span><span class="sxs-lookup"><span data-stu-id="23db0-459">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="23db0-460">支持十六进制格式和命名颜色。</span><span class="sxs-lookup"><span data-stu-id="23db0-460">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="23db0-461">color</span><span class="sxs-lookup"><span data-stu-id="23db0-461">color</span></span> | <span data-ttu-id="23db0-462">`style="color:#ffffff"`（默认为黑色）</span><span class="sxs-lookup"><span data-stu-id="23db0-462">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="23db0-463">font-family</span><span class="sxs-lookup"><span data-stu-id="23db0-463">font-family</span></span> | <span data-ttu-id="23db0-464">`style="font-family:Courier"`（默认为 Calibri）</span><span class="sxs-lookup"><span data-stu-id="23db0-464">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="23db0-465">font-size</span><span class="sxs-lookup"><span data-stu-id="23db0-465">font-size</span></span> | <span data-ttu-id="23db0-466">`style="font-size:10pt"`（默认为 11pt）</span><span class="sxs-lookup"><span data-stu-id="23db0-466">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="23db0-467">API 接受 *pt* 或 *px* 的字体大小，但会将 *px* 转换为 *pt*。</span><span class="sxs-lookup"><span data-stu-id="23db0-467">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="23db0-468">十进制值被四舍五入为最接近的 n.0pt 或 n.5pt。</span><span class="sxs-lookup"><span data-stu-id="23db0-468">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="23db0-469">font-style</span><span class="sxs-lookup"><span data-stu-id="23db0-469">font-style</span></span> | <span data-ttu-id="23db0-470">`style="font-style:italic"`（正常或仅倾斜）</span><span class="sxs-lookup"><span data-stu-id="23db0-470">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="23db0-471">font-weight</span><span class="sxs-lookup"><span data-stu-id="23db0-471">font-weight</span></span> | <span data-ttu-id="23db0-472">`style="font-weight:bold"`（正常或仅加粗）</span><span class="sxs-lookup"><span data-stu-id="23db0-472">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="23db0-473">strike-through</span><span class="sxs-lookup"><span data-stu-id="23db0-473">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="23db0-474">text-align</span><span class="sxs-lookup"><span data-stu-id="23db0-474">text-align</span></span> | <span data-ttu-id="23db0-475">`style="text-align:center"`（仅适用于块元素）</span><span class="sxs-lookup"><span data-stu-id="23db0-475">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="23db0-476">text-decoration</span><span class="sxs-lookup"><span data-stu-id="23db0-476">text-decoration</span></span> | <span data-ttu-id="23db0-477">`style="text-decoration:underline"`（无或仅加下划线）</span><span class="sxs-lookup"><span data-stu-id="23db0-477">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="23db0-478">另外，还支持下列内联字符样式：</span><span class="sxs-lookup"><span data-stu-id="23db0-478">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="23db0-479"><b></span><span class="sxs-lookup"><span data-stu-id="23db0-479"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-480"><i></span><span class="sxs-lookup"><span data-stu-id="23db0-480"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-481"><u></span><span class="sxs-lookup"><span data-stu-id="23db0-481"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="23db0-482"><em></span><span class="sxs-lookup"><span data-stu-id="23db0-482"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-483"><strong></span><span class="sxs-lookup"><span data-stu-id="23db0-483"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-484"><strike></span><span class="sxs-lookup"><span data-stu-id="23db0-484"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="23db0-485"><sup></span><span class="sxs-lookup"><span data-stu-id="23db0-485"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-486"><sub></span><span class="sxs-lookup"><span data-stu-id="23db0-486"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="23db0-487"><del></span><span class="sxs-lookup"><span data-stu-id="23db0-487"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="23db0-488"><cite></span><span class="sxs-lookup"><span data-stu-id="23db0-488"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="23db0-489">输入和输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="23db0-489">Input and output HTML example</span></span>

<span data-ttu-id="23db0-490">下图显示了使用 Microsoft Graph 创建的简单页面。</span><span class="sxs-lookup"><span data-stu-id="23db0-490">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![包含维基百科中的内容的学习笔记的 OneNote 页的图像](images/onenote-sample-image.png)

<span data-ttu-id="23db0-492">这是在创建页面的邮件正文中发送的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-492">This is the input HTML sent in the message body to create the page.</span></span>

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
        <img alt="Apollo 11 commemorative stamp." src="https://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="23db0-493">这是[获取页面内容](onenote-get-content.md)时 Microsoft Graph 返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="23db0-493">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="23db0-494">**注意：**[创建页面](onenote-create-page.md)或[获取页面元数据](/graph/api/page-get?view=graph-rest-1.0)时，API 返回 **contentUrl** 属性中的页面的 *content* 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="23db0-494">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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
            <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="23db0-495">另请参阅</span><span class="sxs-lookup"><span data-stu-id="23db0-495">See also</span></span>

- [<span data-ttu-id="23db0-496">获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="23db0-496">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="23db0-497">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="23db0-497">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="23db0-498">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="23db0-498">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="23db0-499">添加图像、视频和文件</span><span class="sxs-lookup"><span data-stu-id="23db0-499">Add images, videos, and files</span></span>](onenote-images-files.md)
