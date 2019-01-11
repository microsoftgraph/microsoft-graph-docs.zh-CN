---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: 获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。 对等会话类型包括 IM、音频、视频、应用共享和文件传输。
localization_priority: Normal
ms.openlocfilehash: 466a725b9dd9f357c082d48817b5134e702c8b30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891866"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="b2d4f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b2d4f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

> <span data-ttu-id="b2d4f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2d4f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2d4f-107">获取使用情况趋势，即组织中召开的对等会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-107">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="b2d4f-108">对等会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-108">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="b2d4f-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d4f-110">权限</span><span class="sxs-lookup"><span data-stu-id="b2d4f-110">Permissions</span></span>

<span data-ttu-id="b2d4f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2d4f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2d4f-113">Permission type</span></span>                        | <span data-ttu-id="b2d4f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2d4f-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b2d4f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d4f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2d4f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2d4f-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b2d4f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d4f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2d4f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-118">Not supported.</span></span>                           |
| <span data-ttu-id="b2d4f-119">应用</span><span class="sxs-lookup"><span data-stu-id="b2d4f-119">Application</span></span>                            | <span data-ttu-id="b2d4f-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2d4f-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b2d4f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2d4f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b2d4f-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="b2d4f-122">Function parameters</span></span>

<span data-ttu-id="b2d4f-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b2d4f-124">参数</span><span class="sxs-lookup"><span data-stu-id="b2d4f-124">Parameter</span></span> | <span data-ttu-id="b2d4f-125">类型</span><span class="sxs-lookup"><span data-stu-id="b2d4f-125">Type</span></span>   | <span data-ttu-id="b2d4f-126">说明</span><span class="sxs-lookup"><span data-stu-id="b2d4f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b2d4f-127">period</span><span class="sxs-lookup"><span data-stu-id="b2d4f-127">period</span></span>    | <span data-ttu-id="b2d4f-128">string</span><span class="sxs-lookup"><span data-stu-id="b2d4f-128">string</span></span> | <span data-ttu-id="b2d4f-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b2d4f-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b2d4f-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b2d4f-132">必需。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-132">Required.</span></span> |

<span data-ttu-id="b2d4f-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b2d4f-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-134">The default output type is text/csv.</span></span> <span data-ttu-id="b2d4f-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2d4f-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2d4f-136">Request headers</span></span>

| <span data-ttu-id="b2d4f-137">名称</span><span class="sxs-lookup"><span data-stu-id="b2d4f-137">Name</span></span>          | <span data-ttu-id="b2d4f-138">说明</span><span class="sxs-lookup"><span data-stu-id="b2d4f-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b2d4f-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d4f-139">Authorization</span></span> | <span data-ttu-id="b2d4f-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b2d4f-142">响应</span><span class="sxs-lookup"><span data-stu-id="b2d4f-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b2d4f-143">CSV</span><span class="sxs-lookup"><span data-stu-id="b2d4f-143">CSV</span></span>

<span data-ttu-id="b2d4f-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b2d4f-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b2d4f-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b2d4f-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b2d4f-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b2d4f-148">Report Refresh Date</span></span>
- <span data-ttu-id="b2d4f-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="b2d4f-149">Report Date</span></span>
- <span data-ttu-id="b2d4f-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="b2d4f-150">Report Period</span></span>
- <span data-ttu-id="b2d4f-151">IM</span><span class="sxs-lookup"><span data-stu-id="b2d4f-151">IM</span></span>
- <span data-ttu-id="b2d4f-152">音频</span><span class="sxs-lookup"><span data-stu-id="b2d4f-152">Audio</span></span>
- <span data-ttu-id="b2d4f-153">视频</span><span class="sxs-lookup"><span data-stu-id="b2d4f-153">Video</span></span>
- <span data-ttu-id="b2d4f-154">应用共享</span><span class="sxs-lookup"><span data-stu-id="b2d4f-154">App Sharing</span></span>
- <span data-ttu-id="b2d4f-155">文件传输</span><span class="sxs-lookup"><span data-stu-id="b2d4f-155">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="b2d4f-156">JSON</span><span class="sxs-lookup"><span data-stu-id="b2d4f-156">JSON</span></span>

<span data-ttu-id="b2d4f-157">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2d4f-158">示例</span><span class="sxs-lookup"><span data-stu-id="b2d4f-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b2d4f-159">CSV</span><span class="sxs-lookup"><span data-stu-id="b2d4f-159">CSV</span></span>

<span data-ttu-id="b2d4f-160">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b2d4f-161">请求</span><span class="sxs-lookup"><span data-stu-id="b2d4f-161">Request</span></span>

<span data-ttu-id="b2d4f-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b2d4f-163">响应</span><span class="sxs-lookup"><span data-stu-id="b2d4f-163">Response</span></span>

<span data-ttu-id="b2d4f-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b2d4f-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b2d4f-166">JSON</span><span class="sxs-lookup"><span data-stu-id="b2d4f-166">JSON</span></span>

<span data-ttu-id="b2d4f-167">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b2d4f-168">请求</span><span class="sxs-lookup"><span data-stu-id="b2d4f-168">Request</span></span>

<span data-ttu-id="b2d4f-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b2d4f-170">响应</span><span class="sxs-lookup"><span data-stu-id="b2d4f-170">Response</span></span>

<span data-ttu-id="b2d4f-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-171">The following is an example of the response.</span></span>

> <span data-ttu-id="b2d4f-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b2d4f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
