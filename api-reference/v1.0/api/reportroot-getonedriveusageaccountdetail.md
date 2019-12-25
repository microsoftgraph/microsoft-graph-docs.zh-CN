---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c73f4fe8f41a5fe57075cff8a61065f6104cdaf6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865375"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="7e02c-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="7e02c-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="7e02c-104">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7e02c-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="7e02c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="7e02c-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e02c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e02c-106">Permissions</span></span>

<span data-ttu-id="7e02c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e02c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e02c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e02c-109">Permission type</span></span>                        | <span data-ttu-id="7e02c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e02c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7e02c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e02c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e02c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e02c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7e02c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e02c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e02c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e02c-114">Not supported.</span></span>                           |
| <span data-ttu-id="7e02c-115">应用</span><span class="sxs-lookup"><span data-stu-id="7e02c-115">Application</span></span>                            | <span data-ttu-id="7e02c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e02c-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7e02c-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="7e02c-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7e02c-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="7e02c-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7e02c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e02c-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7e02c-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="7e02c-120">Function parameters</span></span>

<span data-ttu-id="7e02c-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7e02c-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7e02c-122">参数</span><span class="sxs-lookup"><span data-stu-id="7e02c-122">Parameter</span></span> | <span data-ttu-id="7e02c-123">类型</span><span class="sxs-lookup"><span data-stu-id="7e02c-123">Type</span></span>   | <span data-ttu-id="7e02c-124">说明</span><span class="sxs-lookup"><span data-stu-id="7e02c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7e02c-125">period</span><span class="sxs-lookup"><span data-stu-id="7e02c-125">period</span></span>    | <span data-ttu-id="7e02c-126">string</span><span class="sxs-lookup"><span data-stu-id="7e02c-126">string</span></span> | <span data-ttu-id="7e02c-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e02c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7e02c-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7e02c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7e02c-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e02c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7e02c-130">date</span><span class="sxs-lookup"><span data-stu-id="7e02c-130">date</span></span>      | <span data-ttu-id="7e02c-131">Date</span><span class="sxs-lookup"><span data-stu-id="7e02c-131">Date</span></span>   | <span data-ttu-id="7e02c-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="7e02c-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7e02c-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="7e02c-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7e02c-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="7e02c-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7e02c-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="7e02c-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e02c-136">请求头</span><span class="sxs-lookup"><span data-stu-id="7e02c-136">Request headers</span></span>

| <span data-ttu-id="7e02c-137">名称</span><span class="sxs-lookup"><span data-stu-id="7e02c-137">Name</span></span>          | <span data-ttu-id="7e02c-138">说明</span><span class="sxs-lookup"><span data-stu-id="7e02c-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7e02c-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e02c-139">Authorization</span></span> | <span data-ttu-id="7e02c-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e02c-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7e02c-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7e02c-142">If-None-Match</span></span> | <span data-ttu-id="7e02c-143">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7e02c-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7e02c-144">可选。</span><span class="sxs-lookup"><span data-stu-id="7e02c-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7e02c-145">响应</span><span class="sxs-lookup"><span data-stu-id="7e02c-145">Response</span></span>

<span data-ttu-id="7e02c-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7e02c-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7e02c-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7e02c-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7e02c-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7e02c-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7e02c-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7e02c-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7e02c-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7e02c-150">Report Refresh Date</span></span>
- <span data-ttu-id="7e02c-151">网站 URL</span><span class="sxs-lookup"><span data-stu-id="7e02c-151">Site URL</span></span>
- <span data-ttu-id="7e02c-152">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="7e02c-152">Owner Display Name</span></span>
- <span data-ttu-id="7e02c-153">已删除</span><span class="sxs-lookup"><span data-stu-id="7e02c-153">Is Deleted</span></span>
- <span data-ttu-id="7e02c-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7e02c-154">Last Activity Date</span></span>
- <span data-ttu-id="7e02c-155">文件数</span><span class="sxs-lookup"><span data-stu-id="7e02c-155">File Count</span></span>
- <span data-ttu-id="7e02c-156">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="7e02c-156">Active File Count</span></span>
- <span data-ttu-id="7e02c-157">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="7e02c-157">Storage Used (Byte)</span></span>
- <span data-ttu-id="7e02c-158">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="7e02c-158">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="7e02c-159">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="7e02c-159">Owner Principal Name</span></span>
- <span data-ttu-id="7e02c-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="7e02c-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7e02c-161">示例</span><span class="sxs-lookup"><span data-stu-id="7e02c-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e02c-162">请求</span><span class="sxs-lookup"><span data-stu-id="7e02c-162">Request</span></span>

<span data-ttu-id="7e02c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e02c-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e02c-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e02c-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e02c-165">C#</span><span class="sxs-lookup"><span data-stu-id="7e02c-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e02c-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e02c-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e02c-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e02c-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e02c-168">Java</span><span class="sxs-lookup"><span data-stu-id="7e02c-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e02c-169">响应</span><span class="sxs-lookup"><span data-stu-id="7e02c-169">Response</span></span>

<span data-ttu-id="7e02c-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e02c-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="7e02c-171">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7e02c-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
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
