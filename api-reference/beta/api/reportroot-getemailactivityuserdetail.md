---
title: 'reportRoot: getEmailActivityUserDetail'
description: 获取用户执行的电子邮件活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e3232d7108db73166e4396b8cbb7b95d72bb681f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454470"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="b2fed-103">reportRoot：getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b2fed-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="b2fed-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b2fed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2fed-105">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b2fed-105">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="b2fed-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="b2fed-106">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2fed-107">权限</span><span class="sxs-lookup"><span data-stu-id="b2fed-107">Permissions</span></span>

<span data-ttu-id="b2fed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2fed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2fed-110">Permission type</span></span>                        | <span data-ttu-id="b2fed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2fed-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b2fed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2fed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2fed-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2fed-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b2fed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2fed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2fed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2fed-115">Not supported.</span></span>                           |
| <span data-ttu-id="b2fed-116">应用</span><span class="sxs-lookup"><span data-stu-id="b2fed-116">Application</span></span>                            | <span data-ttu-id="b2fed-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2fed-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="b2fed-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="b2fed-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b2fed-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="b2fed-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b2fed-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2fed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b2fed-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="b2fed-121">Function parameters</span></span>

<span data-ttu-id="b2fed-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b2fed-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b2fed-123">参数</span><span class="sxs-lookup"><span data-stu-id="b2fed-123">Parameter</span></span> | <span data-ttu-id="b2fed-124">类型</span><span class="sxs-lookup"><span data-stu-id="b2fed-124">Type</span></span>   | <span data-ttu-id="b2fed-125">说明</span><span class="sxs-lookup"><span data-stu-id="b2fed-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b2fed-126">period</span><span class="sxs-lookup"><span data-stu-id="b2fed-126">period</span></span>    | <span data-ttu-id="b2fed-127">string</span><span class="sxs-lookup"><span data-stu-id="b2fed-127">string</span></span> | <span data-ttu-id="b2fed-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b2fed-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b2fed-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b2fed-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b2fed-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b2fed-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b2fed-131">date</span><span class="sxs-lookup"><span data-stu-id="b2fed-131">date</span></span>      | <span data-ttu-id="b2fed-132">Date</span><span class="sxs-lookup"><span data-stu-id="b2fed-132">Date</span></span>   | <span data-ttu-id="b2fed-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b2fed-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b2fed-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b2fed-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b2fed-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b2fed-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b2fed-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b2fed-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b2fed-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b2fed-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b2fed-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="b2fed-138">The default output type is text/csv.</span></span> <span data-ttu-id="b2fed-139">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="b2fed-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2fed-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2fed-140">Request headers</span></span>

| <span data-ttu-id="b2fed-141">名称</span><span class="sxs-lookup"><span data-stu-id="b2fed-141">Name</span></span>          | <span data-ttu-id="b2fed-142">说明</span><span class="sxs-lookup"><span data-stu-id="b2fed-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b2fed-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2fed-143">Authorization</span></span> | <span data-ttu-id="b2fed-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2fed-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b2fed-146">响应</span><span class="sxs-lookup"><span data-stu-id="b2fed-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b2fed-147">CSV</span><span class="sxs-lookup"><span data-stu-id="b2fed-147">CSV</span></span>

<span data-ttu-id="b2fed-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b2fed-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b2fed-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b2fed-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b2fed-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b2fed-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b2fed-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b2fed-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b2fed-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b2fed-152">Report Refresh Date</span></span>
- <span data-ttu-id="b2fed-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b2fed-153">User Principal Name</span></span>
- <span data-ttu-id="b2fed-154">显示名称</span><span class="sxs-lookup"><span data-stu-id="b2fed-154">Display Name</span></span>
- <span data-ttu-id="b2fed-155">已删除</span><span class="sxs-lookup"><span data-stu-id="b2fed-155">Is Deleted</span></span>
- <span data-ttu-id="b2fed-156">删除日期</span><span class="sxs-lookup"><span data-stu-id="b2fed-156">Deleted Date</span></span>
- <span data-ttu-id="b2fed-157">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b2fed-157">Last Activity Date</span></span>
- <span data-ttu-id="b2fed-158">已发送数</span><span class="sxs-lookup"><span data-stu-id="b2fed-158">Send Count</span></span>
- <span data-ttu-id="b2fed-159">已接收数</span><span class="sxs-lookup"><span data-stu-id="b2fed-159">Receive Count</span></span>
- <span data-ttu-id="b2fed-160">已阅读数</span><span class="sxs-lookup"><span data-stu-id="b2fed-160">Read Count</span></span>
- <span data-ttu-id="b2fed-161">分配的产品</span><span class="sxs-lookup"><span data-stu-id="b2fed-161">Assigned Products</span></span>
- <span data-ttu-id="b2fed-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="b2fed-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b2fed-163">JSON</span><span class="sxs-lookup"><span data-stu-id="b2fed-163">JSON</span></span>

<span data-ttu-id="b2fed-164">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b2fed-164">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b2fed-165">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="b2fed-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b2fed-166">示例</span><span class="sxs-lookup"><span data-stu-id="b2fed-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b2fed-167">CSV</span><span class="sxs-lookup"><span data-stu-id="b2fed-167">CSV</span></span>

<span data-ttu-id="b2fed-168">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="b2fed-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b2fed-169">请求</span><span class="sxs-lookup"><span data-stu-id="b2fed-169">Request</span></span>

<span data-ttu-id="b2fed-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2fed-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2fed-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2fed-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="b2fed-172">C#</span><span class="sxs-lookup"><span data-stu-id="b2fed-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2fed-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2fed-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2fed-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2fed-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b2fed-175">响应</span><span class="sxs-lookup"><span data-stu-id="b2fed-175">Response</span></span>

<span data-ttu-id="b2fed-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2fed-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b2fed-177">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b2fed-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="b2fed-178">JSON</span><span class="sxs-lookup"><span data-stu-id="b2fed-178">JSON</span></span>

<span data-ttu-id="b2fed-179">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b2fed-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b2fed-180">请求</span><span class="sxs-lookup"><span data-stu-id="b2fed-180">Request</span></span>

<span data-ttu-id="b2fed-181">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2fed-181">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2fed-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2fed-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="b2fed-183">C#</span><span class="sxs-lookup"><span data-stu-id="b2fed-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2fed-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2fed-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2fed-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2fed-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b2fed-186">响应</span><span class="sxs-lookup"><span data-stu-id="b2fed-186">Response</span></span>

<span data-ttu-id="b2fed-187">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b2fed-187">The following is an example of the response.</span></span>

> <span data-ttu-id="b2fed-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b2fed-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
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
