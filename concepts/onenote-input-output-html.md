---
title: OneNote 页中的输入和输出 HTML
description: '创建或更新 OneNote 页时定义页面内容和结构的 HTML 被称为*输入 HTML*。 '
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 2ba3ce1432a2213a4ecdcfce1ab9a9c98c88c818
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2020
ms.locfileid: "42618771"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="05a3c-103">OneNote 页中的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="05a3c-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="05a3c-104">[创建](onenote-create-page.md)或[更新](onenote-update-page.md) OneNote 页时定义页面内容和结构的 HTML 被称为*输入 HTML*。</span><span class="sxs-lookup"><span data-stu-id="05a3c-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="05a3c-105">[获取页面内容](onenote-get-content.md)时返回的 HTML 被称为*输出 HTML*。</span><span class="sxs-lookup"><span data-stu-id="05a3c-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="05a3c-106">输出 HTML 与输入 HTML 存在差别。</span><span class="sxs-lookup"><span data-stu-id="05a3c-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="05a3c-107">Microsoft Graph 中的 OneNote API 保留输入 HTML 的语义内容和基本结构，但会将其转换为一组[受支持的 HTML 元素和 CSS 属性](onenote-create-page.md#supported-html-and-css-for-onenote-pages)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="05a3c-108">API 还添加支持 OneNote 功能的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="05a3c-109">本文介绍输入和输出 HTML 的主体元素和属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="05a3c-110">它可以帮助你理解创建或更新页面内容时的输入 HTML 以及分析返回的页面内容时的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="05a3c-111">body 元素</span><span class="sxs-lookup"><span data-stu-id="05a3c-111">body element</span></span>

<span data-ttu-id="05a3c-112">页面正文中的 HTML 内容表示页面内容和结构，其中包括图像和文件资源。</span><span class="sxs-lookup"><span data-stu-id="05a3c-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="05a3c-113">**body** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-114">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-114">Input attributes</span></span>

|<span data-ttu-id="05a3c-115">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-115">Input attribute</span></span>|<span data-ttu-id="05a3c-116">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="05a3c-117">data-absolute-enabled</span></span> | <span data-ttu-id="05a3c-118">指示输入正文是否支持[绝对定位](onenote-abs-pos.md)元素。</span><span class="sxs-lookup"><span data-stu-id="05a3c-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="05a3c-119">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-119">style</span></span> | <p><span data-ttu-id="05a3c-120">正文的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="05a3c-121">在输出 HTML 中，可能在相应的子元素上内嵌返回输入设置。</span><span class="sxs-lookup"><span data-stu-id="05a3c-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="05a3c-122">**body** 元素当前不支持背景色。</span><span class="sxs-lookup"><span data-stu-id="05a3c-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-123">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-123">Output attributes</span></span>

|<span data-ttu-id="05a3c-124">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-124">Output attribute</span></span>|<span data-ttu-id="05a3c-125">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="05a3c-126">data-absolute-enabled</span></span> | <span data-ttu-id="05a3c-127">指示正文是否支持[绝对定位](onenote-abs-pos.md)元素。</span><span class="sxs-lookup"><span data-stu-id="05a3c-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="05a3c-128">在输出 HTML 中始终为 **true**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="05a3c-129">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-129">style</span></span> | <span data-ttu-id="05a3c-130">正文的 **font-family** 和 **font-size** 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="05a3c-131">div 元素</span><span class="sxs-lookup"><span data-stu-id="05a3c-131">div elements</span></span>

<span data-ttu-id="05a3c-132">**Div** 元素包含文本、图像和其他内容。</span><span class="sxs-lookup"><span data-stu-id="05a3c-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="05a3c-133">**div** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-134">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-134">Input attributes</span></span>

|<span data-ttu-id="05a3c-135">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-135">Input attribute</span></span>|<span data-ttu-id="05a3c-136">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-137">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-137">data-id</span></span> | <span data-ttu-id="05a3c-138">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-139">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="05a3c-140">data-render-fallback</span></span> | <span data-ttu-id="05a3c-141">[提取](onenote-extract-data.md)失败时的回退操作：**render**（默认）或 **none**</span><span class="sxs-lookup"><span data-stu-id="05a3c-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="05a3c-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="05a3c-142">data-render-method</span></span> | <span data-ttu-id="05a3c-143">要执行的[提取](onenote-extract-data.md)方法，例如：</span><span class="sxs-lookup"><span data-stu-id="05a3c-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="05a3c-144">`extract.businesscard` 或 `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="05a3c-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="05a3c-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-145">data-render-src</span></span> | <span data-ttu-id="05a3c-146">[提取](onenote-extract-data.md)的内容源。</span><span class="sxs-lookup"><span data-stu-id="05a3c-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="05a3c-147">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-147">style</span></span> | <span data-ttu-id="05a3c-148">div 的位置、大小、字体和颜色属性：</span><span class="sxs-lookup"><span data-stu-id="05a3c-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="05a3c-149">**位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**（会为 div 自动配置高度）</span><span class="sxs-lookup"><span data-stu-id="05a3c-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="05a3c-150">用于创建[绝对定位](onenote-abs-pos.md) div（仅在正文设置 `data-absolute-enabled="true"` 且 div 是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="05a3c-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="05a3c-151">示例：`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="05a3c-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="05a3c-p108">元素的 CSS [样式](#styles)属性。在输出 HTML 中，这些值在适当的子元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="05a3c-154">Microsoft Graph 中的 OneNote API 至少在一个 div 中包装所有正文内容。</span><span class="sxs-lookup"><span data-stu-id="05a3c-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="05a3c-155">在以下情况下，API 创建一个默认 div（使用 `data-id="_default"` 设定属性）以包含正文内容：</span><span class="sxs-lookup"><span data-stu-id="05a3c-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="05a3c-156">输入 body 元素的 **data-absolute-enabled** 属性被省略或被设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="05a3c-157">在此情况下，所有正文内容都被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="05a3c-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="05a3c-158">输入 body 元素的 **data-absolute-enabled** 属性为 **true**，但输入 HTML 包含的直接子级不是[绝对定位](onenote-abs-pos.md)&nbsp; **div**、**img** 或 **object** 元素。</span><span class="sxs-lookup"><span data-stu-id="05a3c-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="05a3c-159">在此情况下，不是[绝对定位](onenote-abs-pos.md)&nbsp; **div**、**img** 或 **object** 元素的直接子级被设置为默认的 div。</span><span class="sxs-lookup"><span data-stu-id="05a3c-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="05a3c-160">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-160">Output attributes</span></span>

|<span data-ttu-id="05a3c-161">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-161">Output attribute</span></span>|<span data-ttu-id="05a3c-162">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-163">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-163">data-id</span></span> | <span data-ttu-id="05a3c-164">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-165">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-166">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-166">id</span></span> | <span data-ttu-id="05a3c-167">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-168">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-169">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-170">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-170">style</span></span> | <span data-ttu-id="05a3c-171">div 的位置和大小属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="05a3c-172">非贡献 div</span><span class="sxs-lookup"><span data-stu-id="05a3c-172">Non-contributing divs</span></span>

<span data-ttu-id="05a3c-173">当输入 HTML 中的 **div** 元素不对页面结构做出贡献或带有 OneNote 所使用的信息时，此 API 将 div 的内容移动到父 div 或默认 div。</span><span class="sxs-lookup"><span data-stu-id="05a3c-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="05a3c-174">下面的示例对此进行了说明。</span><span class="sxs-lookup"><span data-stu-id="05a3c-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="05a3c-175">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="05a3c-175">Input HTML</span></span>

<span data-ttu-id="05a3c-176">包含非贡献嵌套 div。</span><span class="sxs-lookup"><span data-stu-id="05a3c-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="05a3c-177">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="05a3c-177">Output HTML</span></span>

> <span data-ttu-id="05a3c-178">**注意**：div 的内容已被移至父 div 且嵌套的 `<div>` 标记已被删除。</span><span class="sxs-lookup"><span data-stu-id="05a3c-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="05a3c-179">如果 div 定义了任何语义信息，例如 **data-id**（示例：`<div data-id="keep-me">`），则保留该 div。</span><span class="sxs-lookup"><span data-stu-id="05a3c-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="05a3c-180">img 元素</span><span class="sxs-lookup"><span data-stu-id="05a3c-180">img elements</span></span>

<span data-ttu-id="05a3c-181">OneNote 页上的图像由 **img** 元素表示。</span><span class="sxs-lookup"><span data-stu-id="05a3c-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="05a3c-182">**img** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-183">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-183">Input attributes</span></span>

|<span data-ttu-id="05a3c-184">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-184">Input attribute</span></span>|<span data-ttu-id="05a3c-185">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-186">alt</span><span class="sxs-lookup"><span data-stu-id="05a3c-186">alt</span></span> | <span data-ttu-id="05a3c-187">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="05a3c-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="05a3c-188">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-188">data-id</span></span> | <span data-ttu-id="05a3c-189">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-190">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-191">data-render-src</span></span> |<span data-ttu-id="05a3c-192">需要 **data-render-src** 或 **src**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="05a3c-193">在 OneNote 页上显示为位图图像的网页：</span><span class="sxs-lookup"><span data-stu-id="05a3c-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="05a3c-194">- `data-render-src="https://..."` 表示公共 URL。</span><span class="sxs-lookup"><span data-stu-id="05a3c-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="05a3c-195">- `data-render-src="name:BlockName"` 表示[多部分请求](/graph/api/section-post-pages?view=graph-rest-1.0#example)的“演示文稿”块中的图像部分。</span><span class="sxs-lookup"><span data-stu-id="05a3c-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="05a3c-196">如果网页比 OneNote 页能够忠实呈现的内容更为复杂，或者页面需要登录凭据，则此方法很有用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="05a3c-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-197">data-tag</span></span> | <span data-ttu-id="05a3c-198">元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="05a3c-199">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-199">style</span></span> |<span data-ttu-id="05a3c-200">图像的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**、**宽度**和**高度**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="05a3c-201">可在任何图像上设置大小。</span><span class="sxs-lookup"><span data-stu-id="05a3c-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="05a3c-202">位置属性用于创建[绝对定位](onenote-abs-pos.md)图像（仅在正文设置 `data-absolute-enabled="true"` 且图像是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="05a3c-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="05a3c-203">示例：`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="05a3c-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="05a3c-204">在输出 HTML 中，图像大小分别以 **width** 和 **height** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="05a3c-205">src</span><span class="sxs-lookup"><span data-stu-id="05a3c-205">src</span></span> |<span data-ttu-id="05a3c-206">需要 **src** 或 **data-render-src**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="05a3c-207">要在 OneNote 页上呈现的图像：</span><span class="sxs-lookup"><span data-stu-id="05a3c-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="05a3c-208">- `src="https://..."` 表示 Internet 上公开可用图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="05a3c-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="05a3c-209">- `src="name:BlockName"` 表示代表此图像的多部分请求中的已命名部分。</span><span class="sxs-lookup"><span data-stu-id="05a3c-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="05a3c-210">width，height</span><span class="sxs-lookup"><span data-stu-id="05a3c-210">width, height</span></span> | <span data-ttu-id="05a3c-211">图像的宽度或高度，以不带 px 的像素为单位。</span><span class="sxs-lookup"><span data-stu-id="05a3c-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="05a3c-212">示例：`width="400"`</span><span class="sxs-lookup"><span data-stu-id="05a3c-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="05a3c-213">**注意：** OneNote API 自动检测输入图像类型，并在输出 HTML 中将其返回为 **data-fullres-src-type**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="05a3c-214">此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="05a3c-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-215">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-215">Output attributes</span></span>

|<span data-ttu-id="05a3c-216">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-216">Output attribute</span></span>|<span data-ttu-id="05a3c-217">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-218">alt</span><span class="sxs-lookup"><span data-stu-id="05a3c-218">alt</span></span> | <span data-ttu-id="05a3c-219">为此图像提供的替换文字。</span><span class="sxs-lookup"><span data-stu-id="05a3c-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="05a3c-220">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-220">data-id</span></span> | <span data-ttu-id="05a3c-221">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-222">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-223">data-index</span><span class="sxs-lookup"><span data-stu-id="05a3c-223">data-index</span></span> | <span data-ttu-id="05a3c-p118">此图像的位置。用于支持[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="05a3c-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-226">data-fullres-src</span></span> | <span data-ttu-id="05a3c-227">最初嵌入在页面中的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="05a3c-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="05a3c-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="05a3c-228">data-fullres-src-type</span></span> | <span data-ttu-id="05a3c-229">**data-fullres-src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="05a3c-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="05a3c-230">data-options</span><span class="sxs-lookup"><span data-stu-id="05a3c-230">data-options</span></span> | <span data-ttu-id="05a3c-p119">源类型：PDF 文件的源类型为 **printout**，而所有其他文件的源类型为 **splitimage**。仅适用于使用 **data-render-src** 属性创建的[拆分图像](#split-images)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p119">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="05a3c-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-233">data-render-original-src</span></span> | <span data-ttu-id="05a3c-234">此图像的原始源 URL，前提是该源图像来自公共 Internet，且使用 **data-render-src** 属性创建。</span><span class="sxs-lookup"><span data-stu-id="05a3c-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="05a3c-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="05a3c-235">data-src-type</span></span> | <span data-ttu-id="05a3c-236">**src** 资源的媒体类型，例如：`image/png` 或 `image/jpeg`。</span><span class="sxs-lookup"><span data-stu-id="05a3c-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="05a3c-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-237">data-tag</span></span> | <span data-ttu-id="05a3c-238">元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="05a3c-239">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-239">id</span></span> | <span data-ttu-id="05a3c-240">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-241">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-242">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-243">src</span><span class="sxs-lookup"><span data-stu-id="05a3c-243">src</span></span> | <span data-ttu-id="05a3c-244">已针对 Web 浏览器以及移动设备和平板电脑外形规格进行优化的图像资源版本的终结点。</span><span class="sxs-lookup"><span data-stu-id="05a3c-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="05a3c-245">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-245">style</span></span> | <span data-ttu-id="05a3c-246">此图像的位置属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-246">The position properties of the image.</span></span> |
| <span data-ttu-id="05a3c-247">width、height</span><span class="sxs-lookup"><span data-stu-id="05a3c-247">width, height</span></span> | <span data-ttu-id="05a3c-248">此图像的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="05a3c-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="05a3c-249">图像的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="05a3c-249">Output HTML examples for images</span></span>

<span data-ttu-id="05a3c-250">输出 **img** 元素包含图像文件资源的终结点和图像类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="05a3c-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="05a3c-251">可以发出单独的[图像资源终结点的 GET 请求](/graph/api/resource-get?view=graph-rest-1.0)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="05a3c-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="05a3c-252">以下示例说明 **img** 元素在输出 HTML 中可能包含的信息。</span><span class="sxs-lookup"><span data-stu-id="05a3c-252">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="05a3c-253">带有 Web 安全和高分辨率资源的图像</span><span class="sxs-lookup"><span data-stu-id="05a3c-253">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="05a3c-254">通过使用 *data-render-src* 属性创建的图像</span><span class="sxs-lookup"><span data-stu-id="05a3c-254">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="05a3c-255">拆分图像</span><span class="sxs-lookup"><span data-stu-id="05a3c-255">Split images</span></span>

<span data-ttu-id="05a3c-256">出于性能和呈现的考虑，使用 **data-render-src** 属性（从网页 URL 或已命名的部分）创建的图像可能被拆分为多个组件图像。</span><span class="sxs-lookup"><span data-stu-id="05a3c-256">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="05a3c-257">向所有组件映像分配同一 **data-id** 值。</span><span class="sxs-lookup"><span data-stu-id="05a3c-257">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="05a3c-258">每个组件图像均具有从零开始的数据索引属性，该属性定义原始垂直布局。</span><span class="sxs-lookup"><span data-stu-id="05a3c-258">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="05a3c-259">带有三个组件图像的拆分图像</span><span class="sxs-lookup"><span data-stu-id="05a3c-259">Split image with three component images</span></span>

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

<span data-ttu-id="05a3c-260">用户可以在页面上移动图像，因此返回的索引可能是无序的。</span><span class="sxs-lookup"><span data-stu-id="05a3c-260">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="05a3c-261">排序方法应采用从上到下的 Y 轴排序，如果 Y 轴顺序存在冲突，则从左到右按 X 轴进行排序。</span><span class="sxs-lookup"><span data-stu-id="05a3c-261">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="05a3c-262">iframe 元素</span><span class="sxs-lookup"><span data-stu-id="05a3c-262">iframe elements</span></span>

<span data-ttu-id="05a3c-263">OneNote 页可包含由 **iframe** 元素所表示的嵌入的视频。</span><span class="sxs-lookup"><span data-stu-id="05a3c-263">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="05a3c-264">**注意：** 也可以[使用 **object** 元素附加视频文件](onenote-images-files.md#adding-files)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-264">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-265">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-265">Input attributes</span></span>

|<span data-ttu-id="05a3c-266">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-266">Input attribute</span></span>|<span data-ttu-id="05a3c-267">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-267">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-268">data-original-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-268">data-original-src</span></span> | <span data-ttu-id="05a3c-269">必需。</span><span class="sxs-lookup"><span data-stu-id="05a3c-269">Required.</span></span> <span data-ttu-id="05a3c-270">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="05a3c-270">The URL of the video source.</span></span> <span data-ttu-id="05a3c-271">请参阅[受支持的视频源的列表](onenote-images-files.md#adding-videos)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-271">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="05a3c-272">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="05a3c-272">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="05a3c-273">width，height</span><span class="sxs-lookup"><span data-stu-id="05a3c-273">width, height</span></span> | <span data-ttu-id="05a3c-274">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="05a3c-274">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="05a3c-275">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="05a3c-275">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-276">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-276">Output attributes</span></span>

|<span data-ttu-id="05a3c-277">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-277">Output attribute</span></span>|<span data-ttu-id="05a3c-278">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-278">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-279">data-original-src</span><span class="sxs-lookup"><span data-stu-id="05a3c-279">data-original-src</span></span> | <span data-ttu-id="05a3c-280">视频源的 URL。</span><span class="sxs-lookup"><span data-stu-id="05a3c-280">The URL of the video source.</span></span> |
| <span data-ttu-id="05a3c-281">src</span><span class="sxs-lookup"><span data-stu-id="05a3c-281">src</span></span> | <span data-ttu-id="05a3c-282">在 OneNote 页中嵌入的视频的链接。</span><span class="sxs-lookup"><span data-stu-id="05a3c-282">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="05a3c-283">width，height</span><span class="sxs-lookup"><span data-stu-id="05a3c-283">width, height</span></span> | <span data-ttu-id="05a3c-284">iframe 的宽度或高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="05a3c-284">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="05a3c-285">示例：`width=300`</span><span class="sxs-lookup"><span data-stu-id="05a3c-285">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="05a3c-286">视频的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="05a3c-286">Output HTML example for videos</span></span>

<span data-ttu-id="05a3c-287">输出 **iframe** 元素包含链接到源页面和视频的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="05a3c-287">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="05a3c-288">object 元素</span><span class="sxs-lookup"><span data-stu-id="05a3c-288">object elements</span></span>

<span data-ttu-id="05a3c-289">OneNote 页可包含由 **object** 元素表示的文件附件。</span><span class="sxs-lookup"><span data-stu-id="05a3c-289">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="05a3c-290">**object** 元素可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-290">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="05a3c-291">**注意：** 将文件发送为图像并使用 **data-render-src** 属性时，OneNote API 还可以将此文件的内容呈现为页面中的图像。</span><span class="sxs-lookup"><span data-stu-id="05a3c-291">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="05a3c-292">示例：`<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="05a3c-292">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-293">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-293">Input attributes</span></span>

|<span data-ttu-id="05a3c-294">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-294">Input attribute</span></span>|<span data-ttu-id="05a3c-295">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-295">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-296">data</span><span class="sxs-lookup"><span data-stu-id="05a3c-296">data</span></span> | <span data-ttu-id="05a3c-297">必需。</span><span class="sxs-lookup"><span data-stu-id="05a3c-297">Required.</span></span> <span data-ttu-id="05a3c-298">表示[多部分请求](/graph/api/section-post-pages?view=graph-rest-1.0#example)中文件的部分的名称。</span><span class="sxs-lookup"><span data-stu-id="05a3c-298">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="05a3c-299">data-attachment</span><span class="sxs-lookup"><span data-stu-id="05a3c-299">data-attachment</span></span> | <span data-ttu-id="05a3c-p129">必需。文件名。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p129">Required. The file name.</span></span> |
| <span data-ttu-id="05a3c-302">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-302">data-id</span></span> | <span data-ttu-id="05a3c-303">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-303">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-304">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-304">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-305">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-305">style</span></span> | <span data-ttu-id="05a3c-306">对象的位置和大小属性：**位置**（仅限**绝对**）、**左侧**、**顶部**和**宽度**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-306">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="05a3c-307">用于创建[绝对定位](onenote-abs-pos.md)对象（仅在正文设置 `data-absolute-enabled="true"` 且对象是正文的直接子级时）。</span><span class="sxs-lookup"><span data-stu-id="05a3c-307">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="05a3c-308">示例：`<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="05a3c-308">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="05a3c-309">type</span><span class="sxs-lookup"><span data-stu-id="05a3c-309">type</span></span> | <span data-ttu-id="05a3c-310">必需。</span><span class="sxs-lookup"><span data-stu-id="05a3c-310">Required.</span></span><br/><br/><span data-ttu-id="05a3c-311">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="05a3c-311">The standard media file type.</span></span> <span data-ttu-id="05a3c-312">已知文件类型显示与 OneNote 页上的文件类型相关联的图标。</span><span class="sxs-lookup"><span data-stu-id="05a3c-312">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="05a3c-313">已知文件类型显示通用文件图标。</span><span class="sxs-lookup"><span data-stu-id="05a3c-313">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-314">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-314">Output attributes</span></span>

|<span data-ttu-id="05a3c-315">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-315">Output attribute</span></span>|<span data-ttu-id="05a3c-316">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-316">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-317">data</span><span class="sxs-lookup"><span data-stu-id="05a3c-317">data</span></span> | <span data-ttu-id="05a3c-318">文件资源的终结点。</span><span class="sxs-lookup"><span data-stu-id="05a3c-318">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="05a3c-319">data-attachment</span><span class="sxs-lookup"><span data-stu-id="05a3c-319">data-attachment</span></span> | <span data-ttu-id="05a3c-320">文件名。</span><span class="sxs-lookup"><span data-stu-id="05a3c-320">The file name.</span></span> |
| <span data-ttu-id="05a3c-321">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-321">data-id</span></span> | <span data-ttu-id="05a3c-322">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-322">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-323">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-323">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-324">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-324">id</span></span> | <span data-ttu-id="05a3c-325">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-325">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-326">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-326">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-327">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-328">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-328">style</span></span> | <span data-ttu-id="05a3c-329">此对象的位置属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-329">The position properties of the object.</span></span> |
| <span data-ttu-id="05a3c-330">type</span><span class="sxs-lookup"><span data-stu-id="05a3c-330">type</span></span> | <span data-ttu-id="05a3c-331">标准媒体文件类型。</span><span class="sxs-lookup"><span data-stu-id="05a3c-331">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="05a3c-332">对象的输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="05a3c-332">Output HTML example for objects</span></span>

<span data-ttu-id="05a3c-333">输出 **object** 元素包含链接到页面中的文件资源的终结点，如下所示。</span><span class="sxs-lookup"><span data-stu-id="05a3c-333">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="05a3c-334">可以发出单独的[文件资源终结点的 GET 请求](/graph/api/resource-get?view=graph-rest-1.0)，以检索其二进制内容。</span><span class="sxs-lookup"><span data-stu-id="05a3c-334">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="05a3c-335">段落和标题</span><span class="sxs-lookup"><span data-stu-id="05a3c-335">Paragraphs and headings</span></span>

<span data-ttu-id="05a3c-336">段落、标题和其他文本容器可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-336">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-337">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-337">Input attributes</span></span>

|<span data-ttu-id="05a3c-338">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-338">Input attribute</span></span>|<span data-ttu-id="05a3c-339">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-339">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-340">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-340">data-id</span></span> | <span data-ttu-id="05a3c-341">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-341">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-342">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-342">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-343">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-343">data-tag</span></span> | <span data-ttu-id="05a3c-344">**p** 或 **h1** - **h6** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-344">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="05a3c-345">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-345">style</span></span> | <span data-ttu-id="05a3c-346">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-346">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-347">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-347">Output attributes</span></span>

|<span data-ttu-id="05a3c-348">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-348">Output attribute</span></span>|<span data-ttu-id="05a3c-349">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-349">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-350">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-350">data-id</span></span> | <span data-ttu-id="05a3c-351">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-351">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-352">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-352">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-353">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-353">data-tag</span></span> | <span data-ttu-id="05a3c-354">**p** 或 **h1** - **h6** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-354">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="05a3c-355">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-355">id</span></span> | <span data-ttu-id="05a3c-356">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-356">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-357">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-357">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-358">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-358">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-359">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-359">style</span></span> | <span data-ttu-id="05a3c-360">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-360">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="05a3c-361">在输出 HTML 中，可能在相应的子元素或 **span** 元素上内嵌返回这些值。</span><span class="sxs-lookup"><span data-stu-id="05a3c-361">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="05a3c-362">以下示例显示使用不同方法定义文本容器样式的输入 HTML 和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-362">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="05a3c-363">在 span 元素的起始标记中使用内联字符样式定义样式的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-363">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="05a3c-364">带有 `<i>` 字符样式以及 `<p>` 起始标记中的字体设置的输出 HTML 作为 span 元素上的内联 CSS 样式返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-364">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="05a3c-365">列表</span><span class="sxs-lookup"><span data-stu-id="05a3c-365">Lists</span></span>

<span data-ttu-id="05a3c-366">列表表示为包含由 **li** 元素所表示的列表项的 **ol** 或 **ul** 元素。</span><span class="sxs-lookup"><span data-stu-id="05a3c-366">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="05a3c-367">列表和列表项可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-367">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-368">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-368">Input attributes</span></span>

|<span data-ttu-id="05a3c-369">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-369">Input attribute</span></span>|<span data-ttu-id="05a3c-370">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-370">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-371">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-371">data-id</span></span> | <span data-ttu-id="05a3c-372">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-372">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-373">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-373">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-374">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-374">data-tag</span></span> | <span data-ttu-id="05a3c-375">**ul**、**ol** 或 **li** 元素上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-375">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="05a3c-376">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-376">style</span></span> | <span data-ttu-id="05a3c-377">列表或列表项的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-377">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-378">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-378">Output attributes</span></span>

|<span data-ttu-id="05a3c-379">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-379">Output attribute</span></span>|<span data-ttu-id="05a3c-380">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-380">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-381">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-381">data-id</span></span> | <span data-ttu-id="05a3c-382">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-382">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-383">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-383">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-384">data-tag</span><span class="sxs-lookup"><span data-stu-id="05a3c-384">data-tag</span></span> |  <span data-ttu-id="05a3c-385">**li** 元素中的 span 上的[笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-385">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="05a3c-386">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-386">id</span></span> | <span data-ttu-id="05a3c-387">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-387">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-388">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-388">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-389">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-389">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-390">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-390">style</span></span> | <span data-ttu-id="05a3c-391">元素的 **list-style-type** 和 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-391">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="05a3c-392">在输出 HTML 中，在列表项上返回列表级别设置。</span><span class="sxs-lookup"><span data-stu-id="05a3c-392">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="05a3c-393">不会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-393">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="05a3c-394">列表样式</span><span class="sxs-lookup"><span data-stu-id="05a3c-394">List styles</span></span>

<span data-ttu-id="05a3c-395">Microsoft Graph 中的 OneNote API 支持以下列表样式：</span><span class="sxs-lookup"><span data-stu-id="05a3c-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="05a3c-396">已排序列表</span><span class="sxs-lookup"><span data-stu-id="05a3c-396">Ordered list</span></span>|<span data-ttu-id="05a3c-397">未排序列表</span><span class="sxs-lookup"><span data-stu-id="05a3c-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-398">无</span><span class="sxs-lookup"><span data-stu-id="05a3c-398">none</span></span> | <span data-ttu-id="05a3c-399">无</span><span class="sxs-lookup"><span data-stu-id="05a3c-399">none</span></span> |
| <span data-ttu-id="05a3c-400">decimal (default)</span><span class="sxs-lookup"><span data-stu-id="05a3c-400">decimal (default)</span></span> | <span data-ttu-id="05a3c-401">disc (default)</span><span class="sxs-lookup"><span data-stu-id="05a3c-401">disc (default)</span></span> |
| <span data-ttu-id="05a3c-402">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="05a3c-402">lower-alpha</span></span> | <span data-ttu-id="05a3c-403">circle</span><span class="sxs-lookup"><span data-stu-id="05a3c-403">circle</span></span> |
| <span data-ttu-id="05a3c-404">lower-roman</span><span class="sxs-lookup"><span data-stu-id="05a3c-404">lower-roman</span></span> | <span data-ttu-id="05a3c-405">square</span><span class="sxs-lookup"><span data-stu-id="05a3c-405">square</span></span> |
| <span data-ttu-id="05a3c-406">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="05a3c-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="05a3c-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="05a3c-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="05a3c-408">您可以在输入 HTML 中对 **ol** 或 **ul** 元素上的列表应用全局样式，但样式在 **li** 元素上返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="05a3c-409">同源列表样式</span><span class="sxs-lookup"><span data-stu-id="05a3c-409">Homogenous list style</span></span>

<span data-ttu-id="05a3c-410">本示例显示了在 **ol** 元素上设置列表样式类型以及在单独列表项上设置 CSS 样式的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="05a3c-p137">这是输出 HTML。请注意，这些样式在单独 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p137">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="05a3c-413">变量列表样式</span><span class="sxs-lookup"><span data-stu-id="05a3c-413">Variable list styles</span></span>

<span data-ttu-id="05a3c-414">本示例显示了在 **li** 元素上设置不同列表样式类型的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="05a3c-p138">这是输出 HTML。请注意，这些样式在单独 **li** 或 **span** 元素上内嵌返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="05a3c-417">表</span><span class="sxs-lookup"><span data-stu-id="05a3c-417">Tables</span></span>

<span data-ttu-id="05a3c-p139">这些表表示为可以包含 **tr** 和 **td** 元素的 **table** 元素。支持嵌套表。</span><span class="sxs-lookup"><span data-stu-id="05a3c-p139">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="05a3c-420">表可以在输入和输出 HTML 中包含下列属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="05a3c-421">OneNote API 不支持 **rowspan** 或 **colspan** 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="05a3c-422">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-422">Input attributes</span></span>

|<span data-ttu-id="05a3c-423">输入属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-423">Input attribute</span></span>|<span data-ttu-id="05a3c-424">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-425">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-425">data-id</span></span> | <span data-ttu-id="05a3c-426">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-426">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-427">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-427">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-428">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-428">style</span></span> | <span data-ttu-id="05a3c-429">此元素的 CSS [style](#styles) 属性，以及：</span><span class="sxs-lookup"><span data-stu-id="05a3c-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="05a3c-430">- **width**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-430">- **width**.</span></span> <span data-ttu-id="05a3c-431">受 **table** 和 **td** 支持作为页面宽度的像素或百分比。</span><span class="sxs-lookup"><span data-stu-id="05a3c-431">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="05a3c-432">示例：`width="100px"` 或 `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="05a3c-432">Example: `width="100px"` or `width="60%"`</span></span> |
| <span data-ttu-id="05a3c-433">边框</span><span class="sxs-lookup"><span data-stu-id="05a3c-433">border</span></span> | <span data-ttu-id="05a3c-434">添加边框至指定宽度的表格</span><span class="sxs-lookup"><span data-stu-id="05a3c-434">Adds border to table with specified width</span></span> |
| <span data-ttu-id="05a3c-435">宽度</span><span class="sxs-lookup"><span data-stu-id="05a3c-435">width</span></span> | <span data-ttu-id="05a3c-436">表格宽度</span><span class="sxs-lookup"><span data-stu-id="05a3c-436">Width of the table</span></span> |
| <span data-ttu-id="05a3c-437">bgcolor</span><span class="sxs-lookup"><span data-stu-id="05a3c-437">bgcolor</span></span> | <span data-ttu-id="05a3c-438">表格背景色</span><span class="sxs-lookup"><span data-stu-id="05a3c-438">The background color of the table</span></span> |

<span data-ttu-id="05a3c-439">**注意：** 在输入 html 中不支持使用表格样式属性中“**边框**”属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-439">**Note:** The use of the **border** property in the style attribute of a table is not supported in input html.</span></span> 
 

#### <a name="output-attributes"></a><span data-ttu-id="05a3c-440">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-440">Output attributes</span></span>

|<span data-ttu-id="05a3c-441">输出属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-441">Output attribute</span></span>|<span data-ttu-id="05a3c-442">说明</span><span class="sxs-lookup"><span data-stu-id="05a3c-442">Description</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-443">data-id</span><span class="sxs-lookup"><span data-stu-id="05a3c-443">data-id</span></span> | <span data-ttu-id="05a3c-444">元素的引用。</span><span class="sxs-lookup"><span data-stu-id="05a3c-444">A reference for the element.</span></span><br/><br/><span data-ttu-id="05a3c-445">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-445">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-446">id</span><span class="sxs-lookup"><span data-stu-id="05a3c-446">id</span></span> | <span data-ttu-id="05a3c-447">元素的唯一生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="05a3c-447">A unique, generated ID for the element.</span></span> <span data-ttu-id="05a3c-448">使用 `includeIDs=true` 查询选项时，由[对页面的 *content* 终结点的 GET 请求](/graph/api/page-get?view=graph-rest-1.0)返回。</span><span class="sxs-lookup"><span data-stu-id="05a3c-448">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="05a3c-449">用于[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="05a3c-449">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="05a3c-450">style</span><span class="sxs-lookup"><span data-stu-id="05a3c-450">style</span></span> | <span data-ttu-id="05a3c-451">此元素的 CSS [style](#styles) 属性。</span><span class="sxs-lookup"><span data-stu-id="05a3c-451">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="05a3c-452">以下示例显示使用不同方法定义表样式的输入 HTML和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-452">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="05a3c-453">具有不同级别可选设置的输入 HTML</span><span class="sxs-lookup"><span data-stu-id="05a3c-453">Input HTML with optional settings at different levels</span></span>

```html
<table border="1"; Width="500"; bgcolor = "green">
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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="05a3c-454">具有 CSS 样式的输出 HTML 在 td 元素上内嵌返回</span><span class="sxs-lookup"><span data-stu-id="05a3c-454">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="05a3c-455">样式</span><span class="sxs-lookup"><span data-stu-id="05a3c-455">Styles</span></span>

<span data-ttu-id="05a3c-456">Microsoft Graph 中的 OneNote API 支持页面正文中元素的以下内联 CSS **style** 属性，如 **body**、**div**、**p**、**li** 和 **span**。</span><span class="sxs-lookup"><span data-stu-id="05a3c-456">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="05a3c-457">属性</span><span class="sxs-lookup"><span data-stu-id="05a3c-457">Property</span></span>|<span data-ttu-id="05a3c-458">示例</span><span class="sxs-lookup"><span data-stu-id="05a3c-458">Example</span></span>|
|:------|:------|
| <span data-ttu-id="05a3c-459">background-color</span><span class="sxs-lookup"><span data-stu-id="05a3c-459">background-color</span></span> | <span data-ttu-id="05a3c-460">`style="background-color:#66cc66"`（默认为白色）</span><span class="sxs-lookup"><span data-stu-id="05a3c-460">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="05a3c-461">支持十六进制格式和命名颜色。</span><span class="sxs-lookup"><span data-stu-id="05a3c-461">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="05a3c-462">color</span><span class="sxs-lookup"><span data-stu-id="05a3c-462">color</span></span> | <span data-ttu-id="05a3c-463">`style="color:#ffffff"`（默认为黑色）</span><span class="sxs-lookup"><span data-stu-id="05a3c-463">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="05a3c-464">font-family</span><span class="sxs-lookup"><span data-stu-id="05a3c-464">font-family</span></span> | <span data-ttu-id="05a3c-465">`style="font-family:Courier"`（默认为 Calibri）</span><span class="sxs-lookup"><span data-stu-id="05a3c-465">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="05a3c-466">font-size</span><span class="sxs-lookup"><span data-stu-id="05a3c-466">font-size</span></span> | <span data-ttu-id="05a3c-467">`style="font-size:10pt"`（默认为 11pt）</span><span class="sxs-lookup"><span data-stu-id="05a3c-467">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="05a3c-468">API 接受 *pt* 或 *px* 的字体大小，但会将 *px* 转换为 *pt*。</span><span class="sxs-lookup"><span data-stu-id="05a3c-468">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="05a3c-469">十进制值被四舍五入为最接近的 n.0pt 或 n.5pt。</span><span class="sxs-lookup"><span data-stu-id="05a3c-469">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="05a3c-470">font-style</span><span class="sxs-lookup"><span data-stu-id="05a3c-470">font-style</span></span> | <span data-ttu-id="05a3c-471">`style="font-style:italic"`（正常或仅倾斜）</span><span class="sxs-lookup"><span data-stu-id="05a3c-471">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="05a3c-472">font-weight</span><span class="sxs-lookup"><span data-stu-id="05a3c-472">font-weight</span></span> | <span data-ttu-id="05a3c-473">`style="font-weight:bold"`（正常或仅加粗）</span><span class="sxs-lookup"><span data-stu-id="05a3c-473">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="05a3c-474">strike-through</span><span class="sxs-lookup"><span data-stu-id="05a3c-474">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="05a3c-475">text-align</span><span class="sxs-lookup"><span data-stu-id="05a3c-475">text-align</span></span> | <span data-ttu-id="05a3c-476">`style="text-align:center"`（仅适用于块元素）</span><span class="sxs-lookup"><span data-stu-id="05a3c-476">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="05a3c-477">text-decoration</span><span class="sxs-lookup"><span data-stu-id="05a3c-477">text-decoration</span></span> | <span data-ttu-id="05a3c-478">`style="text-decoration:underline"`（无或仅加下划线）</span><span class="sxs-lookup"><span data-stu-id="05a3c-478">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="05a3c-479">另外，还支持下列内联字符样式：</span><span class="sxs-lookup"><span data-stu-id="05a3c-479">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="05a3c-480"><b></span><span class="sxs-lookup"><span data-stu-id="05a3c-480"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-481"><i></span><span class="sxs-lookup"><span data-stu-id="05a3c-481"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-482"><u></span><span class="sxs-lookup"><span data-stu-id="05a3c-482"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="05a3c-483"><em></span><span class="sxs-lookup"><span data-stu-id="05a3c-483"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-484"><strong></span><span class="sxs-lookup"><span data-stu-id="05a3c-484"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-485"><strike></span><span class="sxs-lookup"><span data-stu-id="05a3c-485"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="05a3c-486"><sup></span><span class="sxs-lookup"><span data-stu-id="05a3c-486"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-487"><sub></span><span class="sxs-lookup"><span data-stu-id="05a3c-487"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="05a3c-488"><del></span><span class="sxs-lookup"><span data-stu-id="05a3c-488"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="05a3c-489"><cite></span><span class="sxs-lookup"><span data-stu-id="05a3c-489"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="05a3c-490">输入和输出 HTML 示例</span><span class="sxs-lookup"><span data-stu-id="05a3c-490">Input and output HTML example</span></span>

<span data-ttu-id="05a3c-491">下图显示了使用 Microsoft Graph 创建的简单页面。</span><span class="sxs-lookup"><span data-stu-id="05a3c-491">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![包含维基百科中的内容的学习笔记的 OneNote 页的图像](images/onenote-sample-image.png)

<span data-ttu-id="05a3c-493">这是在创建页面的邮件正文中发送的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-493">This is the input HTML sent in the message body to create the page.</span></span>

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

<span data-ttu-id="05a3c-494">这是[获取页面内容](onenote-get-content.md)时 Microsoft Graph 返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="05a3c-494">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="05a3c-495">**注意：**[创建页面](onenote-create-page.md)或[获取页面元数据](/graph/api/page-get?view=graph-rest-1.0)时，API 返回 **contentUrl** 属性中的页面的 *content* 终结点 URL。</span><span class="sxs-lookup"><span data-stu-id="05a3c-495">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="05a3c-496">另请参阅</span><span class="sxs-lookup"><span data-stu-id="05a3c-496">See also</span></span>

- [<span data-ttu-id="05a3c-497">获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="05a3c-497">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="05a3c-498">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="05a3c-498">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="05a3c-499">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="05a3c-499">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="05a3c-500">添加图像、视频和文件</span><span class="sxs-lookup"><span data-stu-id="05a3c-500">Add images, videos, and files</span></span>](onenote-images-files.md)
