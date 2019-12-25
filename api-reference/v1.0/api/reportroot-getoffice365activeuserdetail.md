---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e1a57d5c2c8a1fbd3dec4a4cce61b026bd93a245
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865403"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="9839a-103">reportRoot：getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="9839a-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="9839a-104">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9839a-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="9839a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="9839a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="9839a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9839a-106">Permissions</span></span>

<span data-ttu-id="9839a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9839a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9839a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9839a-109">Permission type</span></span>                        | <span data-ttu-id="9839a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9839a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9839a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9839a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9839a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9839a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9839a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9839a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9839a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9839a-114">Not supported.</span></span>                           |
| <span data-ttu-id="9839a-115">应用</span><span class="sxs-lookup"><span data-stu-id="9839a-115">Application</span></span>                            | <span data-ttu-id="9839a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9839a-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="9839a-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9839a-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9839a-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="9839a-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9839a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9839a-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9839a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="9839a-120">Function parameters</span></span>

<span data-ttu-id="9839a-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="9839a-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9839a-122">参数</span><span class="sxs-lookup"><span data-stu-id="9839a-122">Parameter</span></span> | <span data-ttu-id="9839a-123">类型</span><span class="sxs-lookup"><span data-stu-id="9839a-123">Type</span></span>   | <span data-ttu-id="9839a-124">说明</span><span class="sxs-lookup"><span data-stu-id="9839a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9839a-125">period</span><span class="sxs-lookup"><span data-stu-id="9839a-125">period</span></span>    | <span data-ttu-id="9839a-126">string</span><span class="sxs-lookup"><span data-stu-id="9839a-126">string</span></span> | <span data-ttu-id="9839a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9839a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9839a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9839a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9839a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9839a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9839a-130">date</span><span class="sxs-lookup"><span data-stu-id="9839a-130">date</span></span>      | <span data-ttu-id="9839a-131">Date</span><span class="sxs-lookup"><span data-stu-id="9839a-131">Date</span></span>   | <span data-ttu-id="9839a-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="9839a-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9839a-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="9839a-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9839a-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="9839a-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9839a-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="9839a-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9839a-136">请求头</span><span class="sxs-lookup"><span data-stu-id="9839a-136">Request headers</span></span>

| <span data-ttu-id="9839a-137">名称</span><span class="sxs-lookup"><span data-stu-id="9839a-137">Name</span></span>          | <span data-ttu-id="9839a-138">说明</span><span class="sxs-lookup"><span data-stu-id="9839a-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9839a-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="9839a-139">Authorization</span></span> | <span data-ttu-id="9839a-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="9839a-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9839a-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9839a-142">If-None-Match</span></span> | <span data-ttu-id="9839a-143">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9839a-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9839a-144">可选。</span><span class="sxs-lookup"><span data-stu-id="9839a-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9839a-145">响应</span><span class="sxs-lookup"><span data-stu-id="9839a-145">Response</span></span>

<span data-ttu-id="9839a-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9839a-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9839a-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9839a-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9839a-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9839a-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9839a-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9839a-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9839a-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9839a-150">Report Refresh Date</span></span>
- <span data-ttu-id="9839a-151">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9839a-151">User Principal Name</span></span>
- <span data-ttu-id="9839a-152">显示名称</span><span class="sxs-lookup"><span data-stu-id="9839a-152">Display Name</span></span>
- <span data-ttu-id="9839a-153">已删除</span><span class="sxs-lookup"><span data-stu-id="9839a-153">Is Deleted</span></span>
- <span data-ttu-id="9839a-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="9839a-154">Deleted Date</span></span>
- <span data-ttu-id="9839a-155">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-155">Has Exchange License</span></span>
- <span data-ttu-id="9839a-156">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-156">Has OneDrive License</span></span>
- <span data-ttu-id="9839a-157">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-157">Has SharePoint License</span></span>
- <span data-ttu-id="9839a-158">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-158">Has Skype For Business License</span></span>
- <span data-ttu-id="9839a-159">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-159">Has Yammer License</span></span>
- <span data-ttu-id="9839a-160">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="9839a-160">Has Teams License</span></span>
- <span data-ttu-id="9839a-161">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-161">Exchange Last Activity Date</span></span>
- <span data-ttu-id="9839a-162">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-162">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="9839a-163">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-163">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="9839a-164">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-164">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="9839a-165">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-165">Yammer Last Activity Date</span></span>
- <span data-ttu-id="9839a-166">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9839a-166">Teams Last Activity Date</span></span>
- <span data-ttu-id="9839a-167">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-167">Exchange License Assign Date</span></span>
- <span data-ttu-id="9839a-168">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-168">OneDrive License Assign Date</span></span>
- <span data-ttu-id="9839a-169">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-169">SharePoint License Assign Date</span></span>
- <span data-ttu-id="9839a-170">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-170">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="9839a-171">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-171">Yammer License Assign Date</span></span>
- <span data-ttu-id="9839a-172">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="9839a-172">Teams License Assign Date</span></span>
- <span data-ttu-id="9839a-173">分配的产品</span><span class="sxs-lookup"><span data-stu-id="9839a-173">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="9839a-174">示例</span><span class="sxs-lookup"><span data-stu-id="9839a-174">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9839a-175">请求</span><span class="sxs-lookup"><span data-stu-id="9839a-175">Request</span></span>

<span data-ttu-id="9839a-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9839a-176">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9839a-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="9839a-177">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9839a-178">C#</span><span class="sxs-lookup"><span data-stu-id="9839a-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9839a-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9839a-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9839a-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9839a-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9839a-181">Java</span><span class="sxs-lookup"><span data-stu-id="9839a-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9839a-182">响应</span><span class="sxs-lookup"><span data-stu-id="9839a-182">Response</span></span>

<span data-ttu-id="9839a-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9839a-183">The following is an example of the response.</span></span>

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

<span data-ttu-id="9839a-184">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9839a-184">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
