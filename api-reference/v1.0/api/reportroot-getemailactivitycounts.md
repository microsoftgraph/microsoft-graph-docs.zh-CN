---
title: 'reportRoot: getEmailActivityCounts'
description: 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 527936d1e51e982e8c483c318a7749aea805659a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864535"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="43052-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="43052-103">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="43052-104">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="43052-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="43052-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="43052-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="43052-106">权限</span><span class="sxs-lookup"><span data-stu-id="43052-106">Permissions</span></span>

<span data-ttu-id="43052-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43052-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="43052-109">Permission type</span></span>                        | <span data-ttu-id="43052-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43052-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="43052-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43052-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="43052-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43052-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="43052-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43052-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43052-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="43052-114">Not supported.</span></span>                           |
| <span data-ttu-id="43052-115">应用</span><span class="sxs-lookup"><span data-stu-id="43052-115">Application</span></span>                            | <span data-ttu-id="43052-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="43052-116">Reports.Read.All</span></span>                         |

> <span data-ttu-id="43052-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="43052-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="43052-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="43052-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="43052-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43052-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="43052-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="43052-120">Function parameters</span></span>

<span data-ttu-id="43052-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="43052-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="43052-122">参数</span><span class="sxs-lookup"><span data-stu-id="43052-122">Parameter</span></span> | <span data-ttu-id="43052-123">类型</span><span class="sxs-lookup"><span data-stu-id="43052-123">Type</span></span>   | <span data-ttu-id="43052-124">说明</span><span class="sxs-lookup"><span data-stu-id="43052-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="43052-125">period</span><span class="sxs-lookup"><span data-stu-id="43052-125">period</span></span>    | <span data-ttu-id="43052-126">string</span><span class="sxs-lookup"><span data-stu-id="43052-126">string</span></span> | <span data-ttu-id="43052-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="43052-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="43052-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="43052-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="43052-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="43052-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="43052-130">必需。</span><span class="sxs-lookup"><span data-stu-id="43052-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="43052-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="43052-131">Request headers</span></span>

| <span data-ttu-id="43052-132">名称</span><span class="sxs-lookup"><span data-stu-id="43052-132">Name</span></span>          | <span data-ttu-id="43052-133">说明</span><span class="sxs-lookup"><span data-stu-id="43052-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="43052-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="43052-134">Authorization</span></span> | <span data-ttu-id="43052-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="43052-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="43052-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="43052-137">If-None-Match</span></span> | <span data-ttu-id="43052-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="43052-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="43052-139">可选。</span><span class="sxs-lookup"><span data-stu-id="43052-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="43052-140">响应</span><span class="sxs-lookup"><span data-stu-id="43052-140">Response</span></span>

<span data-ttu-id="43052-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="43052-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="43052-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="43052-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="43052-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="43052-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="43052-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="43052-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="43052-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="43052-145">Report Refresh Date</span></span>
- <span data-ttu-id="43052-146">已发送</span><span class="sxs-lookup"><span data-stu-id="43052-146">Send</span></span>
- <span data-ttu-id="43052-147">已接收</span><span class="sxs-lookup"><span data-stu-id="43052-147">Receive</span></span>
- <span data-ttu-id="43052-148">已阅读</span><span class="sxs-lookup"><span data-stu-id="43052-148">Read</span></span>
- <span data-ttu-id="43052-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="43052-149">Report Date</span></span>
- <span data-ttu-id="43052-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="43052-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="43052-151">示例</span><span class="sxs-lookup"><span data-stu-id="43052-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="43052-152">请求</span><span class="sxs-lookup"><span data-stu-id="43052-152">Request</span></span>

<span data-ttu-id="43052-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="43052-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="43052-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="43052-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43052-155">C#</span><span class="sxs-lookup"><span data-stu-id="43052-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43052-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43052-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43052-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43052-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="43052-158">Java</span><span class="sxs-lookup"><span data-stu-id="43052-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="43052-159">响应</span><span class="sxs-lookup"><span data-stu-id="43052-159">Response</span></span>

<span data-ttu-id="43052-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="43052-160">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="43052-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="43052-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
