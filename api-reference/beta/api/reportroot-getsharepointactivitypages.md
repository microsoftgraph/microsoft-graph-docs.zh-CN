---
title: 'reportRoot: getSharePointActivityPages'
description: 获取用户访问的唯一页面数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c0c08943a5ba387230241848e8797458337e3cac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454267"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="3cf49-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="3cf49-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="3cf49-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3cf49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cf49-105">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="3cf49-105">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="3cf49-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="3cf49-106">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf49-107">权限</span><span class="sxs-lookup"><span data-stu-id="3cf49-107">Permissions</span></span>

<span data-ttu-id="3cf49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cf49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cf49-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cf49-110">Permission type</span></span>                        | <span data-ttu-id="3cf49-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cf49-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3cf49-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cf49-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cf49-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cf49-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3cf49-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cf49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf49-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cf49-115">Not supported.</span></span>                           |
| <span data-ttu-id="3cf49-116">应用</span><span class="sxs-lookup"><span data-stu-id="3cf49-116">Application</span></span>                            | <span data-ttu-id="3cf49-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cf49-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3cf49-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3cf49-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3cf49-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3cf49-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3cf49-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cf49-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3cf49-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="3cf49-121">Function parameters</span></span>

<span data-ttu-id="3cf49-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3cf49-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3cf49-123">参数</span><span class="sxs-lookup"><span data-stu-id="3cf49-123">Parameter</span></span> | <span data-ttu-id="3cf49-124">类型</span><span class="sxs-lookup"><span data-stu-id="3cf49-124">Type</span></span>   | <span data-ttu-id="3cf49-125">说明</span><span class="sxs-lookup"><span data-stu-id="3cf49-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3cf49-126">period</span><span class="sxs-lookup"><span data-stu-id="3cf49-126">period</span></span>    | <span data-ttu-id="3cf49-127">string</span><span class="sxs-lookup"><span data-stu-id="3cf49-127">string</span></span> | <span data-ttu-id="3cf49-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3cf49-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3cf49-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3cf49-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3cf49-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3cf49-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3cf49-131">必需。</span><span class="sxs-lookup"><span data-stu-id="3cf49-131">Required.</span></span> |

<span data-ttu-id="3cf49-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cf49-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3cf49-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3cf49-133">The default output type is text/csv.</span></span> <span data-ttu-id="3cf49-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3cf49-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cf49-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cf49-135">Request headers</span></span>

| <span data-ttu-id="3cf49-136">名称</span><span class="sxs-lookup"><span data-stu-id="3cf49-136">Name</span></span>          | <span data-ttu-id="3cf49-137">说明</span><span class="sxs-lookup"><span data-stu-id="3cf49-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3cf49-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cf49-138">Authorization</span></span> | <span data-ttu-id="3cf49-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cf49-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3cf49-141">响应</span><span class="sxs-lookup"><span data-stu-id="3cf49-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3cf49-142">CSV</span><span class="sxs-lookup"><span data-stu-id="3cf49-142">CSV</span></span>

<span data-ttu-id="3cf49-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3cf49-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3cf49-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3cf49-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3cf49-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="3cf49-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3cf49-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="3cf49-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3cf49-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3cf49-147">Report Refresh Date</span></span>
- <span data-ttu-id="3cf49-148">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="3cf49-148">Visited Page Count</span></span>
- <span data-ttu-id="3cf49-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="3cf49-149">Report Date</span></span>
- <span data-ttu-id="3cf49-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="3cf49-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3cf49-151">JSON</span><span class="sxs-lookup"><span data-stu-id="3cf49-151">JSON</span></span>

<span data-ttu-id="3cf49-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[sharePointActivityPages](../resources/sharepointactivitypages.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3cf49-152">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf49-153">示例</span><span class="sxs-lookup"><span data-stu-id="3cf49-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3cf49-154">CSV</span><span class="sxs-lookup"><span data-stu-id="3cf49-154">CSV</span></span>

<span data-ttu-id="3cf49-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3cf49-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3cf49-156">请求</span><span class="sxs-lookup"><span data-stu-id="3cf49-156">Request</span></span>

<span data-ttu-id="3cf49-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cf49-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cf49-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf49-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="3cf49-159">C#</span><span class="sxs-lookup"><span data-stu-id="3cf49-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cf49-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cf49-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cf49-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cf49-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3cf49-162">响应</span><span class="sxs-lookup"><span data-stu-id="3cf49-162">Response</span></span>

<span data-ttu-id="3cf49-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3cf49-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3cf49-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3cf49-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="3cf49-165">JSON</span><span class="sxs-lookup"><span data-stu-id="3cf49-165">JSON</span></span>

<span data-ttu-id="3cf49-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3cf49-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3cf49-167">请求</span><span class="sxs-lookup"><span data-stu-id="3cf49-167">Request</span></span>

<span data-ttu-id="3cf49-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cf49-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3cf49-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cf49-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="3cf49-170">C#</span><span class="sxs-lookup"><span data-stu-id="3cf49-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cf49-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cf49-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cf49-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cf49-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3cf49-173">响应</span><span class="sxs-lookup"><span data-stu-id="3cf49-173">Response</span></span>

<span data-ttu-id="3cf49-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3cf49-174">The following is an example of the response.</span></span>

> <span data-ttu-id="3cf49-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3cf49-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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
