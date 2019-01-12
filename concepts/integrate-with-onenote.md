---
title: OneNote API 概述
description: OneNote 是一个数字笔记本，可让客户通过在 Web、手机、平板电脑或桌面上键入、草绘或语音来跟踪家庭、学校或工作方面的想法和笔记。 用户可以随意整理笔记、切换设备、接续之前的工作，以及与他人展开实时笔记协作。
author: Jewan-microsoft
localization_priority: Priority
ms.openlocfilehash: a3ca57e9bac52613fbe884368f79b31b5b5165e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825716"
---
# <a name="onenote-api-overview"></a><span data-ttu-id="b2fb0-104">OneNote API 概述</span><span class="sxs-lookup"><span data-stu-id="b2fb0-104">OneNote API overview</span></span>

<span data-ttu-id="b2fb0-105">OneNote 是一个数字笔记本，可让客户通过在 Web、手机、平板电脑或桌面上键入、草绘或语音来跟踪家庭、学校或工作方面的想法和笔记。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-105">OneNote is a digital notebook that lets customers track ideas and notes for home, school, or work, by typing, sketching, or voice, on the web, phone, tablet, or desktop.</span></span> <span data-ttu-id="b2fb0-106">用户可以随意整理笔记、切换设备、接续之前的工作，以及通过与他人实时交互笔记展开协作。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-106">They can freely organize notes, switch devices and pick up where they left off, and collaborate on notes with others in real time.</span></span>

![包含节和页面的 OneNote 笔记本](images/onenote-page.png)

## <a name="why-integrate-with-onenote"></a><span data-ttu-id="b2fb0-108">为什么与 OneNote 集成？</span><span class="sxs-lookup"><span data-stu-id="b2fb0-108">Why integrate with OneNote?</span></span>

<span data-ttu-id="b2fb0-109">通过将应用与 OneNote 集成，可以在服务于全球数百万用户的多个平台中创建强大的体验。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-109">By integrating your apps with OneNote, you can create empowering experiences across multiple platforms that reach millions of users worldwide.</span></span> <span data-ttu-id="b2fb0-110">可以使用 Microsoft Graph 访问 OneNote 中的笔记本、节和页面，从而创建可帮助用户计划和管理想法和信息的解决方案。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-110">You can use Microsoft Graph to access notebooks, sections, and pages in OneNote to create solutions that help your users plan and organize ideas and information.</span></span>

### <a name="collect-and-organize-notes-and-ideas"></a><span data-ttu-id="b2fb0-111">收集并整理笔记和想法</span><span class="sxs-lookup"><span data-stu-id="b2fb0-111">Collect and organize notes and ideas</span></span>  

<span data-ttu-id="b2fb0-112">将 OneNote 用作画布，用户可以在其中添加和排列他们的内容。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-112">Use OneNote as a canvas where users can add and arrange their content.</span></span> <span data-ttu-id="b2fb0-113">借助 Microsoft Graph，可以轻松地编写应用，让学生做笔记并进行研究、让家庭分享计划和想法或让购物者分享图片。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-113">Microsoft Graph makes it easy to write apps that enable students to take notes and do research, families to share plans and ideas, or shoppers to share pictures.</span></span> <span data-ttu-id="b2fb0-114">应用可以捕获用户所需的信息，将其发送到 OneNote，然后帮助用户管理这些信息。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-114">Your app can grab the information people want, send it to OneNote, and then help them organize it.</span></span>

### <a name="capture-information-in-many-formats"></a><span data-ttu-id="b2fb0-115">以多种格式捕获信息</span><span class="sxs-lookup"><span data-stu-id="b2fb0-115">Capture information in many formats</span></span>

<span data-ttu-id="b2fb0-116">捕获 HTML、嵌入的图像（源自本地或公共 URL）、视频、音频、电子邮件和其他常见的文件类型。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-116">Capture HTML, embed images (sourced locally or at a public URL), video, audio, email messages, and other common file types.</span></span> <span data-ttu-id="b2fb0-117">OneNote 甚至还能够以快照的形式呈现网页和 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-117">OneNote can even render webpages and PDF files as snapshots.</span></span> <span data-ttu-id="b2fb0-118">Microsoft Graph 支持 OneNote 页面布局的一组标准 HTML 和 CSS，因此，用户可以使用表、内嵌图像和基本格式以获取所需的外观。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-118">Microsoft Graph supports a set of standard HTML and CSS for OneNote page layout, so you can use tables, inline images, and basic formatting to get the look you want.</span></span> 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a><span data-ttu-id="b2fb0-119">使用 OneNote 生态系统增强核心方案</span><span class="sxs-lookup"><span data-stu-id="b2fb0-119">Use the OneNote ecosystem to enhance your core scenarios</span></span>

<span data-ttu-id="b2fb0-120">了解 OneNote 其他强大的功能。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-120">Tap into other powerful OneNote features.</span></span> <span data-ttu-id="b2fb0-121">Microsoft Graph 中的 OneNote API 在图像上运行 OCR、支持全文搜索、自动同步客户端、处理图像和提取名片捕获、联机产品以及方法列表。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-121">The OneNote APIs in Microsoft Graph run OCR on images, support full-text search, auto-syncs clients, process images, and extract business card captures and online product and recipe listings.</span></span> <span data-ttu-id="b2fb0-122">针对笔记和轻型媒体，在云中将 OneNote 用作数字内存存储，或针对特定于域的数据用作数据馈送。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-122">Use OneNote as your digital memory store in the cloud for notes and lightweight media, or as a data feed for domain-specific data.</span></span> 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a><span data-ttu-id="b2fb0-123">服务于所有主要平台上的数百万 OneNote 用户</span><span class="sxs-lookup"><span data-stu-id="b2fb0-123">Reach millions of OneNote users on all major platforms</span></span>

<span data-ttu-id="b2fb0-124">使用 OneNote 提高应用使用率。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-124">Use OneNote to increase your app usage.</span></span> <span data-ttu-id="b2fb0-125">在新的 Windows 设备上预安装了 OneNote，可作为 Office 365 的一部分联机用于大部分平台。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-125">OneNote is preinstalled on new Windows devices, and is available for most platforms, online, and as part of Office 365.</span></span> <span data-ttu-id="b2fb0-126">发布使用功能丰富的 OneNote 环境的应用时，可以获得广泛的跨平台市场潜力。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-126">When you publish apps that use the feature-rich OneNote environment, you have access to broad cross-platform market potential.</span></span>

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="b2fb0-127">可以通过 Microsoft Graph 中的 OneNote API 实现什么功能？</span><span class="sxs-lookup"><span data-stu-id="b2fb0-127">What can I do with OneNote APIs in Microsoft Graph?</span></span>

<span data-ttu-id="b2fb0-128">以下是使用 OneNote 资源的一些最热门的请求。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-128">The following are some of the most popular requests for working with OneNote resources.</span></span>

|<span data-ttu-id="b2fb0-129">操作</span><span class="sxs-lookup"><span data-stu-id="b2fb0-129">Operation</span></span>|<span data-ttu-id="b2fb0-130">URL</span><span class="sxs-lookup"><span data-stu-id="b2fb0-130">URL</span></span>|
|:--------|:--|
|<span data-ttu-id="b2fb0-131">获取我的笔记本</span><span class="sxs-lookup"><span data-stu-id="b2fb0-131">GET my notebooks</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|<span data-ttu-id="b2fb0-132">获取我的部分</span><span class="sxs-lookup"><span data-stu-id="b2fb0-132">GET my sections</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|<span data-ttu-id="b2fb0-133">获取我的页面</span><span class="sxs-lookup"><span data-stu-id="b2fb0-133">GET my pages</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a><span data-ttu-id="b2fb0-134">详细了解 OneNote API</span><span class="sxs-lookup"><span data-stu-id="b2fb0-134">Learn more about OneNote APIs</span></span>

<span data-ttu-id="b2fb0-135">深入探索 Microsoft Graph API 以了解 OneNote 内容更新功能。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-135">Take an in-depth look at Microsoft Graph APIs to learn about the OneNote content updating capabilities.</span></span> <span data-ttu-id="b2fb0-136">以下列表中的主题说明如何创建新的 OneNote 页并用新内容更新现有页。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-136">The topics in the following list show you how to create new OneNote pages and update existing pages with new content.</span></span> <span data-ttu-id="b2fb0-137">此外，还将了解使用 Microsoft Graph 更新 OneNote 笔记本的最佳做法。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-137">You'll also learn about best practices in using Microsoft Graph to update OneNote notebooks.</span></span> 


### <a name="work-with-onenote"></a><span data-ttu-id="b2fb0-138">使用 OneNote</span><span class="sxs-lookup"><span data-stu-id="b2fb0-138">Work with OneNote</span></span>

* [<span data-ttu-id="b2fb0-139">使用 OneNote REST API</span><span class="sxs-lookup"><span data-stu-id="b2fb0-139">Use the OneNote REST API</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [<span data-ttu-id="b2fb0-140">最佳做法</span><span class="sxs-lookup"><span data-stu-id="b2fb0-140">Best practices</span></span>](onenote-best-practices.md)
* [<span data-ttu-id="b2fb0-141">品牌塑造准则</span><span class="sxs-lookup"><span data-stu-id="b2fb0-141">Branding guidelines</span></span>](onenote-branding.md)
* [<span data-ttu-id="b2fb0-142">打开 OneNote 客户端</span><span class="sxs-lookup"><span data-stu-id="b2fb0-142">Open the OneNote client</span></span>](open-onenote-client.md)
* [<span data-ttu-id="b2fb0-143">在 OneNote 页中使用笔记标记</span><span class="sxs-lookup"><span data-stu-id="b2fb0-143">Use note tags in OneNote pages</span></span>](onenote-note-tags.md)
* [<span data-ttu-id="b2fb0-144">Microsoft Graph 中的 OneNote API 错误代码</span><span class="sxs-lookup"><span data-stu-id="b2fb0-144">Error codes for OneNote APIs in Microsoft Graph</span></span>](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a><span data-ttu-id="b2fb0-145">使用 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="b2fb0-145">Work with OneNote pages</span></span>

* [<span data-ttu-id="b2fb0-146">OneNote 页中的输入和输出 HTML</span><span class="sxs-lookup"><span data-stu-id="b2fb0-146">Input and output HTML in OneNote pages</span></span>](onenote-input-output-html.md)
* [<span data-ttu-id="b2fb0-147">使用 Microsoft Graph 获取 OneNote 内容和结构</span><span class="sxs-lookup"><span data-stu-id="b2fb0-147">Get OneNote content and structure with Microsoft Graph</span></span>](onenote-get-content.md)
* [<span data-ttu-id="b2fb0-148">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="b2fb0-148">Create OneNote pages</span></span>](onenote-create-page.md)
* [<span data-ttu-id="b2fb0-149">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="b2fb0-149">Update OneNote page content</span></span>](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a><span data-ttu-id="b2fb0-150">使用 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="b2fb0-150">Work with OneNote page content</span></span>

* [<span data-ttu-id="b2fb0-151">在 OneNote 页中创建绝对定位的元素</span><span class="sxs-lookup"><span data-stu-id="b2fb0-151">Create absolute positioned elements in OneNote pages</span></span>](onenote-abs-pos.md)
* [<span data-ttu-id="b2fb0-152">将图像、视频和文件添加到 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="b2fb0-152">Add images, videos, and files to OneNote pages</span></span>](onenote-images-files.md)
* [<span data-ttu-id="b2fb0-153">使用 OneNote API div 标记从捕获内容中提取数据</span><span class="sxs-lookup"><span data-stu-id="b2fb0-153">Use OneNote API div tags to extract data from captures</span></span>](onenote-extract-data.md)

## <a name="see-also"></a><span data-ttu-id="b2fb0-154">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b2fb0-154">See also</span></span>
<span data-ttu-id="b2fb0-155">了解仅对 OneNote 服务专用 REST 终结点公开的其他一些 OneNote 功能。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-155">Find out about a few other OneNote features that are exposed only on the OneNote service-specific REST endpoint.</span></span>

- [<span data-ttu-id="b2fb0-156">OneNote 开发</span><span class="sxs-lookup"><span data-stu-id="b2fb0-156">OneNote development</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-landing)
- [<span data-ttu-id="b2fb0-157">处理课堂笔记本</span><span class="sxs-lookup"><span data-stu-id="b2fb0-157">Work with class notebooks</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [<span data-ttu-id="b2fb0-158">使用异步课堂笔记本</span><span class="sxs-lookup"><span data-stu-id="b2fb0-158">Work with asynchronous class notebooks</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [<span data-ttu-id="b2fb0-159">使用教职员工笔记本</span><span class="sxs-lookup"><span data-stu-id="b2fb0-159">Work with staff notebooks</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [<span data-ttu-id="b2fb0-160">复制笔记本、节和页面</span><span class="sxs-lookup"><span data-stu-id="b2fb0-160">Copy notebooks, sections, and pages</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-copy)
- [<span data-ttu-id="b2fb0-161">管理 OneNote 实体的权限</span><span class="sxs-lookup"><span data-stu-id="b2fb0-161">Manage permissions on OneNote entities</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [<span data-ttu-id="b2fb0-162">使用网页上的 OneNote 保存对话框</span><span class="sxs-lookup"><span data-stu-id="b2fb0-162">Use the OneNote save dialog on your webpages</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [<span data-ttu-id="b2fb0-163">订阅 Webhook</span><span class="sxs-lookup"><span data-stu-id="b2fb0-163">Subscribe to webhooks</span></span>](https://docs.microsoft.com/zh-CN/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="api-reference"></a><span data-ttu-id="b2fb0-164">API 参考</span><span class="sxs-lookup"><span data-stu-id="b2fb0-164">API reference</span></span>
<span data-ttu-id="b2fb0-165">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="b2fb0-165">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="b2fb0-166">Microsoft Graph v1.0 中的 OneNote API</span><span class="sxs-lookup"><span data-stu-id="b2fb0-166">OneNote API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="b2fb0-167">Microsoft Graph beta 中的 OneNote API</span><span class="sxs-lookup"><span data-stu-id="b2fb0-167">OneNote API in Microsoft Graph beta</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="b2fb0-168">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b2fb0-168">Next steps</span></span>

<span data-ttu-id="b2fb0-169">使用 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)在你自己的 OneNote 笔记本中试用 OneNote API。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-169">Use the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the OneNote APIs with your own OneNote notebooks.</span></span>

<span data-ttu-id="b2fb0-170">若要在 Graph 浏览器中进行 OneNote API 调用，请选择左侧栏中的“显示更多示例”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-170">To make OneNote API calls from the Graph Explorer, choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="b2fb0-171">使用菜单将 OneNote 切换至“打开”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-171">Use the menu to toggle OneNote **On**.</span></span> <span data-ttu-id="b2fb0-172">还需要启用相应的权限。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-172">You will also need to enable the appropriate permissions.</span></span> <span data-ttu-id="b2fb0-173">在左侧菜单中的帐户名称中，选择“修改权限”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-173">Under your account name in the menu on the left, choose **modify permissions**.</span></span> <span data-ttu-id="b2fb0-174">有关 OneNote 权限的详细信息，请参阅[笔记权限](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-174">For more information about OneNote permissions, see [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

<span data-ttu-id="b2fb0-175">若要开始在 Microsoft Graph 中使用 OneNote API，请参阅 [OneNote 参考内容](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="b2fb0-175">To get started with OneNote APIs in Microsoft Graph, see the [OneNote reference content](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).</span></span>

