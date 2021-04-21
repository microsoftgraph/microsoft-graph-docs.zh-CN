---
title: '使用 OneNote API div 标记从捕获中提取数据 '
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d575ab5609adcc60f4886c726c50ced9bcb10d0b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920185"
---
# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="2a4ae-103">使用 OneNote API div 标记从捕获中提取数据</span><span class="sxs-lookup"><span data-stu-id="2a4ae-103">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="2a4ae-104">**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="2a4ae-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="2a4ae-105">使用 OneNote API 从图像中提取名片数据，或从 URL 中提取食谱和产品数据。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-105">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>

## <a name="extraction-attributes"></a><span data-ttu-id="2a4ae-106">提取属性</span><span class="sxs-lookup"><span data-stu-id="2a4ae-106">Extraction attributes</span></span>

<span data-ttu-id="2a4ae-107">若要提取和转换数据，只需在 [create-page](onenote-create-page.md) 或 [update-page](onenote-update-page.md) 请求中包含一个指定源内容、提取方法和回退行为的 div。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-107">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote-update-page.md) request.</span></span> <span data-ttu-id="2a4ae-108">API 以易于阅读的格式在页面上呈现提取的数据。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-108">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a><span data-ttu-id="2a4ae-109">data-render-src</span><span class="sxs-lookup"><span data-stu-id="2a4ae-109">data-render-src</span></span>

<span data-ttu-id="2a4ae-110">内容源。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-110">The content source.</span></span> <span data-ttu-id="2a4ae-111">这可以是名片的图像或来自许多热门食谱或产品网站的绝对 URL。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-111">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="2a4ae-112">必需。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-112">Required.</span></span>

<span data-ttu-id="2a4ae-113">为在指定 URL 时获得最佳结果，请使用源网页的 HTML 中定义的规范 URL（如果已定义）。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-113">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined.</span></span> <span data-ttu-id="2a4ae-114">例如，规范 URL 可能会在源网页中定义，如下所示：</span><span class="sxs-lookup"><span data-stu-id="2a4ae-114">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a><span data-ttu-id="2a4ae-115">data-render-method</span><span class="sxs-lookup"><span data-stu-id="2a4ae-115">data-render-method</span></span>

<span data-ttu-id="2a4ae-116">要运行的提取方法。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-116">The extraction method to run.</span></span> <span data-ttu-id="2a4ae-117">必需。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-117">Required.</span></span>

| <span data-ttu-id="2a4ae-118">值</span><span class="sxs-lookup"><span data-stu-id="2a4ae-118">Value</span></span> | <span data-ttu-id="2a4ae-119">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ae-119">Description</span></span> |
|:------|:------|
| <span data-ttu-id="2a4ae-120">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="2a4ae-120">extract.businesscard</span></span> | <span data-ttu-id="2a4ae-121">名片提取。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-121">A business card extraction.</span></span> |
| <span data-ttu-id="2a4ae-122">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="2a4ae-122">extract.recipe</span></span> | <span data-ttu-id="2a4ae-123">食谱提取。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-123">A recipe extraction.</span></span> |
| <span data-ttu-id="2a4ae-124">extract.product</span><span class="sxs-lookup"><span data-stu-id="2a4ae-124">extract.product</span></span> | <span data-ttu-id="2a4ae-125">产品列表提取。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-125">A product listing extraction.</span></span> |
| <span data-ttu-id="2a4ae-126">提取</span><span class="sxs-lookup"><span data-stu-id="2a4ae-126">extract</span></span> | <span data-ttu-id="2a4ae-127">未知的提取类型。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-127">An unknown extraction type.</span></span> |

<span data-ttu-id="2a4ae-128">为获得最佳结果，如果你知道的话，请指定内容类型（`extract.businesscard`、`extract.recipe` 或 `extract.product`）。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-128">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="2a4ae-129">如果类型未知，请使用 `extract` 方法，OneNote API 将尝试自动检测类型。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-129">If the type is unknown, use the `extract` method, and the OneNote API will try to auto-detect the type.</span></span>

### <a name="data-render-fallback"></a><span data-ttu-id="2a4ae-130">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="2a4ae-130">data-render-fallback</span></span>

<span data-ttu-id="2a4ae-131">提取失败时的回退行为。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-131">The fallback behavior if the extraction fails.</span></span> <span data-ttu-id="2a4ae-132">如果省略，默认值为 **render**。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-132">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="2a4ae-133">值</span><span class="sxs-lookup"><span data-stu-id="2a4ae-133">Value</span></span> | <span data-ttu-id="2a4ae-134">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ae-134">Description</span></span> |
|:------|:------|
| <span data-ttu-id="2a4ae-135">呈现</span><span class="sxs-lookup"><span data-stu-id="2a4ae-135">render</span></span> | <span data-ttu-id="2a4ae-136">呈现源图片或食谱或产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-136">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="2a4ae-137">无</span><span class="sxs-lookup"><span data-stu-id="2a4ae-137">none</span></span> | <span data-ttu-id="2a4ae-138">不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-138">Does nothing.</span></span><br /><br /><span data-ttu-id="2a4ae-139">如果希望除任何提取内容外，在页面上始终包含名片或网页的快照，此选项非常有用。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-139">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content.</span></span> <span data-ttu-id="2a4ae-140">请务必在请求中发送单独的 `img` 元素，如示例中所示。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-140">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a><span data-ttu-id="2a4ae-141">名片提取</span><span class="sxs-lookup"><span data-stu-id="2a4ae-141">Business card extractions</span></span>

<span data-ttu-id="2a4ae-142">OneNote API 尝试基于个人或公司的名片图片，查找和呈现以下联系人信息。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-142">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>

- <span data-ttu-id="2a4ae-143">名称</span><span class="sxs-lookup"><span data-stu-id="2a4ae-143">Name</span></span>
- <span data-ttu-id="2a4ae-144">标题</span><span class="sxs-lookup"><span data-stu-id="2a4ae-144">Title</span></span>
- <span data-ttu-id="2a4ae-145">组织</span><span class="sxs-lookup"><span data-stu-id="2a4ae-145">Organization</span></span>
- <span data-ttu-id="2a4ae-146">电话和传真号码</span><span class="sxs-lookup"><span data-stu-id="2a4ae-146">Phone and fax numbers</span></span>
- <span data-ttu-id="2a4ae-147">邮寄和实际地址</span><span class="sxs-lookup"><span data-stu-id="2a4ae-147">Mailing and physical addresses</span></span>
- <span data-ttu-id="2a4ae-148">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="2a4ae-148">Email addresses</span></span>
- <span data-ttu-id="2a4ae-149">网站</span><span class="sxs-lookup"><span data-stu-id="2a4ae-149">Websites</span></span>



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

<span data-ttu-id="2a4ae-p108">带有提取联系人信息的 vCard（.VCF 文件）也会嵌入到页面中。检索页面 HTML 内容时，vCard 是获取联系人信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-p108">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="2a4ae-152">名片提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="2a4ae-152">Common scenarios for business card extractions</span></span>

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a><span data-ttu-id="2a4ae-153">提取名片信息，并且呈现名片图像</span><span class="sxs-lookup"><span data-stu-id="2a4ae-153">Extract business card information, and also render the business card image</span></span>

<span data-ttu-id="2a4ae-154">指定 `extract.businesscard` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-154">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="2a4ae-155">此外，发送 `src` 属性同样引用图像的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-155">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="2a4ae-156">如果 API 无法提取任何内容，则只会呈现名片图像。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-156">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a><span data-ttu-id="2a4ae-157">提取名片信息，并且仅在提取失败时呈现名片图像</span><span class="sxs-lookup"><span data-stu-id="2a4ae-157">Extract business card information, and render the business card image only if the extraction fails</span></span>

<span data-ttu-id="2a4ae-158">指定 `extract.businesscard` 方法并使用默认的 `render` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-158">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="2a4ae-159">如果 API 无法提取任何内容，则会改为呈现名片图像。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-159">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="2a4ae-160">对于名片提取，图像作为多部分请求中的指定部件发送。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-160">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="2a4ae-161">请参阅[添加图像和文件](onenote-images-files.md)，查看有关说明如何在请求中发送图像的示例。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-161">See [Add images and files](onenote-images-files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>

## <a name="recipe-extractions"></a><span data-ttu-id="2a4ae-162">食谱提取</span><span class="sxs-lookup"><span data-stu-id="2a4ae-162">Recipe extractions</span></span>

<span data-ttu-id="2a4ae-163">OneNote API 尝试基于食谱的 URL 查找和呈现以下信息。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-163">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="2a4ae-164">主图</span><span class="sxs-lookup"><span data-stu-id="2a4ae-164">Hero image</span></span>
- <span data-ttu-id="2a4ae-165">评级</span><span class="sxs-lookup"><span data-stu-id="2a4ae-165">Rating</span></span>
- <span data-ttu-id="2a4ae-166">食材</span><span class="sxs-lookup"><span data-stu-id="2a4ae-166">Ingredients</span></span>
- <span data-ttu-id="2a4ae-167">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ae-167">Instructions</span></span>
- <span data-ttu-id="2a4ae-168">准备时间、烹饪时间和总时间</span><span class="sxs-lookup"><span data-stu-id="2a4ae-168">Prep, cook, and total times</span></span>
- <span data-ttu-id="2a4ae-169">份数</span><span class="sxs-lookup"><span data-stu-id="2a4ae-169">Servings</span></span>


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

<span data-ttu-id="2a4ae-170">API 已针对很多热门网站（如 *Allrecipes.com*、*FoodNetwork.com* 和 *SeriousEats.com*）上的食谱进行了优化。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-170">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="2a4ae-171">食谱提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="2a4ae-171">Common scenarios for recipe extractions</span></span>

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a><span data-ttu-id="2a4ae-172">提取食谱信息，并呈现食谱网页的快照</span><span class="sxs-lookup"><span data-stu-id="2a4ae-172">Extract recipe information, and also render a snapshot of the recipe webpage</span></span>

<span data-ttu-id="2a4ae-173">指定 `extract.recipe` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-173">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="2a4ae-174">此外，发送 `data-render-src` 属性设置为食谱 URL 的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-174">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="2a4ae-175">如果 API 无法提取任何内容，则只会呈现食谱网页的快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-175">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="2a4ae-176">本方案提供的信息可能最多，因为网页可能包含客户评论和建议等其他信息。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-176">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="https://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="2a4ae-177">提取食谱信息，并且仅在提取失败时呈现食谱网页的快照</span><span class="sxs-lookup"><span data-stu-id="2a4ae-177">Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails</span></span>

<span data-ttu-id="2a4ae-178">指定 `extract.recipe` 方法，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-178">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="2a4ae-179">如果 API 无法提取任何内容，则会改为呈现食谱网页的快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-179">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="https://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a><span data-ttu-id="2a4ae-180">提取食谱信息，并呈现指向食谱的链接</span><span class="sxs-lookup"><span data-stu-id="2a4ae-180">Extract recipe information, and also render a link to the recipe</span></span>

<span data-ttu-id="2a4ae-181">指定 `extract.recipe` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-181">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="2a4ae-182">此外，发送 `src` 属性设置为食谱 URL 的 `a` 元素（也可以发送要添加到页面的任何其他信息）。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-182">Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="2a4ae-183">如果 API 无法提取任何内容，则只会呈现食谱链接。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-183">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a><span data-ttu-id="2a4ae-184">产品列表提取</span><span class="sxs-lookup"><span data-stu-id="2a4ae-184">Product listing extractions</span></span>

- <span data-ttu-id="2a4ae-185">标题</span><span class="sxs-lookup"><span data-stu-id="2a4ae-185">Title</span></span>
- <span data-ttu-id="2a4ae-186">评级</span><span class="sxs-lookup"><span data-stu-id="2a4ae-186">Rating</span></span>
- <span data-ttu-id="2a4ae-187">原始图象</span><span class="sxs-lookup"><span data-stu-id="2a4ae-187">Primary image</span></span>
- <span data-ttu-id="2a4ae-188">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ae-188">Description</span></span>
- <span data-ttu-id="2a4ae-189">功能</span><span class="sxs-lookup"><span data-stu-id="2a4ae-189">Features</span></span>
- <span data-ttu-id="2a4ae-190">规格</span><span class="sxs-lookup"><span data-stu-id="2a4ae-190">Specifications</span></span>



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

<span data-ttu-id="2a4ae-191">API 已针对很多热门网站（如 *Amazon.com* 和 *HomeDepot.com*）上的产品进行了优化。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-191">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="2a4ae-192">食谱提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="2a4ae-192">Common scenarios for recipe extractions</span></span>

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a><span data-ttu-id="2a4ae-193">提取产品信息，并呈现产品网页的快照</span><span class="sxs-lookup"><span data-stu-id="2a4ae-193">Extract product information, and also render a snapshot of the product webpage</span></span>

<span data-ttu-id="2a4ae-194">指定 `extract.product` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-194">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="2a4ae-195">此外，发送 `data-render-src` 属性设置为产品 URL 的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-195">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="2a4ae-196">如果 API 无法提取任何内容，则只会呈现产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-196">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="2a4ae-197">本方案提供的信息可能最多，因为网页可能包含客户评论和建议等其他信息。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-197">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="2a4ae-198">提取产品信息，并且仅在提取失败时呈现产品网页的快照</span><span class="sxs-lookup"><span data-stu-id="2a4ae-198">Extract product information, and render a snapshot of the product webpage only if the extraction fails</span></span>

<span data-ttu-id="2a4ae-199">指定 `extract.product` 方法，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-199">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="2a4ae-200">如果 API 无法提取任何内容，则会改为呈现产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-200">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="https://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a><span data-ttu-id="2a4ae-201">提取产品信息，并呈现指向产品的链接</span><span class="sxs-lookup"><span data-stu-id="2a4ae-201">Extract product information, and also render a link to the product</span></span>

<span data-ttu-id="2a4ae-202">指定 `extract.product` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-202">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="2a4ae-203">此外，发送 `src` 属性设置为产品 URL 的 `a` 元素（也可以发送要添加到页面的任何其他信息）。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-203">Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="2a4ae-204">如果 API 无法提取任何内容，则只会呈现页面链接。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-204">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a><span data-ttu-id="2a4ae-205">未知内容类型提取</span><span class="sxs-lookup"><span data-stu-id="2a4ae-205">Unknown content type extractions</span></span>

<span data-ttu-id="2a4ae-206">如果不知道要发送的内容类型（名片、食谱还是产品），可以使用未限定的 `extract` 方法，让 OneNote API 自动检测类型。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-206">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type.</span></span> <span data-ttu-id="2a4ae-207">如果你的应用发送不同的捕获类型，则你可能需要这样做。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-207">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="2a4ae-208">**注意：** 如果确实知道要发送的内容类型，则应使用 `extract.businesscard`、`extract.recipe` 或 `extract.product` 方法。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-208">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="2a4ae-209">在某些情况下，这将有助于优化提取结果。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-209">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="2a4ae-210">未知提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="2a4ae-210">Common scenarios for unknown extractions</span></span>

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a><span data-ttu-id="2a4ae-211">发送图像或 URL，并在提取失败时呈现提供的网页图像或快照</span><span class="sxs-lookup"><span data-stu-id="2a4ae-211">Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails</span></span>

<span data-ttu-id="2a4ae-212">指定 `extract` 方法，以便 API 自动检测内容类型，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-212">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="2a4ae-213">如果 API 无法提取任何内容，则会改为呈现提供的图像或网页快照。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-213">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="2a4ae-214">响应信息</span><span class="sxs-lookup"><span data-stu-id="2a4ae-214">Response information</span></span>

| <span data-ttu-id="2a4ae-215">响应数据</span><span class="sxs-lookup"><span data-stu-id="2a4ae-215">Response data</span></span> | <span data-ttu-id="2a4ae-216">说明</span><span class="sxs-lookup"><span data-stu-id="2a4ae-216">Description</span></span> |  
|------|------|  
| <span data-ttu-id="2a4ae-217">成功代码</span><span class="sxs-lookup"><span data-stu-id="2a4ae-217">Success code</span></span> | <span data-ttu-id="2a4ae-218">成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-218">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="2a4ae-219">错误</span><span class="sxs-lookup"><span data-stu-id="2a4ae-219">Errors</span></span>| <span data-ttu-id="2a4ae-220">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-220">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="2a4ae-221">权限</span><span class="sxs-lookup"><span data-stu-id="2a4ae-221">Permissions</span></span>

<span data-ttu-id="2a4ae-222">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-222">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="2a4ae-223">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-223">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="2a4ae-224">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="2a4ae-224">Permissions for POST pages</span></span>

- <span data-ttu-id="2a4ae-225">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="2a4ae-225">Notes.Create</span></span>
- <span data-ttu-id="2a4ae-226">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a4ae-226">Notes.ReadWrite</span></span>
- <span data-ttu-id="2a4ae-227">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4ae-227">Notes.ReadWrite.All</span></span>  

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="2a4ae-228">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="2a4ae-228">Permissions for PATCH pages</span></span>

- <span data-ttu-id="2a4ae-229">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a4ae-229">Notes.ReadWrite</span></span>
- <span data-ttu-id="2a4ae-230">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4ae-230">Notes.ReadWrite.All</span></span>

<span data-ttu-id="2a4ae-231">有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2a4ae-231">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="2a4ae-232">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2a4ae-232">See also</span></span>

- [<span data-ttu-id="2a4ae-233">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="2a4ae-233">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="2a4ae-234">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="2a4ae-234">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="2a4ae-235">添加图像和文件</span><span class="sxs-lookup"><span data-stu-id="2a4ae-235">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="2a4ae-236">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="2a4ae-236">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="2a4ae-237">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="2a4ae-237">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="2a4ae-238">Microsoft Q&A 上的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="2a4ae-238">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="2a4ae-239">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="2a4ae-239">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)