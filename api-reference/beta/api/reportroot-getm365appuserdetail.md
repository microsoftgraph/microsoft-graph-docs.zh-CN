---
title: reportRoot： getM365AppUserDetail
description: 获取一个报告，该报告提供有关用户已使用的应用和平台的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 196e8747254d2fdc1cdb0e97a53eb2fe8c6b78d1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050932"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="d35d1-103">reportRoot： getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="d35d1-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="d35d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d35d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d35d1-105">获取一个报告，该报告提供有关用户已使用的应用和平台的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d35d1-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="d35d1-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)Microsoft 365 应用版使用情况。</span><span class="sxs-lookup"><span data-stu-id="d35d1-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="d35d1-107">权限</span><span class="sxs-lookup"><span data-stu-id="d35d1-107">Permissions</span></span>

<span data-ttu-id="d35d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d35d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d35d1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d35d1-110">Permission type</span></span>                        | <span data-ttu-id="d35d1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d35d1-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d35d1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d35d1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d35d1-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d35d1-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="d35d1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d35d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d35d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d35d1-115">Not supported.</span></span>                              |
| <span data-ttu-id="d35d1-116">应用</span><span class="sxs-lookup"><span data-stu-id="d35d1-116">Application</span></span>                            | <span data-ttu-id="d35d1-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d35d1-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="d35d1-118">**注意：** 对于允许应用代表用户读取服务使用情况报表的委派权限，租户管理员必须为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d35d1-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d35d1-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="d35d1-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d35d1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d35d1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d35d1-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="d35d1-121">Function parameters</span></span>

<span data-ttu-id="d35d1-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d35d1-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d35d1-123">参数</span><span class="sxs-lookup"><span data-stu-id="d35d1-123">Parameter</span></span> | <span data-ttu-id="d35d1-124">类型</span><span class="sxs-lookup"><span data-stu-id="d35d1-124">Type</span></span>   | <span data-ttu-id="d35d1-125">说明</span><span class="sxs-lookup"><span data-stu-id="d35d1-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d35d1-126">period</span><span class="sxs-lookup"><span data-stu-id="d35d1-126">period</span></span>    | <span data-ttu-id="d35d1-127">string</span><span class="sxs-lookup"><span data-stu-id="d35d1-127">string</span></span> | <span data-ttu-id="d35d1-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d35d1-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d35d1-129">{period_value} 支持的值是 `D7` `D30` ：、、 `D90` 和 `D180` 。</span><span class="sxs-lookup"><span data-stu-id="d35d1-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="d35d1-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d35d1-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d35d1-131">date</span><span class="sxs-lookup"><span data-stu-id="d35d1-131">date</span></span>      | <span data-ttu-id="d35d1-132">Date</span><span class="sxs-lookup"><span data-stu-id="d35d1-132">Date</span></span>   | <span data-ttu-id="d35d1-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="d35d1-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d35d1-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="d35d1-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d35d1-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="d35d1-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="d35d1-136">**注意：** 你需要在 URL 中 `period` 设置 `date` 或 。</span><span class="sxs-lookup"><span data-stu-id="d35d1-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d35d1-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d35d1-137">Optional query parameters</span></span>

<span data-ttu-id="d35d1-138">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d35d1-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d35d1-139">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d35d1-139">The default output type is text/csv.</span></span> <span data-ttu-id="d35d1-140">但是，如果要指定输出类型，可以使用 OData 查询参数将默认输出设置为 `$format` text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d35d1-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d35d1-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="d35d1-141">Request headers</span></span>

| <span data-ttu-id="d35d1-142">名称</span><span class="sxs-lookup"><span data-stu-id="d35d1-142">Name</span></span>          | <span data-ttu-id="d35d1-143">说明</span><span class="sxs-lookup"><span data-stu-id="d35d1-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d35d1-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="d35d1-144">Authorization</span></span> | <span data-ttu-id="d35d1-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d35d1-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d35d1-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="d35d1-147">Request body</span></span>

<span data-ttu-id="d35d1-148">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="d35d1-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="d35d1-149">响应</span><span class="sxs-lookup"><span data-stu-id="d35d1-149">Response</span></span>

<span data-ttu-id="d35d1-150">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/intune-shared-report.md)代码和 report 对象。</span><span class="sxs-lookup"><span data-stu-id="d35d1-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="d35d1-151">报表数据包含在 **报表对象的 content\*\*\*\*属性中**。</span><span class="sxs-lookup"><span data-stu-id="d35d1-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="d35d1-152">CSV</span><span class="sxs-lookup"><span data-stu-id="d35d1-152">CSV</span></span>

<span data-ttu-id="d35d1-153">如果成功，请求 **content** 属性将返回响应，该响应会重定向到报告的预先验证的 `302 Found` 下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d35d1-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d35d1-154">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d35d1-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d35d1-155">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="d35d1-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d35d1-156">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="d35d1-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="d35d1-157">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d35d1-157">Report Refresh Date</span></span>
- <span data-ttu-id="d35d1-158">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d35d1-158">User Principal Name</span></span>
- <span data-ttu-id="d35d1-159">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="d35d1-159">Last Activation Date</span></span>
- <span data-ttu-id="d35d1-160">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d35d1-160">Last Activity Date</span></span>
- <span data-ttu-id="d35d1-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="d35d1-161">Report Period</span></span>
- <span data-ttu-id="d35d1-162">Windows</span><span class="sxs-lookup"><span data-stu-id="d35d1-162">Windows</span></span>
- <span data-ttu-id="d35d1-163">Mac</span><span class="sxs-lookup"><span data-stu-id="d35d1-163">Mac</span></span>
- <span data-ttu-id="d35d1-164">移动版</span><span class="sxs-lookup"><span data-stu-id="d35d1-164">Mobile</span></span>
- <span data-ttu-id="d35d1-165">Web</span><span class="sxs-lookup"><span data-stu-id="d35d1-165">Web</span></span>
- <span data-ttu-id="d35d1-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="d35d1-166">Outlook</span></span>
- <span data-ttu-id="d35d1-167">Word</span><span class="sxs-lookup"><span data-stu-id="d35d1-167">Word</span></span>
- <span data-ttu-id="d35d1-168">Excel</span><span class="sxs-lookup"><span data-stu-id="d35d1-168">Excel</span></span>
- <span data-ttu-id="d35d1-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="d35d1-169">PowerPoint</span></span>
- <span data-ttu-id="d35d1-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="d35d1-170">OneNote</span></span>
- <span data-ttu-id="d35d1-171">Teams</span><span class="sxs-lookup"><span data-stu-id="d35d1-171">Teams</span></span>
- <span data-ttu-id="d35d1-172">Outlook (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-172">Outlook (Windows)</span></span>
- <span data-ttu-id="d35d1-173">Word (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-173">Word (Windows)</span></span>
- <span data-ttu-id="d35d1-174">Excel (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-174">Excel (Windows)</span></span>
- <span data-ttu-id="d35d1-175">PowerPoint (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="d35d1-176">OneNote (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-176">OneNote (Windows)</span></span>
- <span data-ttu-id="d35d1-177">Teams (Windows) </span><span class="sxs-lookup"><span data-stu-id="d35d1-177">Teams (Windows)</span></span>
- <span data-ttu-id="d35d1-178">Outlook (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-178">Outlook (Mac)</span></span>
- <span data-ttu-id="d35d1-179">Word (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-179">Word (Mac)</span></span>
- <span data-ttu-id="d35d1-180">Excel (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-180">Excel (Mac)</span></span>
- <span data-ttu-id="d35d1-181">PowerPoint (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="d35d1-182">OneNote (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-182">OneNote (Mac)</span></span>
- <span data-ttu-id="d35d1-183">Teams (Mac) </span><span class="sxs-lookup"><span data-stu-id="d35d1-183">Teams (Mac)</span></span>
- <span data-ttu-id="d35d1-184">Outlook (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="d35d1-185">Word (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-185">Word (Mobile)</span></span>
- <span data-ttu-id="d35d1-186">Excel (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-186">Excel (Mobile)</span></span>
- <span data-ttu-id="d35d1-187">PowerPoint (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="d35d1-188">OneNote (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="d35d1-189">Teams (Mobile) </span><span class="sxs-lookup"><span data-stu-id="d35d1-189">Teams (Mobile)</span></span>
- <span data-ttu-id="d35d1-190">Outlook (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-190">Outlook (Web)</span></span>
- <span data-ttu-id="d35d1-191">Word (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-191">Word (Web)</span></span>
- <span data-ttu-id="d35d1-192">Excel (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-192">Excel (Web)</span></span>
- <span data-ttu-id="d35d1-193">PowerPoint (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="d35d1-194">OneNote (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-194">OneNote (Web)</span></span>
- <span data-ttu-id="d35d1-195">Teams (Web) </span><span class="sxs-lookup"><span data-stu-id="d35d1-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="d35d1-196">JSON</span><span class="sxs-lookup"><span data-stu-id="d35d1-196">JSON</span></span>

<span data-ttu-id="d35d1-197">如果成功，请求 **content** 属性在响应正文中返回 响应代码和 `200 OK` JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d35d1-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="d35d1-198">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="d35d1-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="d35d1-199">示例</span><span class="sxs-lookup"><span data-stu-id="d35d1-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="d35d1-200">示例 1：CSV 输出</span><span class="sxs-lookup"><span data-stu-id="d35d1-200">Example 1: CSV output</span></span>

<span data-ttu-id="d35d1-201">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d35d1-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d35d1-202">请求</span><span class="sxs-lookup"><span data-stu-id="d35d1-202">Request</span></span>

<span data-ttu-id="d35d1-203">下面是请求获取 content 属性 **的示例** 。</span><span class="sxs-lookup"><span data-stu-id="d35d1-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="d35d1-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="d35d1-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="d35d1-205">C#</span><span class="sxs-lookup"><span data-stu-id="d35d1-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d35d1-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d35d1-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d35d1-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d35d1-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d35d1-208">Java</span><span class="sxs-lookup"><span data-stu-id="d35d1-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercoundetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="d35d1-209">响应</span><span class="sxs-lookup"><span data-stu-id="d35d1-209">Response</span></span>

<span data-ttu-id="d35d1-210">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d35d1-210">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d35d1-211">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d35d1-211">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="example-2-json-output"></a><span data-ttu-id="d35d1-212">示例 2：JSON 输出</span><span class="sxs-lookup"><span data-stu-id="d35d1-212">Example 2: JSON output</span></span>

<span data-ttu-id="d35d1-213">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d35d1-213">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d35d1-214">请求</span><span class="sxs-lookup"><span data-stu-id="d35d1-214">Request</span></span>

<span data-ttu-id="d35d1-215">下面是请求获取 content 属性 **的示例** 。</span><span class="sxs-lookup"><span data-stu-id="d35d1-215">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="d35d1-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="d35d1-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="d35d1-217">C#</span><span class="sxs-lookup"><span data-stu-id="d35d1-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d35d1-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d35d1-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d35d1-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d35d1-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d35d1-220">Java</span><span class="sxs-lookup"><span data-stu-id="d35d1-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercountdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="d35d1-221">响应</span><span class="sxs-lookup"><span data-stu-id="d35d1-221">Response</span></span>

<span data-ttu-id="d35d1-222">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d35d1-222">The following is an example of the response.</span></span>

> <span data-ttu-id="d35d1-223">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d35d1-223">**Note:** The response object shown here might be shortened for readability.</span></span>

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
