---
title: reportRoot： getM365AppUserDetail
description: 获取提供有关用户已使用的应用程序和平台的详细信息的报告。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7940a4fed4b11d54e9dddf98b192346eb184c698
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975980"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="63f35-103">reportRoot： getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="63f35-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="63f35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63f35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63f35-105">获取提供有关用户已使用的应用程序和平台的详细信息的报告。</span><span class="sxs-lookup"><span data-stu-id="63f35-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="63f35-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [microsoft 365 报表-microsoft 365 应用程序使用](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)。</span><span class="sxs-lookup"><span data-stu-id="63f35-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="63f35-107">权限</span><span class="sxs-lookup"><span data-stu-id="63f35-107">Permissions</span></span>

<span data-ttu-id="63f35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63f35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63f35-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63f35-110">Permission type</span></span>                        | <span data-ttu-id="63f35-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63f35-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="63f35-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63f35-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="63f35-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63f35-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="63f35-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63f35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f35-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63f35-115">Not supported.</span></span>                              |
| <span data-ttu-id="63f35-116">应用</span><span class="sxs-lookup"><span data-stu-id="63f35-116">Application</span></span>                            | <span data-ttu-id="63f35-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63f35-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="63f35-118">**注意：** 为使应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="63f35-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="63f35-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="63f35-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="63f35-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63f35-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="63f35-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="63f35-121">Function parameters</span></span>

<span data-ttu-id="63f35-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="63f35-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="63f35-123">参数</span><span class="sxs-lookup"><span data-stu-id="63f35-123">Parameter</span></span> | <span data-ttu-id="63f35-124">类型</span><span class="sxs-lookup"><span data-stu-id="63f35-124">Type</span></span>   | <span data-ttu-id="63f35-125">说明</span><span class="sxs-lookup"><span data-stu-id="63f35-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="63f35-126">period</span><span class="sxs-lookup"><span data-stu-id="63f35-126">period</span></span>    | <span data-ttu-id="63f35-127">string</span><span class="sxs-lookup"><span data-stu-id="63f35-127">string</span></span> | <span data-ttu-id="63f35-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="63f35-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="63f35-129">{Period_value} 支持的值为： `D7` 、 `D30` 、 `D90` 、和 `D180` 。</span><span class="sxs-lookup"><span data-stu-id="63f35-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="63f35-130">这些值采用格式 D *n* ，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="63f35-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="63f35-131">date</span><span class="sxs-lookup"><span data-stu-id="63f35-131">date</span></span>      | <span data-ttu-id="63f35-132">Date</span><span class="sxs-lookup"><span data-stu-id="63f35-132">Date</span></span>   | <span data-ttu-id="63f35-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="63f35-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="63f35-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="63f35-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="63f35-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="63f35-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="63f35-136">**注意：** 您需要 `period` `date` 在 URL 中设置或。</span><span class="sxs-lookup"><span data-stu-id="63f35-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="63f35-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63f35-137">Optional query parameters</span></span>

<span data-ttu-id="63f35-138">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63f35-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="63f35-139">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="63f35-139">The default output type is text/csv.</span></span> <span data-ttu-id="63f35-140">但是，如果要指定输出类型，则可以使用 OData `$format` 查询参数将默认输出设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="63f35-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63f35-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="63f35-141">Request headers</span></span>

| <span data-ttu-id="63f35-142">名称</span><span class="sxs-lookup"><span data-stu-id="63f35-142">Name</span></span>          | <span data-ttu-id="63f35-143">说明</span><span class="sxs-lookup"><span data-stu-id="63f35-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="63f35-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="63f35-144">Authorization</span></span> | <span data-ttu-id="63f35-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63f35-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63f35-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="63f35-147">Request body</span></span>

<span data-ttu-id="63f35-148">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="63f35-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="63f35-149">响应</span><span class="sxs-lookup"><span data-stu-id="63f35-149">Response</span></span>

<span data-ttu-id="63f35-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [report](../resources/intune-shared-report.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63f35-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="63f35-151">报告数据包含在 **report** 对象的 **content** 属性中。</span><span class="sxs-lookup"><span data-stu-id="63f35-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="63f35-152">CSV</span><span class="sxs-lookup"><span data-stu-id="63f35-152">CSV</span></span>

<span data-ttu-id="63f35-153">如果成功，请求 **content** 属性将返回一个 `302 Found` 响应，该响应将重定向到报告的 preauthenticated 下载 URL。</span><span class="sxs-lookup"><span data-stu-id="63f35-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="63f35-154">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="63f35-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="63f35-155">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="63f35-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="63f35-156">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="63f35-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="63f35-157">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="63f35-157">Report Refresh Date</span></span>
- <span data-ttu-id="63f35-158">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="63f35-158">User Principal Name</span></span>
- <span data-ttu-id="63f35-159">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="63f35-159">Last Activation Date</span></span>
- <span data-ttu-id="63f35-160">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="63f35-160">Last Activity Date</span></span>
- <span data-ttu-id="63f35-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="63f35-161">Report Period</span></span>
- <span data-ttu-id="63f35-162">Windows</span><span class="sxs-lookup"><span data-stu-id="63f35-162">Windows</span></span>
- <span data-ttu-id="63f35-163">Mac</span><span class="sxs-lookup"><span data-stu-id="63f35-163">Mac</span></span>
- <span data-ttu-id="63f35-164">移动版</span><span class="sxs-lookup"><span data-stu-id="63f35-164">Mobile</span></span>
- <span data-ttu-id="63f35-165">Web</span><span class="sxs-lookup"><span data-stu-id="63f35-165">Web</span></span>
- <span data-ttu-id="63f35-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="63f35-166">Outlook</span></span>
- <span data-ttu-id="63f35-167">Word</span><span class="sxs-lookup"><span data-stu-id="63f35-167">Word</span></span>
- <span data-ttu-id="63f35-168">Excel</span><span class="sxs-lookup"><span data-stu-id="63f35-168">Excel</span></span>
- <span data-ttu-id="63f35-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="63f35-169">PowerPoint</span></span>
- <span data-ttu-id="63f35-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="63f35-170">OneNote</span></span>
- <span data-ttu-id="63f35-171">Teams</span><span class="sxs-lookup"><span data-stu-id="63f35-171">Teams</span></span>
- <span data-ttu-id="63f35-172">Outlook (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-172">Outlook (Windows)</span></span>
- <span data-ttu-id="63f35-173">Word (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-173">Word (Windows)</span></span>
- <span data-ttu-id="63f35-174">Excel (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-174">Excel (Windows)</span></span>
- <span data-ttu-id="63f35-175">PowerPoint (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="63f35-176">OneNote (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-176">OneNote (Windows)</span></span>
- <span data-ttu-id="63f35-177">团队 (Windows) </span><span class="sxs-lookup"><span data-stu-id="63f35-177">Teams (Windows)</span></span>
- <span data-ttu-id="63f35-178">Outlook (Mac) </span><span class="sxs-lookup"><span data-stu-id="63f35-178">Outlook (Mac)</span></span>
- <span data-ttu-id="63f35-179">Word (Mac) </span><span class="sxs-lookup"><span data-stu-id="63f35-179">Word (Mac)</span></span>
- <span data-ttu-id="63f35-180">Excel (Mac) </span><span class="sxs-lookup"><span data-stu-id="63f35-180">Excel (Mac)</span></span>
- <span data-ttu-id="63f35-181">PowerPoint (Mac) </span><span class="sxs-lookup"><span data-stu-id="63f35-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="63f35-182">OneNote (Mac) </span><span class="sxs-lookup"><span data-stu-id="63f35-182">OneNote (Mac)</span></span>
- <span data-ttu-id="63f35-183"> (Mac) 的团队</span><span class="sxs-lookup"><span data-stu-id="63f35-183">Teams (Mac)</span></span>
- <span data-ttu-id="63f35-184">Outlook (移动) </span><span class="sxs-lookup"><span data-stu-id="63f35-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="63f35-185">Word (移动) </span><span class="sxs-lookup"><span data-stu-id="63f35-185">Word (Mobile)</span></span>
- <span data-ttu-id="63f35-186">Excel (移动) </span><span class="sxs-lookup"><span data-stu-id="63f35-186">Excel (Mobile)</span></span>
- <span data-ttu-id="63f35-187">PowerPoint (移动) </span><span class="sxs-lookup"><span data-stu-id="63f35-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="63f35-188">OneNote (移动) </span><span class="sxs-lookup"><span data-stu-id="63f35-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="63f35-189"> (移动) 的团队</span><span class="sxs-lookup"><span data-stu-id="63f35-189">Teams (Mobile)</span></span>
- <span data-ttu-id="63f35-190">Outlook (Web) </span><span class="sxs-lookup"><span data-stu-id="63f35-190">Outlook (Web)</span></span>
- <span data-ttu-id="63f35-191">Word (Web) </span><span class="sxs-lookup"><span data-stu-id="63f35-191">Word (Web)</span></span>
- <span data-ttu-id="63f35-192">Excel (Web) </span><span class="sxs-lookup"><span data-stu-id="63f35-192">Excel (Web)</span></span>
- <span data-ttu-id="63f35-193">PowerPoint (Web) </span><span class="sxs-lookup"><span data-stu-id="63f35-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="63f35-194">OneNote (Web) </span><span class="sxs-lookup"><span data-stu-id="63f35-194">OneNote (Web)</span></span>
- <span data-ttu-id="63f35-195"> (Web) 的团队</span><span class="sxs-lookup"><span data-stu-id="63f35-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="63f35-196">JSON</span><span class="sxs-lookup"><span data-stu-id="63f35-196">JSON</span></span>

<span data-ttu-id="63f35-197">如果成功，请求 **content** 属性将 `200 OK` 在响应正文中返回响应代码和 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="63f35-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="63f35-198">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="63f35-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="63f35-199">示例</span><span class="sxs-lookup"><span data-stu-id="63f35-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="63f35-200">示例1： CSV 输出</span><span class="sxs-lookup"><span data-stu-id="63f35-200">Example 1: CSV output</span></span>

<span data-ttu-id="63f35-201">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="63f35-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="63f35-202">请求</span><span class="sxs-lookup"><span data-stu-id="63f35-202">Request</span></span>

<span data-ttu-id="63f35-203">下面的示例显示了获取 **内容** 属性的请求。</span><span class="sxs-lookup"><span data-stu-id="63f35-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="63f35-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="63f35-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="63f35-205">C#</span><span class="sxs-lookup"><span data-stu-id="63f35-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63f35-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63f35-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63f35-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63f35-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63f35-208">Java</span><span class="sxs-lookup"><span data-stu-id="63f35-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercoundetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="63f35-209">响应</span><span class="sxs-lookup"><span data-stu-id="63f35-209">Response</span></span>

<span data-ttu-id="63f35-210">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f35-210">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="63f35-211">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="63f35-211">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activation Date,Last Activity Date,Report Period,Windows,Mac,Mobile,Web,Outlook,Word,Excel,PowerPoint,OneNote,Teams,Outlook (Windows),Word (Windows),Excel (Windows),PowerPoint (Windows),OneNote (Windows),Teams (Windows),Outlook (Mac),Word (Mac),Excel (Mac),PowerPoint (Mac),OneNote (Mac),Teams (Mac),Outlook (Mobile),Word (Mobile),Excel (Mobile),PowerPoint (Mobile),OneNote (Mobile),Teams (Mobile),Outlook (Web),Word (Web),Excel (Web),PowerPoint (Web),OneNote (Web),Teams (Web)
```

### <a name="example-2-json-output"></a><span data-ttu-id="63f35-212">示例2： JSON 输出</span><span class="sxs-lookup"><span data-stu-id="63f35-212">Example 2: JSON output</span></span>

<span data-ttu-id="63f35-213">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="63f35-213">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="63f35-214">请求</span><span class="sxs-lookup"><span data-stu-id="63f35-214">Request</span></span>

<span data-ttu-id="63f35-215">下面的示例显示了获取 **内容** 属性的请求。</span><span class="sxs-lookup"><span data-stu-id="63f35-215">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="63f35-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="63f35-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="63f35-217">C#</span><span class="sxs-lookup"><span data-stu-id="63f35-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63f35-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63f35-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63f35-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63f35-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63f35-220">Java</span><span class="sxs-lookup"><span data-stu-id="63f35-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercountdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="63f35-221">响应</span><span class="sxs-lookup"><span data-stu-id="63f35-221">Response</span></span>

<span data-ttu-id="63f35-222">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f35-222">The following is an example of the response.</span></span>

> <span data-ttu-id="63f35-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63f35-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.nextLink": "https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json&$skiptoken=AAAAA",
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "userPrincipalName": "admin@contoso.com",
      "lastActivationDate": "2020-05-22",
      "lastActivityDate": "2020-06-30",
      "details": [
        {
          "reportPeriod": 7,
          "windows": true,
          "mac": false,
          "mobile": true,
          "web": false,
          "outlook": false,
          "word": false,
          "excel": false,
          "powerPoint": false,
          "oneNote": false,
          "teams": true,
          "outlookWindows": false,
          "wordWindows": false,
          "excelWindows": false,
          "powerPointWindows": false,
          "oneNoteWindows": false,
          "teamsWindows": true,
          "outlookMac": false,
          "wordMac": false,
          "excelMac": false,
          "powerPointMac": false,
          "oneNoteMac": false,
          "teamsMac": false,
          "outlookMobile": false,
          "wordMobile": false,
          "excelMobile": false,
          "powerPointMobile": false,
          "oneNoteMobile": false,
          "teamsMobile": true,
          "outlookWeb": false,
          "wordWeb": false,
          "excelWeb": false,
          "powerPointWeb": false,
          "oneNoteWeb": false,
          "teamsWeb": true
        }
      ]
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
