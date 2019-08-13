---
title: 'reportRoot: getEmailActivityUserCounts'
description: 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 33b9b1374a4b48fefde74df49b8e444a0266b931
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327425"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="64d9b-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="64d9b-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="64d9b-104">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="64d9b-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="64d9b-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="64d9b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="64d9b-106">权限</span><span class="sxs-lookup"><span data-stu-id="64d9b-106">Permissions</span></span>

<span data-ttu-id="64d9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64d9b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64d9b-109">Permission type</span></span>                        | <span data-ttu-id="64d9b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64d9b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64d9b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64d9b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64d9b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d9b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64d9b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64d9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64d9b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64d9b-114">Not supported.</span></span>                           |
| <span data-ttu-id="64d9b-115">应用</span><span class="sxs-lookup"><span data-stu-id="64d9b-115">Application</span></span>                            | <span data-ttu-id="64d9b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64d9b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="64d9b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64d9b-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="64d9b-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="64d9b-118">Function parameters</span></span>

<span data-ttu-id="64d9b-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="64d9b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="64d9b-120">参数</span><span class="sxs-lookup"><span data-stu-id="64d9b-120">Parameter</span></span> | <span data-ttu-id="64d9b-121">类型</span><span class="sxs-lookup"><span data-stu-id="64d9b-121">Type</span></span>   | <span data-ttu-id="64d9b-122">说明</span><span class="sxs-lookup"><span data-stu-id="64d9b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="64d9b-123">period</span><span class="sxs-lookup"><span data-stu-id="64d9b-123">period</span></span>    | <span data-ttu-id="64d9b-124">string</span><span class="sxs-lookup"><span data-stu-id="64d9b-124">string</span></span> | <span data-ttu-id="64d9b-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="64d9b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="64d9b-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="64d9b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="64d9b-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="64d9b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="64d9b-128">必需。</span><span class="sxs-lookup"><span data-stu-id="64d9b-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="64d9b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="64d9b-129">Request headers</span></span>

| <span data-ttu-id="64d9b-130">名称</span><span class="sxs-lookup"><span data-stu-id="64d9b-130">Name</span></span>          | <span data-ttu-id="64d9b-131">说明</span><span class="sxs-lookup"><span data-stu-id="64d9b-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="64d9b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d9b-132">Authorization</span></span> | <span data-ttu-id="64d9b-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="64d9b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="64d9b-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="64d9b-135">If-None-Match</span></span> | <span data-ttu-id="64d9b-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="64d9b-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="64d9b-137">可选。</span><span class="sxs-lookup"><span data-stu-id="64d9b-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="64d9b-138">响应</span><span class="sxs-lookup"><span data-stu-id="64d9b-138">Response</span></span>

<span data-ttu-id="64d9b-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="64d9b-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64d9b-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="64d9b-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64d9b-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="64d9b-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64d9b-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="64d9b-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64d9b-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="64d9b-143">Report Refresh Date</span></span>
- <span data-ttu-id="64d9b-144">已发送</span><span class="sxs-lookup"><span data-stu-id="64d9b-144">Send</span></span>
- <span data-ttu-id="64d9b-145">已接收</span><span class="sxs-lookup"><span data-stu-id="64d9b-145">Receive</span></span>
- <span data-ttu-id="64d9b-146">已阅读</span><span class="sxs-lookup"><span data-stu-id="64d9b-146">Read</span></span>
- <span data-ttu-id="64d9b-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="64d9b-147">Report Date</span></span>
- <span data-ttu-id="64d9b-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="64d9b-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="64d9b-149">示例</span><span class="sxs-lookup"><span data-stu-id="64d9b-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="64d9b-150">请求</span><span class="sxs-lookup"><span data-stu-id="64d9b-150">Request</span></span>

<span data-ttu-id="64d9b-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64d9b-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64d9b-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="64d9b-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64d9b-153">C#</span><span class="sxs-lookup"><span data-stu-id="64d9b-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64d9b-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64d9b-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64d9b-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="64d9b-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64d9b-156">Java</span><span class="sxs-lookup"><span data-stu-id="64d9b-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64d9b-157">响应</span><span class="sxs-lookup"><span data-stu-id="64d9b-157">Response</span></span>

<span data-ttu-id="64d9b-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64d9b-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="64d9b-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="64d9b-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

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
