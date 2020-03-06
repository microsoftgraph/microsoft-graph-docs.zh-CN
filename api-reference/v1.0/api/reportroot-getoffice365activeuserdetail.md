---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9e5c28010aaed4aefd6d12b60fc16abde4fc1880
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510345"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="a65c2-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="a65c2-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="a65c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65c2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a65c2-105">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a65c2-105">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="a65c2-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="a65c2-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a65c2-107">权限</span><span class="sxs-lookup"><span data-stu-id="a65c2-107">Permissions</span></span>

<span data-ttu-id="a65c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a65c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a65c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a65c2-110">Permission type</span></span>                        | <span data-ttu-id="a65c2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a65c2-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a65c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a65c2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a65c2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a65c2-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a65c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a65c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a65c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a65c2-115">Not supported.</span></span>                           |
| <span data-ttu-id="a65c2-116">应用</span><span class="sxs-lookup"><span data-stu-id="a65c2-116">Application</span></span>                            | <span data-ttu-id="a65c2-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a65c2-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a65c2-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a65c2-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a65c2-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a65c2-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a65c2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a65c2-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a65c2-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="a65c2-121">Function parameters</span></span>

<span data-ttu-id="a65c2-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a65c2-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a65c2-123">参数</span><span class="sxs-lookup"><span data-stu-id="a65c2-123">Parameter</span></span> | <span data-ttu-id="a65c2-124">类型</span><span class="sxs-lookup"><span data-stu-id="a65c2-124">Type</span></span>   | <span data-ttu-id="a65c2-125">说明</span><span class="sxs-lookup"><span data-stu-id="a65c2-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a65c2-126">period</span><span class="sxs-lookup"><span data-stu-id="a65c2-126">period</span></span>    | <span data-ttu-id="a65c2-127">string</span><span class="sxs-lookup"><span data-stu-id="a65c2-127">string</span></span> | <span data-ttu-id="a65c2-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a65c2-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a65c2-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a65c2-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a65c2-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a65c2-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a65c2-131">date</span><span class="sxs-lookup"><span data-stu-id="a65c2-131">date</span></span>      | <span data-ttu-id="a65c2-132">Date</span><span class="sxs-lookup"><span data-stu-id="a65c2-132">Date</span></span>   | <span data-ttu-id="a65c2-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a65c2-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a65c2-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a65c2-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a65c2-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a65c2-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a65c2-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a65c2-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a65c2-137">请求头</span><span class="sxs-lookup"><span data-stu-id="a65c2-137">Request headers</span></span>

| <span data-ttu-id="a65c2-138">名称</span><span class="sxs-lookup"><span data-stu-id="a65c2-138">Name</span></span>          | <span data-ttu-id="a65c2-139">说明</span><span class="sxs-lookup"><span data-stu-id="a65c2-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a65c2-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="a65c2-140">Authorization</span></span> | <span data-ttu-id="a65c2-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="a65c2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a65c2-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a65c2-143">If-None-Match</span></span> | <span data-ttu-id="a65c2-144">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a65c2-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a65c2-145">可选。</span><span class="sxs-lookup"><span data-stu-id="a65c2-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a65c2-146">响应</span><span class="sxs-lookup"><span data-stu-id="a65c2-146">Response</span></span>

<span data-ttu-id="a65c2-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a65c2-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a65c2-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a65c2-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a65c2-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a65c2-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a65c2-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a65c2-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a65c2-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-151">Report Refresh Date</span></span>
- <span data-ttu-id="a65c2-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a65c2-152">User Principal Name</span></span>
- <span data-ttu-id="a65c2-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="a65c2-153">Display Name</span></span>
- <span data-ttu-id="a65c2-154">已删除</span><span class="sxs-lookup"><span data-stu-id="a65c2-154">Is Deleted</span></span>
- <span data-ttu-id="a65c2-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-155">Deleted Date</span></span>
- <span data-ttu-id="a65c2-156">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-156">Has Exchange License</span></span>
- <span data-ttu-id="a65c2-157">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-157">Has OneDrive License</span></span>
- <span data-ttu-id="a65c2-158">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-158">Has SharePoint License</span></span>
- <span data-ttu-id="a65c2-159">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-159">Has Skype For Business License</span></span>
- <span data-ttu-id="a65c2-160">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-160">Has Yammer License</span></span>
- <span data-ttu-id="a65c2-161">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="a65c2-161">Has Teams License</span></span>
- <span data-ttu-id="a65c2-162">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="a65c2-163">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="a65c2-164">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="a65c2-165">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="a65c2-166">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="a65c2-167">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="a65c2-168">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="a65c2-169">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="a65c2-170">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="a65c2-171">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="a65c2-172">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="a65c2-173">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="a65c2-173">Teams License Assign Date</span></span>
- <span data-ttu-id="a65c2-174">分配的产品</span><span class="sxs-lookup"><span data-stu-id="a65c2-174">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="a65c2-175">示例</span><span class="sxs-lookup"><span data-stu-id="a65c2-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a65c2-176">请求</span><span class="sxs-lookup"><span data-stu-id="a65c2-176">Request</span></span>

<span data-ttu-id="a65c2-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a65c2-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a65c2-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65c2-178">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="a65c2-179">C#</span><span class="sxs-lookup"><span data-stu-id="a65c2-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65c2-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65c2-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65c2-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65c2-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a65c2-182">Java</span><span class="sxs-lookup"><span data-stu-id="a65c2-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a65c2-183">响应</span><span class="sxs-lookup"><span data-stu-id="a65c2-183">Response</span></span>

<span data-ttu-id="a65c2-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a65c2-184">The following is an example of the response.</span></span>

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

<span data-ttu-id="a65c2-185">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a65c2-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
