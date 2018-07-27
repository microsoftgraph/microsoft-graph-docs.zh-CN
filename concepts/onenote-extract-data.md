# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a><span data-ttu-id="ba29a-101">使用 OneNote API div 标记从捕获中提取数据</span><span class="sxs-lookup"><span data-stu-id="ba29a-101">Use OneNote API div tags to extract data from captures</span></span> 

<span data-ttu-id="ba29a-102">**适用于** OneDrive 上的消费者笔记本 | Office 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="ba29a-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="ba29a-103">使用 OneNote API 从图像中提取名片数据，或从 URL 中提取食谱和产品数据。</span><span class="sxs-lookup"><span data-stu-id="ba29a-103">Use the OneNote API to extract business card data from an image, or recipe and product data from a URL.</span></span>

<a name="attributes"></a>

## <a name="extraction-attributes"></a><span data-ttu-id="ba29a-104">提取属性</span><span class="sxs-lookup"><span data-stu-id="ba29a-104">Extraction attributes</span></span>

<span data-ttu-id="ba29a-105">若要提取和转换数据，只需在 [create-page](onenote-create-page.md) 或 [update-page](onenote_update_page.md) 请求中包含一个指定源内容、提取方法和回退行为的 div。</span><span class="sxs-lookup"><span data-stu-id="ba29a-105">To extract and transform data, simply include a div that specifies the source content, extraction method, and fallback behavior in your [create-page](onenote-create-page.md) or [update-page](onenote_update_page.md) request.</span></span> <span data-ttu-id="ba29a-106">API 以易于阅读的格式在页面上呈现提取的数据。</span><span class="sxs-lookup"><span data-stu-id="ba29a-106">The API renders extracted data on the page in an easy-to-read format.</span></span> 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a><span data-ttu-id="ba29a-107">data-render-src</span><span class="sxs-lookup"><span data-stu-id="ba29a-107">data-render-src</span></span>

<span data-ttu-id="ba29a-108">内容源。</span><span class="sxs-lookup"><span data-stu-id="ba29a-108">The content source.</span></span> <span data-ttu-id="ba29a-109">这可以是名片的图像或来自许多热门食谱或产品网站的绝对 URL。</span><span class="sxs-lookup"><span data-stu-id="ba29a-109">This can be an image of a business card or an absolute URL from many popular recipe or product websites.</span></span> <span data-ttu-id="ba29a-110">必需。</span><span class="sxs-lookup"><span data-stu-id="ba29a-110">Required.</span></span>

<span data-ttu-id="ba29a-111">为在指定 URL 时获得最佳结果，请使用源网页的 HTML 中定义的规范 URL（如果已定义）。</span><span class="sxs-lookup"><span data-stu-id="ba29a-111">For best results when specifying a URL, use the canonical URL defined in the HTML of the source webpage, if one is defined.</span></span> <span data-ttu-id="ba29a-112">例如，规范 URL 可能会在源网页中定义，如下所示：</span><span class="sxs-lookup"><span data-stu-id="ba29a-112">For example, a canonical URL might be defined in the source webpage like this:</span></span>

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a><span data-ttu-id="ba29a-113">data-render-method</span><span class="sxs-lookup"><span data-stu-id="ba29a-113">data-render-method</span></span>

<span data-ttu-id="ba29a-114">要运行的提取方法。</span><span class="sxs-lookup"><span data-stu-id="ba29a-114">The extraction method to run.</span></span> <span data-ttu-id="ba29a-115">必需。</span><span class="sxs-lookup"><span data-stu-id="ba29a-115">Required.</span></span>

| <span data-ttu-id="ba29a-116">值</span><span class="sxs-lookup"><span data-stu-id="ba29a-116">Value</span></span> | <span data-ttu-id="ba29a-117">说明</span><span class="sxs-lookup"><span data-stu-id="ba29a-117">Description</span></span> |
|:------|:------|
| <span data-ttu-id="ba29a-118">extract.businesscard</span><span class="sxs-lookup"><span data-stu-id="ba29a-118">extract.businesscard</span></span> | <span data-ttu-id="ba29a-119">名片提取。</span><span class="sxs-lookup"><span data-stu-id="ba29a-119">A business card extraction.</span></span> |
| <span data-ttu-id="ba29a-120">extract.recipe</span><span class="sxs-lookup"><span data-stu-id="ba29a-120">extract.recipe</span></span> | <span data-ttu-id="ba29a-121">食谱提取。</span><span class="sxs-lookup"><span data-stu-id="ba29a-121">A recipe extraction.</span></span> |
| <span data-ttu-id="ba29a-122">extract.product</span><span class="sxs-lookup"><span data-stu-id="ba29a-122">extract.product</span></span> | <span data-ttu-id="ba29a-123">产品列表提取。</span><span class="sxs-lookup"><span data-stu-id="ba29a-123">A product listing extraction.</span></span> |
| <span data-ttu-id="ba29a-124">提取</span><span class="sxs-lookup"><span data-stu-id="ba29a-124">extract</span></span> | <span data-ttu-id="ba29a-125">未知的提取类型。</span><span class="sxs-lookup"><span data-stu-id="ba29a-125">An unknown extraction type.</span></span> |

<span data-ttu-id="ba29a-126">为获得最佳结果，如果你知道的话，请指定内容类型（`extract.businesscard`、`extract.recipe` 或 `extract.product`）。</span><span class="sxs-lookup"><span data-stu-id="ba29a-126">For best results, specify the content type (`extract.businesscard`, `extract.recipe`, or `extract.product`) if you know it.</span></span> <span data-ttu-id="ba29a-127">如果类型未知，请使用 `extract` 方法，OneNote API 将尝试自动检测类型。</span><span class="sxs-lookup"><span data-stu-id="ba29a-127">If the type is unknown, use the `extract` method and the OneNote API will try to auto-detect the type.</span></span>

### <a name="data-render-fallback"></a><span data-ttu-id="ba29a-128">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="ba29a-128">data-render-fallback</span></span>

<span data-ttu-id="ba29a-129">提取失败时的回退行为。</span><span class="sxs-lookup"><span data-stu-id="ba29a-129">The fallback behavior if the extraction fails.</span></span> <span data-ttu-id="ba29a-130">如果省略，默认值为 **render**。</span><span class="sxs-lookup"><span data-stu-id="ba29a-130">Defaults to **render** if omitted.</span></span> 

| <span data-ttu-id="ba29a-131">值</span><span class="sxs-lookup"><span data-stu-id="ba29a-131">Value</span></span> | <span data-ttu-id="ba29a-132">说明</span><span class="sxs-lookup"><span data-stu-id="ba29a-132">Description</span></span> |
|:------|:------|
| <span data-ttu-id="ba29a-133">呈现</span><span class="sxs-lookup"><span data-stu-id="ba29a-133">render</span></span> | <span data-ttu-id="ba29a-134">呈现源图片或食谱或产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-134">Renders the source image or a snapshot of the recipe or product webpage.</span></span> |
| <span data-ttu-id="ba29a-135">无</span><span class="sxs-lookup"><span data-stu-id="ba29a-135">none</span></span> | <span data-ttu-id="ba29a-136">不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="ba29a-136">Does nothing.</span></span><br /><br /><span data-ttu-id="ba29a-137">如果希望除任何提取内容外，在页面上始终包含名片或网页的快照，此选项非常有用。</span><span class="sxs-lookup"><span data-stu-id="ba29a-137">This option is useful if you want to always include a snapshot of the business card or webpage on the page in addition to any extracted content.</span></span> <span data-ttu-id="ba29a-138">请务必在请求中发送单独的 `img` 元素，如示例中所示。</span><span class="sxs-lookup"><span data-stu-id="ba29a-138">Be sure to send a separate `img` element in the request, as shown in the examples.</span></span> |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a><span data-ttu-id="ba29a-139">名片提取</span><span class="sxs-lookup"><span data-stu-id="ba29a-139">Business card extractions</span></span>

<span data-ttu-id="ba29a-140">OneNote API 尝试基于个人或公司的名片图片，查找和呈现以下联系人信息。</span><span class="sxs-lookup"><span data-stu-id="ba29a-140">The OneNote API tries to find and render the following contact information based on an image of a person's or company's business card.</span></span>

- <span data-ttu-id="ba29a-141">名称</span><span class="sxs-lookup"><span data-stu-id="ba29a-141">Name</span></span>
- <span data-ttu-id="ba29a-142">标题</span><span class="sxs-lookup"><span data-stu-id="ba29a-142">Title</span></span>
- <span data-ttu-id="ba29a-143">组织</span><span class="sxs-lookup"><span data-stu-id="ba29a-143">Organization</span></span>
- <span data-ttu-id="ba29a-144">电话和传真号码</span><span class="sxs-lookup"><span data-stu-id="ba29a-144">Phone and fax numbers</span></span>
- <span data-ttu-id="ba29a-145">邮寄和实际地址</span><span class="sxs-lookup"><span data-stu-id="ba29a-145">Mailing and physical addresses</span></span>
- <span data-ttu-id="ba29a-146">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="ba29a-146">Email addresses</span></span>
- <span data-ttu-id="ba29a-147">网站</span><span class="sxs-lookup"><span data-stu-id="ba29a-147">Websites</span></span>



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

<span data-ttu-id="ba29a-p108">带有提取联系人信息的 vCard（.VCF 文件）也会嵌入到页面中。检索页面 HTML 内容时，vCard 是获取联系人信息的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="ba29a-p108">A vCard (.VCF file) with the extracted contact information is also embedded in the page. The vCard is a convenient way to get the contact information when retrieving page HTML content.</span></span>

### <a name="common-scenarios-for-business-card-extractions"></a><span data-ttu-id="ba29a-150">名片提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="ba29a-150">Common scenarios for business card extractions</span></span>

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a><span data-ttu-id="ba29a-151">提取名片信息，并且呈现名片图像</span><span class="sxs-lookup"><span data-stu-id="ba29a-151">Extract business card information, and also render the business card image</span></span>

<span data-ttu-id="ba29a-152">指定 `extract.businesscard` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-152">Specify the `extract.businesscard` method and the `none` fallback.</span></span> <span data-ttu-id="ba29a-153">此外，发送 `src` 属性同样引用图像的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="ba29a-153">Also send an `img` element with the `src` attribute that also references the image.</span></span> <span data-ttu-id="ba29a-154">如果 API 无法提取任何内容，则只会呈现名片图像。</span><span class="sxs-lookup"><span data-stu-id="ba29a-154">If the API is unable to extract any content, it renders the business card image only.</span></span>

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a><span data-ttu-id="ba29a-155">提取名片信息，并且仅在提取失败时呈现名片图像</span><span class="sxs-lookup"><span data-stu-id="ba29a-155">Extract business card information, and render the business card image only if the extraction fails</span></span>

<span data-ttu-id="ba29a-156">指定 `extract.businesscard` 方法并使用默认的 `render` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-156">Specify the `extract.businesscard` method and use the default `render` fallback.</span></span> <span data-ttu-id="ba29a-157">如果 API 无法提取任何内容，则会改为呈现名片图像。</span><span class="sxs-lookup"><span data-stu-id="ba29a-157">If the API is unable to extract any content, it renders the business card image instead.</span></span>

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
<span data-ttu-id="ba29a-158">对于名片提取，图像作为多部分请求中的指定部件发送。</span><span class="sxs-lookup"><span data-stu-id="ba29a-158">For business card extractions, the image is sent as a named part in a multipart request.</span></span> <span data-ttu-id="ba29a-159">请参阅[添加图像和文件](onenote_images_files.md)，查看有关说明如何在请求中发送图像的示例。</span><span class="sxs-lookup"><span data-stu-id="ba29a-159">See [Add images and files](onenote_images_files.md) for examples that show how to send an image in a request.</span></span>


<a name="recipe"></a>

## <a name="recipe-extractions"></a><span data-ttu-id="ba29a-160">食谱提取</span><span class="sxs-lookup"><span data-stu-id="ba29a-160">Recipe extractions</span></span>

<span data-ttu-id="ba29a-161">OneNote API 尝试基于食谱的 URL 查找和呈现以下信息。</span><span class="sxs-lookup"><span data-stu-id="ba29a-161">The OneNote API tries to find and render the following information based on a recipe's URL.</span></span>

- <span data-ttu-id="ba29a-162">主图</span><span class="sxs-lookup"><span data-stu-id="ba29a-162">Hero image</span></span>
- <span data-ttu-id="ba29a-163">评级</span><span class="sxs-lookup"><span data-stu-id="ba29a-163">Rating</span></span>
- <span data-ttu-id="ba29a-164">食材</span><span class="sxs-lookup"><span data-stu-id="ba29a-164">Ingredients</span></span>
- <span data-ttu-id="ba29a-165">说明</span><span class="sxs-lookup"><span data-stu-id="ba29a-165">Instructions</span></span>
- <span data-ttu-id="ba29a-166">准备时间、烹饪时间和总时间</span><span class="sxs-lookup"><span data-stu-id="ba29a-166">Prep, cook, and total times</span></span>
- <span data-ttu-id="ba29a-167">份数</span><span class="sxs-lookup"><span data-stu-id="ba29a-167">Servings</span></span>


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

<span data-ttu-id="ba29a-168">API 已针对很多热门网站（如 *Allrecipes.com*、*FoodNetwork.com* 和 *SeriousEats.com*）上的食谱进行了优化。</span><span class="sxs-lookup"><span data-stu-id="ba29a-168">The API is optimized for recipes from many popular sites such as *Allrecipes.com*, *FoodNetwork.com*, and *SeriousEats.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="ba29a-169">食谱提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="ba29a-169">Common scenarios for recipe extractions</span></span>

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a><span data-ttu-id="ba29a-170">提取食谱信息，并呈现食谱网页的快照</span><span class="sxs-lookup"><span data-stu-id="ba29a-170">Extract recipe information, and also render a snapshot of the recipe webpage</span></span>

<span data-ttu-id="ba29a-171">指定 `extract.recipe` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-171">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="ba29a-172">此外，发送 `data-render-src` 属性设置为食谱 URL 的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="ba29a-172">Also send an `img` element with the `data-render-src` attribute set to the recipe URL.</span></span> <span data-ttu-id="ba29a-173">如果 API 无法提取任何内容，则只会呈现食谱网页的快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-173">If the API is unable to extract any content, it renders a snapshot of the recipe webpage only.</span></span>

<span data-ttu-id="ba29a-174">本方案提供的信息可能最多，因为网页可能包含客户评论和建议等其他信息。</span><span class="sxs-lookup"><span data-stu-id="ba29a-174">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="http://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="ba29a-175">提取食谱信息，并且仅在提取失败时呈现食谱网页的快照</span><span class="sxs-lookup"><span data-stu-id="ba29a-175">Extract recipe information, and render a snapshot of the recipe webpage only if the extraction fails</span></span>

<span data-ttu-id="ba29a-176">指定 `extract.recipe` 方法，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-176">Specify the `extract.recipe` method and use the default render fallback.</span></span> <span data-ttu-id="ba29a-177">如果 API 无法提取任何内容，则会改为呈现食谱网页的快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-177">If the API is unable to extract any content, it renders a snapshot of the recipe webpage instead.</span></span>

```html  
<div
    data-render-src="http://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a><span data-ttu-id="ba29a-178">提取食谱信息，并呈现指向食谱的链接</span><span class="sxs-lookup"><span data-stu-id="ba29a-178">Extract recipe information, and also render a link to the recipe</span></span>

<span data-ttu-id="ba29a-179">指定 `extract.recipe` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-179">Specify the `extract.recipe` method and the `none` fallback.</span></span> <span data-ttu-id="ba29a-180">此外，发送 `src` 属性设置为食谱 URL 的 `a` 元素（也可以发送要添加到页面的任何其他信息）。</span><span class="sxs-lookup"><span data-stu-id="ba29a-180">Also send an `a` element with the `src` attribute set to the recipe URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="ba29a-181">如果 API 无法提取任何内容，则只会呈现食谱链接。</span><span class="sxs-lookup"><span data-stu-id="ba29a-181">If the API is unable to extract any content, only the recipe link is rendered.</span></span>

```html  
<div
    data-render-src="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="http://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a><span data-ttu-id="ba29a-182">产品列表提取</span><span class="sxs-lookup"><span data-stu-id="ba29a-182">Product listing extractions</span></span>

- <span data-ttu-id="ba29a-183">标题</span><span class="sxs-lookup"><span data-stu-id="ba29a-183">Title</span></span>
- <span data-ttu-id="ba29a-184">评级</span><span class="sxs-lookup"><span data-stu-id="ba29a-184">Rating</span></span>
- <span data-ttu-id="ba29a-185">原始图象</span><span class="sxs-lookup"><span data-stu-id="ba29a-185">Primary image</span></span>
- <span data-ttu-id="ba29a-186">说明</span><span class="sxs-lookup"><span data-stu-id="ba29a-186">Description</span></span>
- <span data-ttu-id="ba29a-187">功能</span><span class="sxs-lookup"><span data-stu-id="ba29a-187">Features</span></span>
- <span data-ttu-id="ba29a-188">规格</span><span class="sxs-lookup"><span data-stu-id="ba29a-188">Specifications</span></span>



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

<span data-ttu-id="ba29a-189">API 已针对很多热门网站（如 *Amazon.com* 和 *HomeDepot.com*）上的产品进行了优化。</span><span class="sxs-lookup"><span data-stu-id="ba29a-189">The API is optimized for products from many popular sites such as *Amazon.com* and *HomeDepot.com*.</span></span>

### <a name="common-scenarios-for-recipe-extractions"></a><span data-ttu-id="ba29a-190">食谱提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="ba29a-190">Common scenarios for recipe extractions</span></span>

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a><span data-ttu-id="ba29a-191">提取产品信息，并呈现产品网页的快照</span><span class="sxs-lookup"><span data-stu-id="ba29a-191">Extract product information, and also render a snapshot of the product webpage</span></span>

<span data-ttu-id="ba29a-192">指定 `extract.product` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-192">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="ba29a-193">此外，发送 `data-render-src` 属性设置为产品 URL 的 `img` 元素。</span><span class="sxs-lookup"><span data-stu-id="ba29a-193">Also send an `img` element with the `data-render-src` attribute set to the product URL.</span></span> <span data-ttu-id="ba29a-194">如果 API 无法提取任何内容，则只会呈现产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-194">If the API is unable to extract any content, it renders a snapshot of the product webpage only.</span></span>

<span data-ttu-id="ba29a-195">本方案提供的信息可能最多，因为网页可能包含客户评论和建议等其他信息。</span><span class="sxs-lookup"><span data-stu-id="ba29a-195">This scenario potentially provides the most information because the webpage may include additional information, such as customer reviews and suggestions.</span></span>

```html 
<div
    data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="http://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a><span data-ttu-id="ba29a-196">提取产品信息，并且仅在提取失败时呈现产品网页的快照</span><span class="sxs-lookup"><span data-stu-id="ba29a-196">Extract product information, and render a snapshot of the product webpage only if the extraction fails</span></span>

<span data-ttu-id="ba29a-197">指定 `extract.product` 方法，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-197">Specify the `extract.product` method and use the default render fallback.</span></span> <span data-ttu-id="ba29a-198">如果 API 无法提取任何内容，则会改为呈现产品网页的快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-198">If the API is unable to extract any content, it renders a snapshot of the product webpage instead.</span></span>

```html 
<div
    data-render-src="http://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a><span data-ttu-id="ba29a-199">提取产品信息，并呈现指向产品的链接</span><span class="sxs-lookup"><span data-stu-id="ba29a-199">Extract product information, and also render a link to the product</span></span>

<span data-ttu-id="ba29a-200">指定 `extract.product` 方法和 `none` 回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-200">Specify the `extract.product` method and the `none` fallback.</span></span> <span data-ttu-id="ba29a-201">此外，发送 `src` 属性设置为产品 URL 的 `a` 元素（也可以发送要添加到页面的任何其他信息）。</span><span class="sxs-lookup"><span data-stu-id="ba29a-201">Also send an `a` element with the `src` attribute set to the product URL (or you can send any other information you want to add to the page).</span></span> <span data-ttu-id="ba29a-202">如果 API 无法提取任何内容，则只会呈现页面链接。</span><span class="sxs-lookup"><span data-stu-id="ba29a-202">If the API is unable to extract any content, only the page link is rendered.</span></span>

```html 
<div
    data-render-src="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="http://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a><span data-ttu-id="ba29a-203">未知内容类型提取</span><span class="sxs-lookup"><span data-stu-id="ba29a-203">Unknown content type extractions</span></span>

<span data-ttu-id="ba29a-204">如果不知道要发送的内容类型（名片、食谱还是产品），可以使用未限定的 `extract` 方法，让 OneNote API 自动检测类型。</span><span class="sxs-lookup"><span data-stu-id="ba29a-204">If you don't know the content type (business card, recipe, or product) that you're sending, you can use the unqualified `extract` method and let the OneNote API automatically detect the type.</span></span> <span data-ttu-id="ba29a-205">如果你的应用发送不同的捕获类型，则你可能需要这样做。</span><span class="sxs-lookup"><span data-stu-id="ba29a-205">You might want to do this if your app sends different capture types.</span></span>

> <span data-ttu-id="ba29a-206">**注意：** 如果确实知道要发送的内容类型，则应使用 `extract.businesscard`、`extract.recipe` 或 `extract.product` 方法。</span><span class="sxs-lookup"><span data-stu-id="ba29a-206">**Note:** If you do know the content type that you're sending, you should use the `extract.businesscard`, `extract.recipe`, or `extract.product` method.</span></span> <span data-ttu-id="ba29a-207">在某些情况下，这将有助于优化提取结果。</span><span class="sxs-lookup"><span data-stu-id="ba29a-207">In some cases, this can help to optimize the extraction results.</span></span>
 
### <a name="common-scenarios-for-unknown-extractions"></a><span data-ttu-id="ba29a-208">未知提取的常见情况</span><span class="sxs-lookup"><span data-stu-id="ba29a-208">Common scenarios for unknown extractions</span></span>

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a><span data-ttu-id="ba29a-209">发送图像或 URL，并在提取失败时呈现提供的网页图像或快照</span><span class="sxs-lookup"><span data-stu-id="ba29a-209">Send an image or a URL, and render the supplied image or a snapshot of the webpage if the extraction fails</span></span>

<span data-ttu-id="ba29a-210">指定 `extract` 方法，以便 API 自动检测内容类型，并使用默认呈现回退。</span><span class="sxs-lookup"><span data-stu-id="ba29a-210">Specify the `extract` method so the API automatically detects the content type, and use the default render fallback.</span></span> <span data-ttu-id="ba29a-211">如果 API 无法提取任何内容，则会改为呈现提供的图像或网页快照。</span><span class="sxs-lookup"><span data-stu-id="ba29a-211">If the API is unable to extract any content, it renders the supplied image or snapshot of the webpage instead.</span></span>

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="ba29a-212">响应信息</span><span class="sxs-lookup"><span data-stu-id="ba29a-212">Response information</span></span>

| <span data-ttu-id="ba29a-213">响应数据</span><span class="sxs-lookup"><span data-stu-id="ba29a-213">Response data</span></span> | <span data-ttu-id="ba29a-214">说明</span><span class="sxs-lookup"><span data-stu-id="ba29a-214">Description</span></span> |  
|------|------|  
| <span data-ttu-id="ba29a-215">成功代码</span><span class="sxs-lookup"><span data-stu-id="ba29a-215">Success code</span></span> | <span data-ttu-id="ba29a-216">成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。</span><span class="sxs-lookup"><span data-stu-id="ba29a-216">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="ba29a-217">错误</span><span class="sxs-lookup"><span data-stu-id="ba29a-217">Errors</span></span>| <span data-ttu-id="ba29a-218">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote_error_codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="ba29a-218">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="ba29a-219">权限</span><span class="sxs-lookup"><span data-stu-id="ba29a-219">Permissions</span></span>

<span data-ttu-id="ba29a-220">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="ba29a-220">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="ba29a-221">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="ba29a-221">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="ba29a-222">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="ba29a-222">Permissions for POST pages</span></span>

- <span data-ttu-id="ba29a-223">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="ba29a-223">Notes.Create</span></span>
- <span data-ttu-id="ba29a-224">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba29a-224">Notes.ReadWrite</span></span>
- <span data-ttu-id="ba29a-225">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba29a-225">Notes.ReadWrite.All</span></span>  

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="ba29a-226">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="ba29a-226">Permissions for PATCH pages</span></span>

- <span data-ttu-id="ba29a-227">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba29a-227">Notes.ReadWrite</span></span>
- <span data-ttu-id="ba29a-228">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba29a-228">Notes.ReadWrite.All</span></span>

<span data-ttu-id="ba29a-229">有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ba29a-229">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="ba29a-230">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ba29a-230">See also</span></span>

- [<span data-ttu-id="ba29a-231">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="ba29a-231">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="ba29a-232">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="ba29a-232">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="ba29a-233">添加图像和文件</span><span class="sxs-lookup"><span data-stu-id="ba29a-233">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="ba29a-234">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="ba29a-234">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="ba29a-235">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="ba29a-235">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="ba29a-236">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="ba29a-236">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="ba29a-237">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="ba29a-237">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

