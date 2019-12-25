---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 95220bec57c6c71518b94c130e6b8c8671ef321b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867328"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="925fa-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="925fa-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="925fa-105">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="925fa-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="925fa-106">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="925fa-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="925fa-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="925fa-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="925fa-108">权限</span><span class="sxs-lookup"><span data-stu-id="925fa-108">Permissions</span></span>

<span data-ttu-id="925fa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="925fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="925fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="925fa-111">Permission type</span></span>                        | <span data-ttu-id="925fa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="925fa-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="925fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="925fa-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="925fa-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="925fa-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="925fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="925fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="925fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="925fa-116">Not supported.</span></span>                           |
| <span data-ttu-id="925fa-117">应用</span><span class="sxs-lookup"><span data-stu-id="925fa-117">Application</span></span>                            | <span data-ttu-id="925fa-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="925fa-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="925fa-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="925fa-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="925fa-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="925fa-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="925fa-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="925fa-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="925fa-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="925fa-122">Function parameters</span></span>

<span data-ttu-id="925fa-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="925fa-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="925fa-124">参数</span><span class="sxs-lookup"><span data-stu-id="925fa-124">Parameter</span></span> | <span data-ttu-id="925fa-125">类型</span><span class="sxs-lookup"><span data-stu-id="925fa-125">Type</span></span>   | <span data-ttu-id="925fa-126">说明</span><span class="sxs-lookup"><span data-stu-id="925fa-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="925fa-127">period</span><span class="sxs-lookup"><span data-stu-id="925fa-127">period</span></span>    | <span data-ttu-id="925fa-128">string</span><span class="sxs-lookup"><span data-stu-id="925fa-128">string</span></span> | <span data-ttu-id="925fa-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="925fa-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="925fa-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="925fa-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="925fa-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="925fa-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="925fa-132">必需。</span><span class="sxs-lookup"><span data-stu-id="925fa-132">Required.</span></span> |

<span data-ttu-id="925fa-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="925fa-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="925fa-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="925fa-134">The default output type is text/csv.</span></span> <span data-ttu-id="925fa-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="925fa-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="925fa-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="925fa-136">Request headers</span></span>

| <span data-ttu-id="925fa-137">名称</span><span class="sxs-lookup"><span data-stu-id="925fa-137">Name</span></span>          | <span data-ttu-id="925fa-138">说明</span><span class="sxs-lookup"><span data-stu-id="925fa-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="925fa-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="925fa-139">Authorization</span></span> | <span data-ttu-id="925fa-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="925fa-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="925fa-142">响应</span><span class="sxs-lookup"><span data-stu-id="925fa-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="925fa-143">CSV</span><span class="sxs-lookup"><span data-stu-id="925fa-143">CSV</span></span>

<span data-ttu-id="925fa-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="925fa-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="925fa-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="925fa-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="925fa-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="925fa-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="925fa-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="925fa-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="925fa-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="925fa-148">Report Refresh Date</span></span>
- <span data-ttu-id="925fa-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="925fa-149">Report Date</span></span>
- <span data-ttu-id="925fa-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="925fa-150">Report Period</span></span>
- <span data-ttu-id="925fa-151">IM</span><span class="sxs-lookup"><span data-stu-id="925fa-151">IM</span></span>
- <span data-ttu-id="925fa-152">音频/视频</span><span class="sxs-lookup"><span data-stu-id="925fa-152">Audio/Video</span></span>
- <span data-ttu-id="925fa-153">应用共享</span><span class="sxs-lookup"><span data-stu-id="925fa-153">App Sharing</span></span>
- <span data-ttu-id="925fa-154">Web</span><span class="sxs-lookup"><span data-stu-id="925fa-154">Web</span></span>
- <span data-ttu-id="925fa-155">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="925fa-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="925fa-156">JSON</span><span class="sxs-lookup"><span data-stu-id="925fa-156">JSON</span></span>

<span data-ttu-id="925fa-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="925fa-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="925fa-158">示例</span><span class="sxs-lookup"><span data-stu-id="925fa-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="925fa-159">CSV</span><span class="sxs-lookup"><span data-stu-id="925fa-159">CSV</span></span>

<span data-ttu-id="925fa-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="925fa-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="925fa-161">请求</span><span class="sxs-lookup"><span data-stu-id="925fa-161">Request</span></span>

<span data-ttu-id="925fa-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="925fa-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="925fa-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="925fa-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="925fa-164">C#</span><span class="sxs-lookup"><span data-stu-id="925fa-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="925fa-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="925fa-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="925fa-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="925fa-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="925fa-167">响应</span><span class="sxs-lookup"><span data-stu-id="925fa-167">Response</span></span>

<span data-ttu-id="925fa-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="925fa-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="925fa-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="925fa-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="925fa-170">JSON</span><span class="sxs-lookup"><span data-stu-id="925fa-170">JSON</span></span>

<span data-ttu-id="925fa-171">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="925fa-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="925fa-172">请求</span><span class="sxs-lookup"><span data-stu-id="925fa-172">Request</span></span>

<span data-ttu-id="925fa-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="925fa-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="925fa-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="925fa-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="925fa-175">C#</span><span class="sxs-lookup"><span data-stu-id="925fa-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="925fa-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="925fa-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="925fa-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="925fa-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="925fa-178">响应</span><span class="sxs-lookup"><span data-stu-id="925fa-178">Response</span></span>

<span data-ttu-id="925fa-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="925fa-179">The following is an example of the response.</span></span>

> <span data-ttu-id="925fa-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="925fa-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
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
