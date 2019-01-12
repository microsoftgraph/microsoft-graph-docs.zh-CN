---
title: Microsoft Graph 中的 OneNote API 错误代码
description: 本文介绍当通过 API 发送的请求失败时，Microsoft Graph 中的 OneNote API 返回的错误代码。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f74f9be52756e068aa3e197f2de526b38c187266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987851"
---
# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="de609-103">Microsoft Graph 中的 OneNote API 错误代码</span><span class="sxs-lookup"><span data-stu-id="de609-103">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="de609-104">本文介绍当通过 API 发送的请求失败时，Microsoft Graph 中的 OneNote API 返回的错误代码。</span><span class="sxs-lookup"><span data-stu-id="de609-104">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="de609-105">错误响应示例</span><span class="sxs-lookup"><span data-stu-id="de609-105">Error response example</span></span>

<span data-ttu-id="de609-106">请求生成错误时，OneNote API 将停止执行此请求并将错误响应作为 JSON 对象返回。</span><span class="sxs-lookup"><span data-stu-id="de609-106">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="de609-107">错误响应将包含相关的错误代码、消息和本文相应部分的链接。</span><span class="sxs-lookup"><span data-stu-id="de609-107">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="de609-108">以下示例演示了错误响应的外观。</span><span class="sxs-lookup"><span data-stu-id="de609-108">The following example shows how an error response looks.</span></span>

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

<span data-ttu-id="de609-109">有关 Microsoft Graph 错误的详细信息，请参阅 [Microsoft Graph 错误响应和资源类型](errors.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-109">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="de609-110">从 10001 到 19999 的代码</span><span class="sxs-lookup"><span data-stu-id="de609-110">Codes from 10001 to 19999</span></span>

<span data-ttu-id="de609-111">服务遇到问题，或向应用程序发送信息。</span><span class="sxs-lookup"><span data-stu-id="de609-111">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="de609-112">10001</span><span class="sxs-lookup"><span data-stu-id="de609-112">10001</span></span>
<span data-ttu-id="de609-113">出现意外错误，请求失败。</span><span class="sxs-lookup"><span data-stu-id="de609-113">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="de609-114">10002</span><span class="sxs-lookup"><span data-stu-id="de609-114">10002</span></span>
<span data-ttu-id="de609-115">服务当前不可用。</span><span class="sxs-lookup"><span data-stu-id="de609-115">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="de609-116">10003</span><span class="sxs-lookup"><span data-stu-id="de609-116">10003</span></span>
<span data-ttu-id="de609-117">当前用户的帐户已超过最大活动请求数。</span><span class="sxs-lookup"><span data-stu-id="de609-117">The current user's account has exceeded the maximum number of active requests.</span></span> <span data-ttu-id="de609-118">你的应用将不得不重复请求。</span><span class="sxs-lookup"><span data-stu-id="de609-118">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="de609-119">10004</span><span class="sxs-lookup"><span data-stu-id="de609-119">10004</span></span>
<span data-ttu-id="de609-120">服务无法在请求的部分创建页面，因为该部分受密码保护。</span><span class="sxs-lookup"><span data-stu-id="de609-120">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="de609-121">10005</span><span class="sxs-lookup"><span data-stu-id="de609-121">10005</span></span>
<span data-ttu-id="de609-122">请求包含超过最大数量的图像标记，其中 **data-render-src** 属性包含 PDF。</span><span class="sxs-lookup"><span data-stu-id="de609-122">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF.</span></span> <span data-ttu-id="de609-123">请参阅[添加图像和文件](onenote-images-files.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-123">See [Add images and files](onenote-images-files.md).</span></span>

### <a name="10006"></a><span data-ttu-id="de609-124">10006</span><span class="sxs-lookup"><span data-stu-id="de609-124">10006</span></span>
<span data-ttu-id="de609-125">OneNote API 程序无法在指定部分创建页面，因为该部分已损坏。</span><span class="sxs-lookup"><span data-stu-id="de609-125">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="de609-126">10007</span><span class="sxs-lookup"><span data-stu-id="de609-126">10007</span></span>
<span data-ttu-id="de609-p104">服务器太忙，目前无法处理传入的请求。请稍后重试。</span><span class="sxs-lookup"><span data-stu-id="de609-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="de609-129">10008</span><span class="sxs-lookup"><span data-stu-id="de609-129">10008</span></span>
<span data-ttu-id="de609-130">用户或组的 OneDrive 上的一个或多个文档库包含的 OneNote 项目数（笔记本、分区、分区组）超过 5000 个，无法使用 API 查询。</span><span class="sxs-lookup"><span data-stu-id="de609-130">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="de609-131">请确保用户或组的文档库包含的 OneNote 项目数均未超过 5000 个。</span><span class="sxs-lookup"><span data-stu-id="de609-131">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="de609-132">请参阅 [OneNote 开发博客](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/)获取缓解步骤。</span><span class="sxs-lookup"><span data-stu-id="de609-132">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="de609-133">10012</span><span class="sxs-lookup"><span data-stu-id="de609-133">10012</span></span>
<span data-ttu-id="de609-134">无法创建或更新实体，因为包含笔记本的库要求先将项目签出然后才能编辑这些项。</span><span class="sxs-lookup"><span data-stu-id="de609-134">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="de609-135">有关详细信息，请参阅[设置库以请求签出文件](https://support.office.com/zh-CN/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7)。</span><span class="sxs-lookup"><span data-stu-id="de609-135">For more information, see [Set up a library to require check-out of files](https://support.office.com/zh-CN/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span></span>

<span data-ttu-id="de609-136">可从库中删除签出要求，也可以移动笔记本。</span><span class="sxs-lookup"><span data-stu-id="de609-136">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="de609-137">10013</span><span class="sxs-lookup"><span data-stu-id="de609-137">10013</span></span>
<span data-ttu-id="de609-p107">用户或组 OneDrive 上的一个或多个文档库包含 20,000 多个项目，无法使用 API 通过索引进行查询。请确保没有任何一个用户或组的文档库包含超过 20,000 个项目。有关缓解步骤，请参阅 [OneNote 开发人员博客](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/)。</span><span class="sxs-lookup"><span data-stu-id="de609-p107">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API. Please make sure that none of the user or group's document libraries contains more than 20,000 items. See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="de609-141">10014</span><span class="sxs-lookup"><span data-stu-id="de609-141">10014</span></span>
<span data-ttu-id="de609-142">Azure Key Vault 太忙，目前无法处理传入的请求。</span><span class="sxs-lookup"><span data-stu-id="de609-142">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="de609-143">请稍后重试。</span><span class="sxs-lookup"><span data-stu-id="de609-143">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="de609-144">10015</span><span class="sxs-lookup"><span data-stu-id="de609-144">10015</span></span>
<span data-ttu-id="de609-145">SharePoint 当前不可用。</span><span class="sxs-lookup"><span data-stu-id="de609-145">SharePoint is currently unavailable.</span></span> <span data-ttu-id="de609-146">请稍后重试。</span><span class="sxs-lookup"><span data-stu-id="de609-146">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="de609-147">10016</span><span class="sxs-lookup"><span data-stu-id="de609-147">10016</span></span>
<span data-ttu-id="de609-148">用户或组的 OneDrive 上的文档库超出了唯一的安全作用域阈值限制。</span><span class="sxs-lookup"><span data-stu-id="de609-148">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="de609-149">为库设置的唯一安全作用域的最大数量不能超过 50,000 个。</span><span class="sxs-lookup"><span data-stu-id="de609-149">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="de609-150">10017</span><span class="sxs-lookup"><span data-stu-id="de609-150">10017</span></span>
<span data-ttu-id="de609-151">错误的请求。</span><span class="sxs-lookup"><span data-stu-id="de609-151">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="de609-152">19999</span><span class="sxs-lookup"><span data-stu-id="de609-152">19999</span></span>
<span data-ttu-id="de609-153">请求失败，因为发生无法确定的错误。</span><span class="sxs-lookup"><span data-stu-id="de609-153">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="de609-154">从 20001 到 29999 的代码</span><span class="sxs-lookup"><span data-stu-id="de609-154">Codes from 20001 to 29999</span></span>

<span data-ttu-id="de609-155">应用程序代码已经出现问题。</span><span class="sxs-lookup"><span data-stu-id="de609-155">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="de609-156">20001</span><span class="sxs-lookup"><span data-stu-id="de609-156">20001</span></span>

<span data-ttu-id="de609-157">请求缺少必需的“演示”部分。</span><span class="sxs-lookup"><span data-stu-id="de609-157">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="de609-158">只需要一个。</span><span class="sxs-lookup"><span data-stu-id="de609-158">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="de609-159">20002</span><span class="sxs-lookup"><span data-stu-id="de609-159">20002</span></span>
<span data-ttu-id="de609-160">请求包含两个或更多个“演示”部分。</span><span class="sxs-lookup"><span data-stu-id="de609-160">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="de609-161">只需要一个。</span><span class="sxs-lookup"><span data-stu-id="de609-161">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="de609-162">20003</span><span class="sxs-lookup"><span data-stu-id="de609-162">20003</span></span>
<span data-ttu-id="de609-163">“演示”部分的内容类型只能是文本/HTML 或应用程序/XHTML+XML。</span><span class="sxs-lookup"><span data-stu-id="de609-163">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="de609-164">20004</span><span class="sxs-lookup"><span data-stu-id="de609-164">20004</span></span>
<span data-ttu-id="de609-p113">“演示”部分 HTML 包含一个图像标记，其中包含 **src** 和 **data-render-src** 属性集。API 将忽略 **src** 属性并使用 **data-render-src** 属性。</span><span class="sxs-lookup"><span data-stu-id="de609-p113">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set. The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="de609-167">20005</span><span class="sxs-lookup"><span data-stu-id="de609-167">20005</span></span>
<span data-ttu-id="de609-168">请求 URI 太长。</span><span class="sxs-lookup"><span data-stu-id="de609-168">The request URI is too long.</span></span> <span data-ttu-id="de609-169">URI 的最大大小（包括所有参数和数据）为 16 KB 或 16,384 个字符。</span><span class="sxs-lookup"><span data-stu-id="de609-169">The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="de609-170">20006</span><span class="sxs-lookup"><span data-stu-id="de609-170">20006</span></span>
<span data-ttu-id="de609-171">“演示”部分 HTML 包含未设置 src 和 **data-render-src** 属性的图像标记。</span><span class="sxs-lookup"><span data-stu-id="de609-171">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="de609-172">API 将忽略该**图像**标记。</span><span class="sxs-lookup"><span data-stu-id="de609-172">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="de609-173">20007</span><span class="sxs-lookup"><span data-stu-id="de609-173">20007</span></span>
<span data-ttu-id="de609-174">“演示文稿”部分 HTML 包含与任何允许的格式均不匹配的创建日期/时间字符串。</span><span class="sxs-lookup"><span data-stu-id="de609-174">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="de609-175">20008</span><span class="sxs-lookup"><span data-stu-id="de609-175">20008</span></span>
<span data-ttu-id="de609-176">请求大小太大。</span><span class="sxs-lookup"><span data-stu-id="de609-176">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="de609-177">20009</span><span class="sxs-lookup"><span data-stu-id="de609-177">20009</span></span>
<span data-ttu-id="de609-178">请求包含使用重复名称的部分。</span><span class="sxs-lookup"><span data-stu-id="de609-178">The request contains parts with duplicate names.</span></span> <span data-ttu-id="de609-179">部分名称必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="de609-179">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="de609-180">20010</span><span class="sxs-lookup"><span data-stu-id="de609-180">20010</span></span>
<span data-ttu-id="de609-181">未提供指定内容类型的内容处置标头。</span><span class="sxs-lookup"><span data-stu-id="de609-181">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="de609-182">20011</span><span class="sxs-lookup"><span data-stu-id="de609-182">20011</span></span>
<span data-ttu-id="de609-183">请求包含格式错误的多部分有效负载。</span><span class="sxs-lookup"><span data-stu-id="de609-183">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="de609-184">问题可能包括缺少空行、缺少末行、部分分隔符格式不正确等。</span><span class="sxs-lookup"><span data-stu-id="de609-184">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="de609-185">如果正在手动生成多部分消息，请仔细检查逻辑，或者考虑使用第三方库。</span><span class="sxs-lookup"><span data-stu-id="de609-185">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="de609-186">20012</span><span class="sxs-lookup"><span data-stu-id="de609-186">20012</span></span>
<span data-ttu-id="de609-187">请求未提供指定部分的内容类型。</span><span class="sxs-lookup"><span data-stu-id="de609-187">The request doesn't supply a content type for the specified part.</span></span> 

### <a name="20013"></a><span data-ttu-id="de609-188">20013</span><span class="sxs-lookup"><span data-stu-id="de609-188">20013</span></span>
<span data-ttu-id="de609-189">请求未提供指定部分的内容类型和内容处置标头。</span><span class="sxs-lookup"><span data-stu-id="de609-189">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="de609-190">20014</span><span class="sxs-lookup"><span data-stu-id="de609-190">20014</span></span>
<span data-ttu-id="de609-191">多部分消息中的某个部分的长度超过最大大小 25 MB。</span><span class="sxs-lookup"><span data-stu-id="de609-191">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="de609-192">20015</span><span class="sxs-lookup"><span data-stu-id="de609-192">20015</span></span>
<span data-ttu-id="de609-193">多部分消息中的部分计数超过 500 个的限制。</span><span class="sxs-lookup"><span data-stu-id="de609-193">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="de609-194">20016</span><span class="sxs-lookup"><span data-stu-id="de609-194">20016</span></span>
<span data-ttu-id="de609-195">多部分消息的长度超过 75 MB 的限制。</span><span class="sxs-lookup"><span data-stu-id="de609-195">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="de609-196">20017</span><span class="sxs-lookup"><span data-stu-id="de609-196">20017</span></span>
<span data-ttu-id="de609-197">电子邮件 MIME 格式不正确。</span><span class="sxs-lookup"><span data-stu-id="de609-197">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="de609-198">20018</span><span class="sxs-lookup"><span data-stu-id="de609-198">20018</span></span>
<span data-ttu-id="de609-199">会议 MIME 或 ICal 格式不正确。</span><span class="sxs-lookup"><span data-stu-id="de609-199">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="de609-200">20019</span><span class="sxs-lookup"><span data-stu-id="de609-200">20019</span></span>
<span data-ttu-id="de609-201">找不到 ICal。</span><span class="sxs-lookup"><span data-stu-id="de609-201">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="de609-202">20020</span><span class="sxs-lookup"><span data-stu-id="de609-202">20020</span></span>
<span data-ttu-id="de609-203">在请求正文中遇到格式不正确的 Json。</span><span class="sxs-lookup"><span data-stu-id="de609-203">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="de609-204">20100</span><span class="sxs-lookup"><span data-stu-id="de609-204">20100</span></span>
<span data-ttu-id="de609-205">请求的语法有问题。</span><span class="sxs-lookup"><span data-stu-id="de609-205">Something is wrong with the syntax of your request.</span></span> 

### <a name="20101"></a><span data-ttu-id="de609-206">20101</span><span class="sxs-lookup"><span data-stu-id="de609-206">20101</span></span>
<span data-ttu-id="de609-207">所请求的属性不存在。</span><span class="sxs-lookup"><span data-stu-id="de609-207">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="de609-208">20102</span><span class="sxs-lookup"><span data-stu-id="de609-208">20102</span></span>
<span data-ttu-id="de609-209">所请求的资源不存在。</span><span class="sxs-lookup"><span data-stu-id="de609-209">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="de609-210">20103</span><span class="sxs-lookup"><span data-stu-id="de609-210">20103</span></span>
<span data-ttu-id="de609-211">此请求不支持 **expand** 查询。</span><span class="sxs-lookup"><span data-stu-id="de609-211">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="de609-212">请参阅[受支持的 OData 查询字符串选项](onenote-get-content.md#supported-odata-query-string-options)。</span><span class="sxs-lookup"><span data-stu-id="de609-212">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20104"></a><span data-ttu-id="de609-213">20104</span><span class="sxs-lookup"><span data-stu-id="de609-213">20104</span></span>
<span data-ttu-id="de609-p119">仅当查询某个部分中的网页集或查询特定页时，才支持 **pagelevel** 查询选项。例如：</span><span class="sxs-lookup"><span data-stu-id="de609-p119">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="de609-216">20106</span><span class="sxs-lookup"><span data-stu-id="de609-216">20106</span></span>
<span data-ttu-id="de609-217">你的请求包含不受支持的查询运算符。</span><span class="sxs-lookup"><span data-stu-id="de609-217">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="de609-218">20108</span><span class="sxs-lookup"><span data-stu-id="de609-218">20108</span></span>
<span data-ttu-id="de609-219">您的请求包含不受支持的 OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="de609-219">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="de609-220">20109</span><span class="sxs-lookup"><span data-stu-id="de609-220">20109</span></span>
<span data-ttu-id="de609-221">PATCH 请求中的有效负载构建不正确。</span><span class="sxs-lookup"><span data-stu-id="de609-221">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="de609-222">20110</span><span class="sxs-lookup"><span data-stu-id="de609-222">20110</span></span>
<span data-ttu-id="de609-223">包含数据部分的页面创建请求要求内容为多部分，并包含“演示”部分。</span><span class="sxs-lookup"><span data-stu-id="de609-223">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="de609-224">20111</span><span class="sxs-lookup"><span data-stu-id="de609-224">20111</span></span>
<span data-ttu-id="de609-225">你的请求使用不受支持的 OData 功能。</span><span class="sxs-lookup"><span data-stu-id="de609-225">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="de609-226">20112</span><span class="sxs-lookup"><span data-stu-id="de609-226">20112</span></span>
<span data-ttu-id="de609-227">您的请求包含无效的目标笔记本、节组、节或页面实体 ID。</span><span class="sxs-lookup"><span data-stu-id="de609-227">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="de609-228">20113</span><span class="sxs-lookup"><span data-stu-id="de609-228">20113</span></span>
<span data-ttu-id="de609-229">请求中指定的资源已被删除。</span><span class="sxs-lookup"><span data-stu-id="de609-229">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="de609-230">20115</span><span class="sxs-lookup"><span data-stu-id="de609-230">20115</span></span>
<span data-ttu-id="de609-231">名称包含无效字符。</span><span class="sxs-lookup"><span data-stu-id="de609-231">The name contains invalid characters.</span></span> <span data-ttu-id="de609-232">笔记本名称中不能包含下列任意字符：`? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="de609-232">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="de609-233">20117</span><span class="sxs-lookup"><span data-stu-id="de609-233">20117</span></span>
<span data-ttu-id="de609-234">在您指定的位置中已存在指定名称的项。</span><span class="sxs-lookup"><span data-stu-id="de609-234">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="de609-235">20119</span><span class="sxs-lookup"><span data-stu-id="de609-235">20119</span></span>
<span data-ttu-id="de609-236">“演示”部分的 HTML 包含一个 **data-attachment** 属性，该属性不为有效格式，或者包含一个或多个对文件名无效的字符：`\ / : * ? < > | "`。</span><span class="sxs-lookup"><span data-stu-id="de609-236">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="de609-237">请求替代了错误消息中指示的值。</span><span class="sxs-lookup"><span data-stu-id="de609-237">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="de609-238">20120</span><span class="sxs-lookup"><span data-stu-id="de609-238">20120</span></span>
<span data-ttu-id="de609-239">找不到你的请求指定的 PATCH 目标。</span><span class="sxs-lookup"><span data-stu-id="de609-239">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="de609-240">20121</span><span class="sxs-lookup"><span data-stu-id="de609-240">20121</span></span>
<span data-ttu-id="de609-p122">请求包含无效的 PATCH 参数。请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p122">Your request contains an invalid PATCH argument. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20122"></a><span data-ttu-id="de609-243">20122</span><span class="sxs-lookup"><span data-stu-id="de609-243">20122</span></span>
<span data-ttu-id="de609-p123">请求指定的 PATCH 操作不受支持。请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p123">Your request specifies an unsupported PATCH action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20123"></a><span data-ttu-id="de609-246">20123</span><span class="sxs-lookup"><span data-stu-id="de609-246">20123</span></span>
<span data-ttu-id="de609-247">PATCH 请求无法修改指定页面。</span><span class="sxs-lookup"><span data-stu-id="de609-247">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="de609-248">20124</span><span class="sxs-lookup"><span data-stu-id="de609-248">20124</span></span>
<span data-ttu-id="de609-249">你的多部分 PATCH 请求不包含使用 PATCH 操作 JSON 结构的“命令”部分。</span><span class="sxs-lookup"><span data-stu-id="de609-249">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="de609-250">请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-250">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20125"></a><span data-ttu-id="de609-251">20125</span><span class="sxs-lookup"><span data-stu-id="de609-251">20125</span></span>
<span data-ttu-id="de609-p125">PATCH 请求不包含任何操作。请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p125">Your PATCH request contains no actions. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20126"></a><span data-ttu-id="de609-254">20126</span><span class="sxs-lookup"><span data-stu-id="de609-254">20126</span></span>
<span data-ttu-id="de609-255">邮件正文包含格式错误的 JSON 或此操作不支持的字段。</span><span class="sxs-lookup"><span data-stu-id="de609-255">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="de609-256">20127</span><span class="sxs-lookup"><span data-stu-id="de609-256">20127</span></span>
<span data-ttu-id="de609-257">您的请求指定了未知属性的名称。</span><span class="sxs-lookup"><span data-stu-id="de609-257">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="de609-258">20128</span><span class="sxs-lookup"><span data-stu-id="de609-258">20128</span></span>
<span data-ttu-id="de609-259">您的请求在消息中指示的位置包含 OData 语法错误。</span><span class="sxs-lookup"><span data-stu-id="de609-259">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="de609-260">20129</span><span class="sxs-lookup"><span data-stu-id="de609-260">20129</span></span>
<span data-ttu-id="de609-261">你的请求包含值过高的 **top** 查询字符串选项。</span><span class="sxs-lookup"><span data-stu-id="de609-261">Your request contains a **top** query string option whose value is too high.</span></span> <span data-ttu-id="de609-262">对于页面查询，最大值为 100，默认值为 20。</span><span class="sxs-lookup"><span data-stu-id="de609-262">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="de609-263">20130</span><span class="sxs-lookup"><span data-stu-id="de609-263">20130</span></span>
<span data-ttu-id="de609-264">你的请求包含指向找不到的 HTTP 资源的 URI。</span><span class="sxs-lookup"><span data-stu-id="de609-264">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="de609-265">20131</span><span class="sxs-lookup"><span data-stu-id="de609-265">20131</span></span>
<span data-ttu-id="de609-266">你的请求包含无效的内容类型值。</span><span class="sxs-lookup"><span data-stu-id="de609-266">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="de609-267">请使用消息中指示的值。</span><span class="sxs-lookup"><span data-stu-id="de609-267">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="de609-268">20132</span><span class="sxs-lookup"><span data-stu-id="de609-268">20132</span></span>
<span data-ttu-id="de609-269">你的请求包含无效的内容。</span><span class="sxs-lookup"><span data-stu-id="de609-269">Your request contains invalid content.</span></span> <span data-ttu-id="de609-270">此问题的常见原因是缺少内容类型请求标头和/或请求正文中没有内容。</span><span class="sxs-lookup"><span data-stu-id="de609-270">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="de609-271">20133</span><span class="sxs-lookup"><span data-stu-id="de609-271">20133</span></span>
<span data-ttu-id="de609-272">你的请求指定的 PATCH 目标不受支持。</span><span class="sxs-lookup"><span data-stu-id="de609-272">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="de609-273">请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-273">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20134"></a><span data-ttu-id="de609-274">20134</span><span class="sxs-lookup"><span data-stu-id="de609-274">20134</span></span>
<span data-ttu-id="de609-p130">您的请求将无效元素指定为 PATCH 操作的目标。如果目标使用 **data-id** 标识符，请确保其前缀为 # 符号。请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p130">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20135"></a><span data-ttu-id="de609-278">20135</span><span class="sxs-lookup"><span data-stu-id="de609-278">20135</span></span>
<span data-ttu-id="de609-279">你的请求指定的实体类型不受 PATCH 操作支持。</span><span class="sxs-lookup"><span data-stu-id="de609-279">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="de609-280">请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-280">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20136"></a><span data-ttu-id="de609-281">20136</span><span class="sxs-lookup"><span data-stu-id="de609-281">20136</span></span>
<span data-ttu-id="de609-282">你的请求包含无效的 **data-render-src** 或 **data-render-method** 属性或缺失这些属性。</span><span class="sxs-lookup"><span data-stu-id="de609-282">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute.</span></span> <span data-ttu-id="de609-283">请参阅[从捕获内容中提取数据](onenote-extract-data.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-283">See [Extract data from captures](onenote-extract-data.md).</span></span>

### <a name="20137"></a><span data-ttu-id="de609-284">20137</span><span class="sxs-lookup"><span data-stu-id="de609-284">20137</span></span>
<span data-ttu-id="de609-285">目标页面不支持 PATCH 请求。</span><span class="sxs-lookup"><span data-stu-id="de609-285">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="de609-286">20138</span><span class="sxs-lookup"><span data-stu-id="de609-286">20138</span></span>
<span data-ttu-id="de609-p133">PATCH 请求中的目标元素类型不支持 **append** 操作。请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p133">The target element type in your PATCH request doesn't support the **append** action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20139"></a><span data-ttu-id="de609-289">20139</span><span class="sxs-lookup"><span data-stu-id="de609-289">20139</span></span>
<span data-ttu-id="de609-p134">请求包含无效的 **data-tag** 属性值。请参阅[使用笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-p134">Your request contains an invalid **data-tag** attribute value. See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20140"></a><span data-ttu-id="de609-292">20140</span><span class="sxs-lookup"><span data-stu-id="de609-292">20140</span></span>
<span data-ttu-id="de609-293">你的请求包含无效的 **data-tag** 状态值。</span><span class="sxs-lookup"><span data-stu-id="de609-293">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="de609-294">复选框笔记标记可以包含**已完成**状态。</span><span class="sxs-lookup"><span data-stu-id="de609-294">Check box note tags can have a **completed** status.</span></span> 

<span data-ttu-id="de609-295">示例：</span><span class="sxs-lookup"><span data-stu-id="de609-295">Example:</span></span>

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="de609-296">请参阅[使用笔记标记](onenote-note-tags.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-296">See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20141"></a><span data-ttu-id="de609-297">20141</span><span class="sxs-lookup"><span data-stu-id="de609-297">20141</span></span>
<span data-ttu-id="de609-298">PATCH 请求中的目标不支持指定操作。</span><span class="sxs-lookup"><span data-stu-id="de609-298">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="de609-299">请参阅[更新页面内容](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-299">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20142"></a><span data-ttu-id="de609-300">20142</span><span class="sxs-lookup"><span data-stu-id="de609-300">20142</span></span>
<span data-ttu-id="de609-301">你的请求包含子实体的父项或父实体的子项的 **expand** 表达式，但它并不受支持。</span><span class="sxs-lookup"><span data-stu-id="de609-301">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported.</span></span> <span data-ttu-id="de609-302">请参阅[受支持的 OData 查询字符串选项](onenote-get-content.md#supported-odata-query-string-options)。</span><span class="sxs-lookup"><span data-stu-id="de609-302">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20143"></a><span data-ttu-id="de609-303">20143</span><span class="sxs-lookup"><span data-stu-id="de609-303">20143</span></span>
<span data-ttu-id="de609-304">OData 查询无效。</span><span class="sxs-lookup"><span data-stu-id="de609-304">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="de609-305">20144</span><span class="sxs-lookup"><span data-stu-id="de609-305">20144</span></span>
<span data-ttu-id="de609-306">你的请求包含非导航属性的 **expand** 表达式。</span><span class="sxs-lookup"><span data-stu-id="de609-306">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="de609-307">只能扩展导航属性。</span><span class="sxs-lookup"><span data-stu-id="de609-307">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="de609-308">20145</span><span class="sxs-lookup"><span data-stu-id="de609-308">20145</span></span>
<span data-ttu-id="de609-309">你的请求中的 **select** 或 **expand** 表达式包含无效条件。</span><span class="sxs-lookup"><span data-stu-id="de609-309">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="de609-310">20146</span><span class="sxs-lookup"><span data-stu-id="de609-310">20146</span></span>
<span data-ttu-id="de609-311">元素上指定了 `style="position:absolute"` 属性，但是 **body** 元素未指定支持定位所需的 `data-absolute-enabled="true"`。</span><span class="sxs-lookup"><span data-stu-id="de609-311">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="de609-312">将忽略所有的定位设置。</span><span class="sxs-lookup"><span data-stu-id="de609-312">All position settings will be ignored.</span></span> <span data-ttu-id="de609-313">请参阅[创建绝对定位的元素](onenote-abs-pos.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-313">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="de609-314">20147</span><span class="sxs-lookup"><span data-stu-id="de609-314">20147</span></span>
<span data-ttu-id="de609-315">在非 **body** 元素直接子级的元素上指定了不受支持的 `style="position:absolute"` 属性。</span><span class="sxs-lookup"><span data-stu-id="de609-315">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="de609-316">如果元素是 **div**、**img** 或 **object**，请使其成为正文的直接子级；否则，将忽略定位设置，并在绝对定位的 div 中呈现它的内容。</span><span class="sxs-lookup"><span data-stu-id="de609-316">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="de609-317">请参阅[创建绝对定位的元素](onenote-abs-pos.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-317">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="de609-318">20148</span><span class="sxs-lookup"><span data-stu-id="de609-318">20148</span></span>
<span data-ttu-id="de609-319">在不支持 `style="position:absolute"` 属性的元素类型上指定了此属性。</span><span class="sxs-lookup"><span data-stu-id="de609-319">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="de609-320">仅属于页面正文直接子级的 **div**、**img**、和 **object** 元素支持定位。</span><span class="sxs-lookup"><span data-stu-id="de609-320">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="de609-321">请参阅[创建绝对定位的元素](onenote-abs-pos.md)。</span><span class="sxs-lookup"><span data-stu-id="de609-321">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="de609-322">20149</span><span class="sxs-lookup"><span data-stu-id="de609-322">20149</span></span>
<span data-ttu-id="de609-323">您的请求指定的目标元素找不到。</span><span class="sxs-lookup"><span data-stu-id="de609-323">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="de609-324">20150</span><span class="sxs-lookup"><span data-stu-id="de609-324">20150</span></span>
<span data-ttu-id="de609-325">请求对此身份验证类型无效。</span><span class="sxs-lookup"><span data-stu-id="de609-325">The request is not valid for this authentication type.</span></span> <span data-ttu-id="de609-326">请改用 `../me/onenote/` 路径。</span><span class="sxs-lookup"><span data-stu-id="de609-326">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="de609-327">20151</span><span class="sxs-lookup"><span data-stu-id="de609-327">20151</span></span>
<span data-ttu-id="de609-328">请求对此身份验证类型无效。</span><span class="sxs-lookup"><span data-stu-id="de609-328">The request is not valid for this authentication type.</span></span> <span data-ttu-id="de609-329">请使用 `../me/onenote/section/{id}/pages` 终结点在特定分区中创建页面。</span><span class="sxs-lookup"><span data-stu-id="de609-329">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="de609-330">20152</span><span class="sxs-lookup"><span data-stu-id="de609-330">20152</span></span>
<span data-ttu-id="de609-p144">没有为实体指定任何 name 值。必须定义名称，并且其中不能仅包含空格。</span><span class="sxs-lookup"><span data-stu-id="de609-p144">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="de609-333">20153</span><span class="sxs-lookup"><span data-stu-id="de609-333">20153</span></span>
<span data-ttu-id="de609-334">实体名称包含无效字符。</span><span class="sxs-lookup"><span data-stu-id="de609-334">The entity name contains invalid characters.</span></span> <span data-ttu-id="de609-335">名称中不能包含下列字符：`? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="de609-335">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="de609-336">20154</span><span class="sxs-lookup"><span data-stu-id="de609-336">20154</span></span>
<span data-ttu-id="de609-337">实体名称不能以空格开头。</span><span class="sxs-lookup"><span data-stu-id="de609-337">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="de609-338">20155</span><span class="sxs-lookup"><span data-stu-id="de609-338">20155</span></span>
<span data-ttu-id="de609-339">实体名称太长。</span><span class="sxs-lookup"><span data-stu-id="de609-339">The entity name is too long.</span></span> <span data-ttu-id="de609-340">笔记本名称的字符数限制为 128 个。</span><span class="sxs-lookup"><span data-stu-id="de609-340">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="de609-341">其他实体名称的字符数限制为 50 个。</span><span class="sxs-lookup"><span data-stu-id="de609-341">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="de609-342">20156</span><span class="sxs-lookup"><span data-stu-id="de609-342">20156</span></span>
<span data-ttu-id="de609-343">目标资源的指定 ID 不存在。</span><span class="sxs-lookup"><span data-stu-id="de609-343">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="de609-344">20157</span><span class="sxs-lookup"><span data-stu-id="de609-344">20157</span></span>
<span data-ttu-id="de609-345">目标实体的指定 ID 无效。</span><span class="sxs-lookup"><span data-stu-id="de609-345">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="de609-346">20158</span><span class="sxs-lookup"><span data-stu-id="de609-346">20158</span></span>
<span data-ttu-id="de609-347">无法获取请求中指定的网站 URL 的元数据。</span><span class="sxs-lookup"><span data-stu-id="de609-347">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="de609-348">请检查所提供的 URL 的格式。</span><span class="sxs-lookup"><span data-stu-id="de609-348">Check the format of the supplied URL.</span></span> <span data-ttu-id="de609-349">支持的格式包括 `https://domain.sharepoint.com/site-a` 和 `https://domain.com/sites/site-a`。</span><span class="sxs-lookup"><span data-stu-id="de609-349">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="de609-350">20160</span><span class="sxs-lookup"><span data-stu-id="de609-350">20160</span></span>
<span data-ttu-id="de609-351">找不到具有指定 ID 的 Office 365 统一组。</span><span class="sxs-lookup"><span data-stu-id="de609-351">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="de609-352">20161</span><span class="sxs-lookup"><span data-stu-id="de609-352">20161</span></span>
<span data-ttu-id="de609-353">此上下文没有指定有效的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="de609-353">The context does not specify a valid user ID.</span></span> <span data-ttu-id="de609-354">一个常见错误是 PUID/CID 作为 long 而不是作为 hex 传入。</span><span class="sxs-lookup"><span data-stu-id="de609-354">One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="de609-355">20166</span><span class="sxs-lookup"><span data-stu-id="de609-355">20166</span></span>
<span data-ttu-id="de609-356">应用程序在短时间内以用户身份发出的请求过多。</span><span class="sxs-lookup"><span data-stu-id="de609-356">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="de609-357">当 API 检测到应用程序使用的资源过多时，它会返回 429 状态代码和此错误，以帮助确保 OneNote API 保持稳定和可响应状态。</span><span class="sxs-lookup"><span data-stu-id="de609-357">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="de609-358">有关详细信息，请参阅 [OneNote API 限制及避免方法](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx)。</span><span class="sxs-lookup"><span data-stu-id="de609-358">For more information, see [OneNote API throttling and how to avoid it](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="de609-359">20168</span><span class="sxs-lookup"><span data-stu-id="de609-359">20168</span></span>
<span data-ttu-id="de609-360">请求中指定的视频源不受支持。</span><span class="sxs-lookup"><span data-stu-id="de609-360">The video source specified in the request is not supported.</span></span> <span data-ttu-id="de609-361">请参阅[支持的视频网站](onenote-images-files.md#adding-videos)获取最新列表。</span><span class="sxs-lookup"><span data-stu-id="de609-361">See [Supported video sites](onenote-images-files.md#adding-videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="de609-362">从 30001 到 39999 的代码</span><span class="sxs-lookup"><span data-stu-id="de609-362">Codes from 30001 to 39999</span></span>
<span data-ttu-id="de609-363">用户的帐户有问题。</span><span class="sxs-lookup"><span data-stu-id="de609-363">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="de609-364">30101</span><span class="sxs-lookup"><span data-stu-id="de609-364">30101</span></span>
<span data-ttu-id="de609-365">用户帐户超出了它的 OneDrive 配额。</span><span class="sxs-lookup"><span data-stu-id="de609-365">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="de609-366">请参阅 [OneDrive](https://onedrive.live.com/about/zh-CN/)。</span><span class="sxs-lookup"><span data-stu-id="de609-366">See [OneDrive](https://onedrive.live.com/about/zh-CN/).</span></span>

### <a name="30102"></a><span data-ttu-id="de609-367">30102</span><span class="sxs-lookup"><span data-stu-id="de609-367">30102</span></span>
<span data-ttu-id="de609-368">不能再向请求的节添加任何内容，因为它已经达到其最大大小。</span><span class="sxs-lookup"><span data-stu-id="de609-368">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="de609-369">30103</span><span class="sxs-lookup"><span data-stu-id="de609-369">30103</span></span>
<span data-ttu-id="de609-370">此请求的资源消耗过高。</span><span class="sxs-lookup"><span data-stu-id="de609-370">Resource consumption is too high for the request.</span></span> <span data-ttu-id="de609-371">目标用户帐户的数据集过大或服务将过多数量的并发请求接收到同一个网站（例如，用户的个人网站或团队网站）。</span><span class="sxs-lookup"><span data-stu-id="de609-371">Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="de609-372">30104</span><span class="sxs-lookup"><span data-stu-id="de609-372">30104</span></span>
<span data-ttu-id="de609-373">用户帐户已被挂起。</span><span class="sxs-lookup"><span data-stu-id="de609-373">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="de609-374">30105</span><span class="sxs-lookup"><span data-stu-id="de609-374">30105</span></span>
<span data-ttu-id="de609-375">未设置用户的个人 OneDrive for Business 网站，需要设置该网站才能访问笔记本。</span><span class="sxs-lookup"><span data-stu-id="de609-375">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="de609-376">OneNote 服务将立即设置此网站。</span><span class="sxs-lookup"><span data-stu-id="de609-376">The OneNote service will provision the site now.</span></span> <span data-ttu-id="de609-377">此进程可能需要几分钟。</span><span class="sxs-lookup"><span data-stu-id="de609-377">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="de609-378">30106</span><span class="sxs-lookup"><span data-stu-id="de609-378">30106</span></span>
<span data-ttu-id="de609-379">正在为用户设置 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="de609-379">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="de609-380">30108</span><span class="sxs-lookup"><span data-stu-id="de609-380">30108</span></span>
<span data-ttu-id="de609-381">无法检索用户的个人 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="de609-381">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="de609-382">下表列出了部分可能的原因。</span><span class="sxs-lookup"><span data-stu-id="de609-382">The following table lists some possible causes.</span></span>

| <span data-ttu-id="de609-383">原因</span><span class="sxs-lookup"><span data-stu-id="de609-383">Cause</span></span> | <span data-ttu-id="de609-384">解决方案</span><span class="sxs-lookup"><span data-stu-id="de609-384">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="de609-385">尚未设置用户的个人网站。</span><span class="sxs-lookup"><span data-stu-id="de609-385">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="de609-386">用户应打开 OneDrive for Business，并按照任意说明设置此网站。</span><span class="sxs-lookup"><span data-stu-id="de609-386">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="de609-387">如果此操作失败，用户应联系他们的 Office 365 租户管理员。</span><span class="sxs-lookup"><span data-stu-id="de609-387">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="de609-388">当前正在设置用户的个人网站。</span><span class="sxs-lookup"><span data-stu-id="de609-388">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="de609-389">稍后再尝试请求。</span><span class="sxs-lookup"><span data-stu-id="de609-389">Try the request later.</span></span> |
| <span data-ttu-id="de609-390">用户没有有效的 OneDrive for Business 许可证。</span><span class="sxs-lookup"><span data-stu-id="de609-390">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="de609-391">用户应联系他们的 Office 365 租户管理员。</span><span class="sxs-lookup"><span data-stu-id="de609-391">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="de609-392">网络问题使请求无法成功发送。</span><span class="sxs-lookup"><span data-stu-id="de609-392">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="de609-393">稍后再尝试请求。</span><span class="sxs-lookup"><span data-stu-id="de609-393">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="de609-394">30109</span><span class="sxs-lookup"><span data-stu-id="de609-394">30109</span></span>
<span data-ttu-id="de609-395">请求中的某些用户不存在。</span><span class="sxs-lookup"><span data-stu-id="de609-395">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="de609-396">30110</span><span class="sxs-lookup"><span data-stu-id="de609-396">30110</span></span>
<span data-ttu-id="de609-397">此租户尚未注册学生信息服务。</span><span class="sxs-lookup"><span data-stu-id="de609-397">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="de609-398">30111</span><span class="sxs-lookup"><span data-stu-id="de609-398">30111</span></span>
<span data-ttu-id="de609-399">学生信息服务出现一般性错误。</span><span class="sxs-lookup"><span data-stu-id="de609-399">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="de609-400">30112</span><span class="sxs-lookup"><span data-stu-id="de609-400">30112</span></span>
<span data-ttu-id="de609-401">受请求影响的多个用户具有相同的用户名。</span><span class="sxs-lookup"><span data-stu-id="de609-401">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="de609-402">30113</span><span class="sxs-lookup"><span data-stu-id="de609-402">30113</span></span>
<span data-ttu-id="de609-403">笔记本未配置为允许邀请。</span><span class="sxs-lookup"><span data-stu-id="de609-403">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="de609-404">30114</span><span class="sxs-lookup"><span data-stu-id="de609-404">30114</span></span>
<span data-ttu-id="de609-405">缺少必需的参数。</span><span class="sxs-lookup"><span data-stu-id="de609-405">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="de609-406">从 40001 到 49999 的代码</span><span class="sxs-lookup"><span data-stu-id="de609-406">Codes from 40001 to 49999</span></span>
<span data-ttu-id="de609-407">用户或应用程序没有正确的权限。</span><span class="sxs-lookup"><span data-stu-id="de609-407">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="de609-408">40001</span><span class="sxs-lookup"><span data-stu-id="de609-408">40001</span></span>
<span data-ttu-id="de609-409">请求不包含有效的 OAuth 标记。</span><span class="sxs-lookup"><span data-stu-id="de609-409">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="de609-410">请参阅[注释权限](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="de609-410">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="de609-411">40002</span><span class="sxs-lookup"><span data-stu-id="de609-411">40002</span></span>
<span data-ttu-id="de609-412">用户在所请求的位置没有写入权限。</span><span class="sxs-lookup"><span data-stu-id="de609-412">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="de609-413">40003</span><span class="sxs-lookup"><span data-stu-id="de609-413">40003</span></span>
<span data-ttu-id="de609-414">用户没有权限访问所请求的资源。</span><span class="sxs-lookup"><span data-stu-id="de609-414">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="de609-415">40004</span><span class="sxs-lookup"><span data-stu-id="de609-415">40004</span></span>
<span data-ttu-id="de609-416">OAuth 令牌没有所需的作用域来执行所请求的操作。</span><span class="sxs-lookup"><span data-stu-id="de609-416">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="de609-417">请参阅[注释权限](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="de609-417">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="de609-418">40006</span><span class="sxs-lookup"><span data-stu-id="de609-418">40006</span></span> 
<span data-ttu-id="de609-419">OAuth 令牌没有所需的作用域来执行所请求的操作。</span><span class="sxs-lookup"><span data-stu-id="de609-419">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="de609-420">尤其是编辑权限。</span><span class="sxs-lookup"><span data-stu-id="de609-420">Specifically the edit permission.</span></span> <span data-ttu-id="de609-421">请参阅[注释权限](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="de609-421">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="de609-422">40007</span><span class="sxs-lookup"><span data-stu-id="de609-422">40007</span></span>
<span data-ttu-id="de609-423">用户没有权限访问此资源。</span><span class="sxs-lookup"><span data-stu-id="de609-423">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="de609-424">40008</span><span class="sxs-lookup"><span data-stu-id="de609-424">40008</span></span>
<span data-ttu-id="de609-425">禁止访问此资源。</span><span class="sxs-lookup"><span data-stu-id="de609-425">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="de609-426">40009</span><span class="sxs-lookup"><span data-stu-id="de609-426">40009</span></span>
<span data-ttu-id="de609-427">容器已被其他资源使用。</span><span class="sxs-lookup"><span data-stu-id="de609-427">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="de609-428">另请参阅</span><span class="sxs-lookup"><span data-stu-id="de609-428">See also</span></span>

- [<span data-ttu-id="de609-429">Microsoft Graph 错误响应和资源类型</span><span class="sxs-lookup"><span data-stu-id="de609-429">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="de609-430">OneNote 参考</span><span class="sxs-lookup"><span data-stu-id="de609-430">OneNote reference</span></span>](/graph/api/resources/onenote?view=graph-rest-1.0)

