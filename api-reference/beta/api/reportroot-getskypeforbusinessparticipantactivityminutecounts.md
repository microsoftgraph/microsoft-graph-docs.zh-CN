---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6677ac111a1cad24e44e4c0e77892d55069ee825
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574353"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="30a60-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="30a60-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a60-105">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="30a60-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="30a60-106">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="30a60-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="30a60-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="30a60-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="30a60-108">权限</span><span class="sxs-lookup"><span data-stu-id="30a60-108">Permissions</span></span>

<span data-ttu-id="30a60-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30a60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30a60-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30a60-111">Permission type</span></span>                        | <span data-ttu-id="30a60-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30a60-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="30a60-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30a60-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="30a60-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30a60-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="30a60-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30a60-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a60-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30a60-116">Not supported.</span></span>                           |
| <span data-ttu-id="30a60-117">应用</span><span class="sxs-lookup"><span data-stu-id="30a60-117">Application</span></span>                            | <span data-ttu-id="30a60-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30a60-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="30a60-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30a60-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="30a60-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="30a60-120">Function parameters</span></span>

<span data-ttu-id="30a60-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="30a60-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="30a60-122">参数</span><span class="sxs-lookup"><span data-stu-id="30a60-122">Parameter</span></span> | <span data-ttu-id="30a60-123">类型</span><span class="sxs-lookup"><span data-stu-id="30a60-123">Type</span></span>   | <span data-ttu-id="30a60-124">说明</span><span class="sxs-lookup"><span data-stu-id="30a60-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="30a60-125">period</span><span class="sxs-lookup"><span data-stu-id="30a60-125">period</span></span>    | <span data-ttu-id="30a60-126">string</span><span class="sxs-lookup"><span data-stu-id="30a60-126">string</span></span> | <span data-ttu-id="30a60-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="30a60-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="30a60-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="30a60-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="30a60-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="30a60-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="30a60-130">必需。</span><span class="sxs-lookup"><span data-stu-id="30a60-130">Required.</span></span> |

<span data-ttu-id="30a60-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="30a60-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="30a60-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="30a60-132">The default output type is text/csv.</span></span> <span data-ttu-id="30a60-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="30a60-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30a60-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="30a60-134">Request headers</span></span>

| <span data-ttu-id="30a60-135">名称</span><span class="sxs-lookup"><span data-stu-id="30a60-135">Name</span></span>          | <span data-ttu-id="30a60-136">说明</span><span class="sxs-lookup"><span data-stu-id="30a60-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="30a60-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="30a60-137">Authorization</span></span> | <span data-ttu-id="30a60-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30a60-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="30a60-140">响应</span><span class="sxs-lookup"><span data-stu-id="30a60-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="30a60-141">CSV</span><span class="sxs-lookup"><span data-stu-id="30a60-141">CSV</span></span>

<span data-ttu-id="30a60-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="30a60-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="30a60-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="30a60-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="30a60-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="30a60-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="30a60-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="30a60-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="30a60-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="30a60-146">Report Refresh Date</span></span>
- <span data-ttu-id="30a60-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="30a60-147">Report Date</span></span>
- <span data-ttu-id="30a60-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="30a60-148">Report Period</span></span>
- <span data-ttu-id="30a60-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="30a60-149">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="30a60-150">JSON</span><span class="sxs-lookup"><span data-stu-id="30a60-150">JSON</span></span>

<span data-ttu-id="30a60-151">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="30a60-151">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a60-152">示例</span><span class="sxs-lookup"><span data-stu-id="30a60-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="30a60-153">CSV</span><span class="sxs-lookup"><span data-stu-id="30a60-153">CSV</span></span>

<span data-ttu-id="30a60-154">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="30a60-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="30a60-155">请求</span><span class="sxs-lookup"><span data-stu-id="30a60-155">Request</span></span>

<span data-ttu-id="30a60-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30a60-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="30a60-157">响应</span><span class="sxs-lookup"><span data-stu-id="30a60-157">Response</span></span>

<span data-ttu-id="30a60-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30a60-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="30a60-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="30a60-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="30a60-160">JSON</span><span class="sxs-lookup"><span data-stu-id="30a60-160">JSON</span></span>

<span data-ttu-id="30a60-161">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="30a60-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="30a60-162">请求</span><span class="sxs-lookup"><span data-stu-id="30a60-162">Request</span></span>

<span data-ttu-id="30a60-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30a60-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="30a60-164">响应</span><span class="sxs-lookup"><span data-stu-id="30a60-164">Response</span></span>

<span data-ttu-id="30a60-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30a60-165">The following is an example of the response.</span></span>

> <span data-ttu-id="30a60-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="30a60-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
