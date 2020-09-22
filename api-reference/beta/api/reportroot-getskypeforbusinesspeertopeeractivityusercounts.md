---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: 获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。 对等会话类型包括 IM、音频、视频、应用共享和文件传输。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 42b0a1f58d17f2dd76a53107ea85dac70cf939c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053130"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="bf7aa-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="bf7aa-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="bf7aa-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf7aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf7aa-106">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-106">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="bf7aa-107">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-107">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="bf7aa-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 reports-Skype For business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf7aa-109">权限</span><span class="sxs-lookup"><span data-stu-id="bf7aa-109">Permissions</span></span>

<span data-ttu-id="bf7aa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf7aa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf7aa-112">Permission type</span></span>                        | <span data-ttu-id="bf7aa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf7aa-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bf7aa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf7aa-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf7aa-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf7aa-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bf7aa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf7aa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf7aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-117">Not supported.</span></span>                           |
| <span data-ttu-id="bf7aa-118">应用</span><span class="sxs-lookup"><span data-stu-id="bf7aa-118">Application</span></span>                            | <span data-ttu-id="bf7aa-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf7aa-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="bf7aa-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bf7aa-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bf7aa-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf7aa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bf7aa-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="bf7aa-123">Function parameters</span></span>

<span data-ttu-id="bf7aa-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bf7aa-125">参数</span><span class="sxs-lookup"><span data-stu-id="bf7aa-125">Parameter</span></span> | <span data-ttu-id="bf7aa-126">类型</span><span class="sxs-lookup"><span data-stu-id="bf7aa-126">Type</span></span>   | <span data-ttu-id="bf7aa-127">说明</span><span class="sxs-lookup"><span data-stu-id="bf7aa-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bf7aa-128">period</span><span class="sxs-lookup"><span data-stu-id="bf7aa-128">period</span></span>    | <span data-ttu-id="bf7aa-129">string</span><span class="sxs-lookup"><span data-stu-id="bf7aa-129">string</span></span> | <span data-ttu-id="bf7aa-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bf7aa-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bf7aa-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bf7aa-133">必需。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-133">Required.</span></span> |

<span data-ttu-id="bf7aa-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bf7aa-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-135">The default output type is text/csv.</span></span> <span data-ttu-id="bf7aa-136">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf7aa-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf7aa-137">Request headers</span></span>

| <span data-ttu-id="bf7aa-138">名称</span><span class="sxs-lookup"><span data-stu-id="bf7aa-138">Name</span></span>          | <span data-ttu-id="bf7aa-139">说明</span><span class="sxs-lookup"><span data-stu-id="bf7aa-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bf7aa-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf7aa-140">Authorization</span></span> | <span data-ttu-id="bf7aa-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bf7aa-143">响应</span><span class="sxs-lookup"><span data-stu-id="bf7aa-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bf7aa-144">CSV</span><span class="sxs-lookup"><span data-stu-id="bf7aa-144">CSV</span></span>

<span data-ttu-id="bf7aa-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bf7aa-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bf7aa-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bf7aa-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bf7aa-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bf7aa-149">Report Refresh Date</span></span>
- <span data-ttu-id="bf7aa-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="bf7aa-150">Report Date</span></span>
- <span data-ttu-id="bf7aa-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="bf7aa-151">Report Period</span></span>
- <span data-ttu-id="bf7aa-152">IM</span><span class="sxs-lookup"><span data-stu-id="bf7aa-152">IM</span></span>
- <span data-ttu-id="bf7aa-153">音频</span><span class="sxs-lookup"><span data-stu-id="bf7aa-153">Audio</span></span>
- <span data-ttu-id="bf7aa-154">视频</span><span class="sxs-lookup"><span data-stu-id="bf7aa-154">Video</span></span>
- <span data-ttu-id="bf7aa-155">应用共享</span><span class="sxs-lookup"><span data-stu-id="bf7aa-155">App Sharing</span></span>
- <span data-ttu-id="bf7aa-156">文件传输</span><span class="sxs-lookup"><span data-stu-id="bf7aa-156">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="bf7aa-157">JSON</span><span class="sxs-lookup"><span data-stu-id="bf7aa-157">JSON</span></span>

<span data-ttu-id="bf7aa-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf7aa-159">示例</span><span class="sxs-lookup"><span data-stu-id="bf7aa-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bf7aa-160">CSV</span><span class="sxs-lookup"><span data-stu-id="bf7aa-160">CSV</span></span>

<span data-ttu-id="bf7aa-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bf7aa-162">请求</span><span class="sxs-lookup"><span data-stu-id="bf7aa-162">Request</span></span>

<span data-ttu-id="bf7aa-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="bf7aa-164">响应</span><span class="sxs-lookup"><span data-stu-id="bf7aa-164">Response</span></span>

<span data-ttu-id="bf7aa-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bf7aa-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="bf7aa-167">JSON</span><span class="sxs-lookup"><span data-stu-id="bf7aa-167">JSON</span></span>

<span data-ttu-id="bf7aa-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bf7aa-169">请求</span><span class="sxs-lookup"><span data-stu-id="bf7aa-169">Request</span></span>

<span data-ttu-id="bf7aa-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="bf7aa-171">响应</span><span class="sxs-lookup"><span data-stu-id="bf7aa-171">Response</span></span>

<span data-ttu-id="bf7aa-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-172">The following is an example of the response.</span></span>

> <span data-ttu-id="bf7aa-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bf7aa-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


