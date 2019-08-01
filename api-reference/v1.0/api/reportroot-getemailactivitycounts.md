---
title: 'reportRoot: getEmailActivityCounts'
description: 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2dd98b73f3dbba6881bc7e68f4d0657d49e1b3c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022083"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="0b2e9-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0b2e9-103">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="0b2e9-104">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="0b2e9-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b2e9-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b2e9-106">Permissions</span></span>

<span data-ttu-id="0b2e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b2e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b2e9-109">Permission type</span></span>                        | <span data-ttu-id="0b2e9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b2e9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b2e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b2e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b2e9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b2e9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b2e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b2e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b2e9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b2e9-115">应用</span><span class="sxs-lookup"><span data-stu-id="0b2e9-115">Application</span></span>                            | <span data-ttu-id="0b2e9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b2e9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b2e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b2e9-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b2e9-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0b2e9-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0b2e9-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="0b2e9-119">Function parameters</span></span>

<span data-ttu-id="0b2e9-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0b2e9-121">参数</span><span class="sxs-lookup"><span data-stu-id="0b2e9-121">Parameter</span></span> | <span data-ttu-id="0b2e9-122">类型</span><span class="sxs-lookup"><span data-stu-id="0b2e9-122">Type</span></span>   | <span data-ttu-id="0b2e9-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b2e9-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b2e9-124">period</span><span class="sxs-lookup"><span data-stu-id="0b2e9-124">period</span></span>    | <span data-ttu-id="0b2e9-125">string</span><span class="sxs-lookup"><span data-stu-id="0b2e9-125">string</span></span> | <span data-ttu-id="0b2e9-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b2e9-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b2e9-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0b2e9-129">必需。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0b2e9-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b2e9-130">Request headers</span></span>

| <span data-ttu-id="0b2e9-131">名称</span><span class="sxs-lookup"><span data-stu-id="0b2e9-131">Name</span></span>          | <span data-ttu-id="0b2e9-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b2e9-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0b2e9-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b2e9-133">Authorization</span></span> | <span data-ttu-id="0b2e9-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0b2e9-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0b2e9-136">If-None-Match</span></span> | <span data-ttu-id="0b2e9-137">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0b2e9-138">可选。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0b2e9-139">响应</span><span class="sxs-lookup"><span data-stu-id="0b2e9-139">Response</span></span>

<span data-ttu-id="0b2e9-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b2e9-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b2e9-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b2e9-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b2e9-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0b2e9-144">Report Refresh Date</span></span>
- <span data-ttu-id="0b2e9-145">已发送</span><span class="sxs-lookup"><span data-stu-id="0b2e9-145">Send</span></span>
- <span data-ttu-id="0b2e9-146">已接收</span><span class="sxs-lookup"><span data-stu-id="0b2e9-146">Receive</span></span>
- <span data-ttu-id="0b2e9-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="0b2e9-147">Read</span></span>
- <span data-ttu-id="0b2e9-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="0b2e9-148">Report Date</span></span>
- <span data-ttu-id="0b2e9-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="0b2e9-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0b2e9-150">示例</span><span class="sxs-lookup"><span data-stu-id="0b2e9-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0b2e9-151">请求</span><span class="sxs-lookup"><span data-stu-id="0b2e9-151">Request</span></span>

<span data-ttu-id="0b2e9-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b2e9-153">C#</span><span class="sxs-lookup"><span data-stu-id="0b2e9-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b2e9-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b2e9-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b2e9-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b2e9-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0b2e9-156">Java</span><span class="sxs-lookup"><span data-stu-id="0b2e9-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b2e9-157">响应</span><span class="sxs-lookup"><span data-stu-id="0b2e9-157">Response</span></span>

<span data-ttu-id="0b2e9-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-158">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b2e9-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0b2e9-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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
