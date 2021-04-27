---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: c99f4b653a94586847a28cf4ed93989fbb8a3baf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049749"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="a2b47-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a2b47-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="a2b47-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2b47-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2b47-106">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a2b47-106">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a2b47-107">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="a2b47-107">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="a2b47-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="a2b47-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b47-109">权限</span><span class="sxs-lookup"><span data-stu-id="a2b47-109">Permissions</span></span>

<span data-ttu-id="a2b47-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2b47-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2b47-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2b47-112">Permission type</span></span>                        | <span data-ttu-id="a2b47-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2b47-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2b47-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b47-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2b47-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b47-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2b47-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b47-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b47-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b47-117">Not supported.</span></span>                           |
| <span data-ttu-id="a2b47-118">应用</span><span class="sxs-lookup"><span data-stu-id="a2b47-118">Application</span></span>                            | <span data-ttu-id="a2b47-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2b47-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="a2b47-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a2b47-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a2b47-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a2b47-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a2b47-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2b47-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a2b47-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="a2b47-123">Function parameters</span></span>

<span data-ttu-id="a2b47-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a2b47-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2b47-125">参数</span><span class="sxs-lookup"><span data-stu-id="a2b47-125">Parameter</span></span> | <span data-ttu-id="a2b47-126">类型</span><span class="sxs-lookup"><span data-stu-id="a2b47-126">Type</span></span>   | <span data-ttu-id="a2b47-127">说明</span><span class="sxs-lookup"><span data-stu-id="a2b47-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2b47-128">period</span><span class="sxs-lookup"><span data-stu-id="a2b47-128">period</span></span>    | <span data-ttu-id="a2b47-129">string</span><span class="sxs-lookup"><span data-stu-id="a2b47-129">string</span></span> | <span data-ttu-id="a2b47-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2b47-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2b47-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a2b47-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2b47-132">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2b47-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a2b47-133">必需。</span><span class="sxs-lookup"><span data-stu-id="a2b47-133">Required.</span></span> |

<span data-ttu-id="a2b47-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2b47-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2b47-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a2b47-135">The default output type is text/csv.</span></span> <span data-ttu-id="a2b47-136">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a2b47-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2b47-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2b47-137">Request headers</span></span>

| <span data-ttu-id="a2b47-138">名称</span><span class="sxs-lookup"><span data-stu-id="a2b47-138">Name</span></span>          | <span data-ttu-id="a2b47-139">说明</span><span class="sxs-lookup"><span data-stu-id="a2b47-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2b47-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b47-140">Authorization</span></span> | <span data-ttu-id="a2b47-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2b47-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2b47-143">响应</span><span class="sxs-lookup"><span data-stu-id="a2b47-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2b47-144">CSV</span><span class="sxs-lookup"><span data-stu-id="a2b47-144">CSV</span></span>

<span data-ttu-id="a2b47-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a2b47-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2b47-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a2b47-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2b47-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a2b47-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2b47-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a2b47-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2b47-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a2b47-149">Report Refresh Date</span></span>
- <span data-ttu-id="a2b47-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="a2b47-150">Report Date</span></span>
- <span data-ttu-id="a2b47-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="a2b47-151">Report Period</span></span>
- <span data-ttu-id="a2b47-152">对等</span><span class="sxs-lookup"><span data-stu-id="a2b47-152">Peer-to-peer</span></span>
- <span data-ttu-id="a2b47-153">组织</span><span class="sxs-lookup"><span data-stu-id="a2b47-153">Organized</span></span>
- <span data-ttu-id="a2b47-154">参与</span><span class="sxs-lookup"><span data-stu-id="a2b47-154">Participated</span></span>

### <a name="json"></a><span data-ttu-id="a2b47-155">JSON</span><span class="sxs-lookup"><span data-stu-id="a2b47-155">JSON</span></span>

<span data-ttu-id="a2b47-156">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a2b47-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b47-157">示例</span><span class="sxs-lookup"><span data-stu-id="a2b47-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2b47-158">CSV</span><span class="sxs-lookup"><span data-stu-id="a2b47-158">CSV</span></span>

<span data-ttu-id="a2b47-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2b47-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2b47-160">请求</span><span class="sxs-lookup"><span data-stu-id="a2b47-160">Request</span></span>

<span data-ttu-id="a2b47-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2b47-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a2b47-162">响应</span><span class="sxs-lookup"><span data-stu-id="a2b47-162">Response</span></span>

<span data-ttu-id="a2b47-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2b47-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a2b47-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a2b47-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="a2b47-165">JSON</span><span class="sxs-lookup"><span data-stu-id="a2b47-165">JSON</span></span>

<span data-ttu-id="a2b47-166">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2b47-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2b47-167">请求</span><span class="sxs-lookup"><span data-stu-id="a2b47-167">Request</span></span>

<span data-ttu-id="a2b47-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2b47-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a2b47-169">响应</span><span class="sxs-lookup"><span data-stu-id="a2b47-169">Response</span></span>

<span data-ttu-id="a2b47-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2b47-170">The following is an example of the response.</span></span>

> <span data-ttu-id="a2b47-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2b47-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
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


