---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: 获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。 对等会话类型包括 IM、音频、视频、应用共享和文件传输。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6945558360a8574a0caf4d9e44f524c56f68920a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987983"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="a2407-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a2407-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2407-105">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="a2407-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="a2407-106">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="a2407-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="a2407-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="a2407-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2407-108">权限</span><span class="sxs-lookup"><span data-stu-id="a2407-108">Permissions</span></span>

<span data-ttu-id="a2407-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2407-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2407-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2407-111">Permission type</span></span>                        | <span data-ttu-id="a2407-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2407-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2407-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2407-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2407-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2407-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2407-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2407-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2407-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2407-116">Not supported.</span></span>                           |
| <span data-ttu-id="a2407-117">应用</span><span class="sxs-lookup"><span data-stu-id="a2407-117">Application</span></span>                            | <span data-ttu-id="a2407-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2407-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a2407-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2407-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a2407-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="a2407-120">Function parameters</span></span>

<span data-ttu-id="a2407-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a2407-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2407-122">参数</span><span class="sxs-lookup"><span data-stu-id="a2407-122">Parameter</span></span> | <span data-ttu-id="a2407-123">类型</span><span class="sxs-lookup"><span data-stu-id="a2407-123">Type</span></span>   | <span data-ttu-id="a2407-124">说明</span><span class="sxs-lookup"><span data-stu-id="a2407-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2407-125">period</span><span class="sxs-lookup"><span data-stu-id="a2407-125">period</span></span>    | <span data-ttu-id="a2407-126">string</span><span class="sxs-lookup"><span data-stu-id="a2407-126">string</span></span> | <span data-ttu-id="a2407-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2407-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2407-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a2407-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2407-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2407-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a2407-130">必需。</span><span class="sxs-lookup"><span data-stu-id="a2407-130">Required.</span></span> |

<span data-ttu-id="a2407-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2407-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2407-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a2407-132">The default output type is text/csv.</span></span> <span data-ttu-id="a2407-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a2407-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2407-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2407-134">Request headers</span></span>

| <span data-ttu-id="a2407-135">名称</span><span class="sxs-lookup"><span data-stu-id="a2407-135">Name</span></span>          | <span data-ttu-id="a2407-136">说明</span><span class="sxs-lookup"><span data-stu-id="a2407-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2407-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2407-137">Authorization</span></span> | <span data-ttu-id="a2407-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2407-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2407-140">响应</span><span class="sxs-lookup"><span data-stu-id="a2407-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2407-141">CSV</span><span class="sxs-lookup"><span data-stu-id="a2407-141">CSV</span></span>

<span data-ttu-id="a2407-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a2407-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2407-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a2407-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2407-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a2407-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2407-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a2407-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2407-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a2407-146">Report Refresh Date</span></span>
- <span data-ttu-id="a2407-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="a2407-147">Report Date</span></span>
- <span data-ttu-id="a2407-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="a2407-148">Report Period</span></span>
- <span data-ttu-id="a2407-149">IM</span><span class="sxs-lookup"><span data-stu-id="a2407-149">IM</span></span>
- <span data-ttu-id="a2407-150">音频</span><span class="sxs-lookup"><span data-stu-id="a2407-150">Audio</span></span>
- <span data-ttu-id="a2407-151">视频</span><span class="sxs-lookup"><span data-stu-id="a2407-151">Video</span></span>
- <span data-ttu-id="a2407-152">应用共享</span><span class="sxs-lookup"><span data-stu-id="a2407-152">App Sharing</span></span>
- <span data-ttu-id="a2407-153">文件传输</span><span class="sxs-lookup"><span data-stu-id="a2407-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="a2407-154">JSON</span><span class="sxs-lookup"><span data-stu-id="a2407-154">JSON</span></span>

<span data-ttu-id="a2407-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a2407-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2407-156">示例</span><span class="sxs-lookup"><span data-stu-id="a2407-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2407-157">CSV</span><span class="sxs-lookup"><span data-stu-id="a2407-157">CSV</span></span>

<span data-ttu-id="a2407-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2407-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2407-159">请求</span><span class="sxs-lookup"><span data-stu-id="a2407-159">Request</span></span>

<span data-ttu-id="a2407-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2407-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a2407-161">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a2407-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2407-162">C#</span><span class="sxs-lookup"><span data-stu-id="a2407-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2407-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2407-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2407-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="a2407-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a2407-165">Java</span><span class="sxs-lookup"><span data-stu-id="a2407-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a2407-166">响应</span><span class="sxs-lookup"><span data-stu-id="a2407-166">Response</span></span>

<span data-ttu-id="a2407-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2407-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a2407-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a2407-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="a2407-169">JSON</span><span class="sxs-lookup"><span data-stu-id="a2407-169">JSON</span></span>

<span data-ttu-id="a2407-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2407-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2407-171">请求</span><span class="sxs-lookup"><span data-stu-id="a2407-171">Request</span></span>

<span data-ttu-id="a2407-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2407-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a2407-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a2407-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2407-174">C#</span><span class="sxs-lookup"><span data-stu-id="a2407-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2407-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2407-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2407-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="a2407-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a2407-177">Java</span><span class="sxs-lookup"><span data-stu-id="a2407-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a2407-178">响应</span><span class="sxs-lookup"><span data-stu-id="a2407-178">Response</span></span>

<span data-ttu-id="a2407-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2407-179">The following is an example of the response.</span></span>

> <span data-ttu-id="a2407-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a2407-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts)", 
  "value": [
    {
      "im": 379, 
      "audio": 42, 
      "video": 2, 
      "appSharing": 34, 
      "fileTransfer": 36, 
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
