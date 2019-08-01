---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 407a6831c8a4ab82a71229865f5b2f2ae00f0dca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021716"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="0b804-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0b804-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

<span data-ttu-id="0b804-105">获取使用情况趋势，即组织中用户参与的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="0b804-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="0b804-106">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="0b804-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="0b804-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="0b804-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b804-108">权限</span><span class="sxs-lookup"><span data-stu-id="0b804-108">Permissions</span></span>

<span data-ttu-id="0b804-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b804-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b804-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b804-111">Permission type</span></span>                        | <span data-ttu-id="0b804-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b804-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b804-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b804-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b804-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b804-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b804-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b804-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b804-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b804-116">Not supported.</span></span>                           |
| <span data-ttu-id="0b804-117">应用</span><span class="sxs-lookup"><span data-stu-id="0b804-117">Application</span></span>                            | <span data-ttu-id="0b804-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b804-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b804-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b804-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b804-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0b804-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0b804-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="0b804-121">Function parameters</span></span>

<span data-ttu-id="0b804-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0b804-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0b804-123">参数</span><span class="sxs-lookup"><span data-stu-id="0b804-123">Parameter</span></span> | <span data-ttu-id="0b804-124">类型</span><span class="sxs-lookup"><span data-stu-id="0b804-124">Type</span></span>   | <span data-ttu-id="0b804-125">说明</span><span class="sxs-lookup"><span data-stu-id="0b804-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b804-126">period</span><span class="sxs-lookup"><span data-stu-id="0b804-126">period</span></span>    | <span data-ttu-id="0b804-127">string</span><span class="sxs-lookup"><span data-stu-id="0b804-127">string</span></span> | <span data-ttu-id="0b804-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b804-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b804-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0b804-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b804-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b804-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0b804-131">必需。</span><span class="sxs-lookup"><span data-stu-id="0b804-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0b804-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b804-132">Request headers</span></span>

| <span data-ttu-id="0b804-133">名称</span><span class="sxs-lookup"><span data-stu-id="0b804-133">Name</span></span>          | <span data-ttu-id="0b804-134">说明</span><span class="sxs-lookup"><span data-stu-id="0b804-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0b804-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b804-135">Authorization</span></span> | <span data-ttu-id="0b804-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b804-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0b804-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0b804-138">If-None-Match</span></span> | <span data-ttu-id="0b804-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0b804-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0b804-140">可选。</span><span class="sxs-lookup"><span data-stu-id="0b804-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0b804-141">响应</span><span class="sxs-lookup"><span data-stu-id="0b804-141">Response</span></span>

<span data-ttu-id="0b804-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0b804-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b804-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0b804-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b804-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="0b804-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b804-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="0b804-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b804-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0b804-146">Report Refresh Date</span></span>
- <span data-ttu-id="0b804-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="0b804-147">Report Date</span></span>
- <span data-ttu-id="0b804-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="0b804-148">Report Period</span></span>
- <span data-ttu-id="0b804-149">IM</span><span class="sxs-lookup"><span data-stu-id="0b804-149">IM</span></span>
- <span data-ttu-id="0b804-150">音频/视频</span><span class="sxs-lookup"><span data-stu-id="0b804-150">Audio/Video</span></span>
- <span data-ttu-id="0b804-151">应用共享</span><span class="sxs-lookup"><span data-stu-id="0b804-151">App Sharing</span></span>
- <span data-ttu-id="0b804-152">Web</span><span class="sxs-lookup"><span data-stu-id="0b804-152">Web</span></span>
- <span data-ttu-id="0b804-153">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="0b804-153">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="0b804-154">示例</span><span class="sxs-lookup"><span data-stu-id="0b804-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0b804-155">请求</span><span class="sxs-lookup"><span data-stu-id="0b804-155">Request</span></span>

<span data-ttu-id="0b804-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b804-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b804-157">C#</span><span class="sxs-lookup"><span data-stu-id="0b804-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b804-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b804-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b804-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b804-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b804-160">Java</span><span class="sxs-lookup"><span data-stu-id="0b804-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b804-161">响应</span><span class="sxs-lookup"><span data-stu-id="0b804-161">Response</span></span>

<span data-ttu-id="0b804-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b804-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b804-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0b804-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
