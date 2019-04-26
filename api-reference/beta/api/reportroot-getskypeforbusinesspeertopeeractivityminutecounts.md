---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。 会话类型包括音频和视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15ed192eab2641dd91354726812ae4d4f528c71a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336475"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="8feac-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="8feac-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8feac-105">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="8feac-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="8feac-106">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="8feac-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="8feac-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="8feac-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="8feac-108">权限</span><span class="sxs-lookup"><span data-stu-id="8feac-108">Permissions</span></span>

<span data-ttu-id="8feac-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8feac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8feac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8feac-111">Permission type</span></span>                        | <span data-ttu-id="8feac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8feac-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8feac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8feac-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8feac-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8feac-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8feac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8feac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8feac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8feac-116">Not supported.</span></span>                           |
| <span data-ttu-id="8feac-117">应用</span><span class="sxs-lookup"><span data-stu-id="8feac-117">Application</span></span>                            | <span data-ttu-id="8feac-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8feac-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8feac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8feac-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8feac-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="8feac-120">Function parameters</span></span>

<span data-ttu-id="8feac-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="8feac-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8feac-122">参数</span><span class="sxs-lookup"><span data-stu-id="8feac-122">Parameter</span></span> | <span data-ttu-id="8feac-123">类型</span><span class="sxs-lookup"><span data-stu-id="8feac-123">Type</span></span>   | <span data-ttu-id="8feac-124">说明</span><span class="sxs-lookup"><span data-stu-id="8feac-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8feac-125">period</span><span class="sxs-lookup"><span data-stu-id="8feac-125">period</span></span>    | <span data-ttu-id="8feac-126">string</span><span class="sxs-lookup"><span data-stu-id="8feac-126">string</span></span> | <span data-ttu-id="8feac-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8feac-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8feac-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8feac-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8feac-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8feac-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8feac-130">必需。</span><span class="sxs-lookup"><span data-stu-id="8feac-130">Required.</span></span> |

<span data-ttu-id="8feac-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8feac-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8feac-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="8feac-132">The default output type is text/csv.</span></span> <span data-ttu-id="8feac-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="8feac-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8feac-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="8feac-134">Request headers</span></span>

| <span data-ttu-id="8feac-135">名称</span><span class="sxs-lookup"><span data-stu-id="8feac-135">Name</span></span>          | <span data-ttu-id="8feac-136">说明</span><span class="sxs-lookup"><span data-stu-id="8feac-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8feac-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8feac-137">Authorization</span></span> | <span data-ttu-id="8feac-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8feac-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8feac-140">响应</span><span class="sxs-lookup"><span data-stu-id="8feac-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8feac-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8feac-141">CSV</span></span>

<span data-ttu-id="8feac-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8feac-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8feac-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8feac-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8feac-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8feac-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8feac-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="8feac-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8feac-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8feac-146">Report Refresh Date</span></span>
- <span data-ttu-id="8feac-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="8feac-147">Report Date</span></span>
- <span data-ttu-id="8feac-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="8feac-148">Report Period</span></span>
- <span data-ttu-id="8feac-149">音频</span><span class="sxs-lookup"><span data-stu-id="8feac-149">Audio</span></span>
- <span data-ttu-id="8feac-150">视频</span><span class="sxs-lookup"><span data-stu-id="8feac-150">Video</span></span>

### <a name="json"></a><span data-ttu-id="8feac-151">JSON</span><span class="sxs-lookup"><span data-stu-id="8feac-151">JSON</span></span>

<span data-ttu-id="8feac-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="8feac-152">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8feac-153">示例</span><span class="sxs-lookup"><span data-stu-id="8feac-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8feac-154">CSV</span><span class="sxs-lookup"><span data-stu-id="8feac-154">CSV</span></span>

<span data-ttu-id="8feac-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="8feac-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8feac-156">请求</span><span class="sxs-lookup"><span data-stu-id="8feac-156">Request</span></span>

<span data-ttu-id="8feac-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8feac-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8feac-158">响应</span><span class="sxs-lookup"><span data-stu-id="8feac-158">Response</span></span>

<span data-ttu-id="8feac-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8feac-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8feac-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8feac-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="8feac-161">JSON</span><span class="sxs-lookup"><span data-stu-id="8feac-161">JSON</span></span>

<span data-ttu-id="8feac-162">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="8feac-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8feac-163">请求</span><span class="sxs-lookup"><span data-stu-id="8feac-163">Request</span></span>

<span data-ttu-id="8feac-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8feac-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8feac-165">响应</span><span class="sxs-lookup"><span data-stu-id="8feac-165">Response</span></span>

<span data-ttu-id="8feac-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8feac-166">The following is an example of the response.</span></span>

> <span data-ttu-id="8feac-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8feac-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
