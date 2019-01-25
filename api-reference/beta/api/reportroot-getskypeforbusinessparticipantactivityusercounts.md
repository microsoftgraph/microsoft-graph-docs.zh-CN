---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 17e12e060e8ffbe6baf99c3bb68d2f999274932e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520846"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="6e3f8-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e3f8-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e3f8-105">获取使用情况趋势，即组织中用户参与的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="6e3f8-106">会议会话类型包括 IM、音频/视频、应用共享、Web 和第三方拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="6e3f8-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e3f8-108">权限</span><span class="sxs-lookup"><span data-stu-id="6e3f8-108">Permissions</span></span>

<span data-ttu-id="6e3f8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e3f8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e3f8-111">Permission type</span></span>                        | <span data-ttu-id="6e3f8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e3f8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6e3f8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e3f8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e3f8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3f8-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6e3f8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e3f8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-116">Not supported.</span></span>                           |
| <span data-ttu-id="6e3f8-117">应用</span><span class="sxs-lookup"><span data-stu-id="6e3f8-117">Application</span></span>                            | <span data-ttu-id="6e3f8-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3f8-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6e3f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e3f8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6e3f8-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="6e3f8-120">Function parameters</span></span>

<span data-ttu-id="6e3f8-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6e3f8-122">参数</span><span class="sxs-lookup"><span data-stu-id="6e3f8-122">Parameter</span></span> | <span data-ttu-id="6e3f8-123">类型</span><span class="sxs-lookup"><span data-stu-id="6e3f8-123">Type</span></span>   | <span data-ttu-id="6e3f8-124">说明</span><span class="sxs-lookup"><span data-stu-id="6e3f8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6e3f8-125">period</span><span class="sxs-lookup"><span data-stu-id="6e3f8-125">period</span></span>    | <span data-ttu-id="6e3f8-126">string</span><span class="sxs-lookup"><span data-stu-id="6e3f8-126">string</span></span> | <span data-ttu-id="6e3f8-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6e3f8-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6e3f8-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6e3f8-130">必需。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-130">Required.</span></span> |

<span data-ttu-id="6e3f8-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6e3f8-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-132">The default output type is text/csv.</span></span> <span data-ttu-id="6e3f8-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e3f8-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e3f8-134">Request headers</span></span>

| <span data-ttu-id="6e3f8-135">名称</span><span class="sxs-lookup"><span data-stu-id="6e3f8-135">Name</span></span>          | <span data-ttu-id="6e3f8-136">说明</span><span class="sxs-lookup"><span data-stu-id="6e3f8-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6e3f8-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e3f8-137">Authorization</span></span> | <span data-ttu-id="6e3f8-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6e3f8-140">响应</span><span class="sxs-lookup"><span data-stu-id="6e3f8-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6e3f8-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6e3f8-141">CSV</span></span>

<span data-ttu-id="6e3f8-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6e3f8-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6e3f8-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6e3f8-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6e3f8-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6e3f8-146">Report Refresh Date</span></span>
- <span data-ttu-id="6e3f8-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="6e3f8-147">Report Date</span></span>
- <span data-ttu-id="6e3f8-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="6e3f8-148">Report Period</span></span>
- <span data-ttu-id="6e3f8-149">IM</span><span class="sxs-lookup"><span data-stu-id="6e3f8-149">IM</span></span>
- <span data-ttu-id="6e3f8-150">音频/视频</span><span class="sxs-lookup"><span data-stu-id="6e3f8-150">Audio/Video</span></span>
- <span data-ttu-id="6e3f8-151">应用共享</span><span class="sxs-lookup"><span data-stu-id="6e3f8-151">App Sharing</span></span>
- <span data-ttu-id="6e3f8-152">Web</span><span class="sxs-lookup"><span data-stu-id="6e3f8-152">Web</span></span>
- <span data-ttu-id="6e3f8-153">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="6e3f8-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="6e3f8-154">JSON</span><span class="sxs-lookup"><span data-stu-id="6e3f8-154">JSON</span></span>

<span data-ttu-id="6e3f8-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e3f8-156">示例</span><span class="sxs-lookup"><span data-stu-id="6e3f8-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6e3f8-157">CSV</span><span class="sxs-lookup"><span data-stu-id="6e3f8-157">CSV</span></span>

<span data-ttu-id="6e3f8-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6e3f8-159">请求</span><span class="sxs-lookup"><span data-stu-id="6e3f8-159">Request</span></span>

<span data-ttu-id="6e3f8-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6e3f8-161">响应</span><span class="sxs-lookup"><span data-stu-id="6e3f8-161">Response</span></span>

<span data-ttu-id="6e3f8-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6e3f8-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="6e3f8-164">JSON</span><span class="sxs-lookup"><span data-stu-id="6e3f8-164">JSON</span></span>

<span data-ttu-id="6e3f8-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6e3f8-166">请求</span><span class="sxs-lookup"><span data-stu-id="6e3f8-166">Request</span></span>

<span data-ttu-id="6e3f8-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6e3f8-168">响应</span><span class="sxs-lookup"><span data-stu-id="6e3f8-168">Response</span></span>

<span data-ttu-id="6e3f8-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-169">The following is an example of the response.</span></span>

> <span data-ttu-id="6e3f8-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e3f8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
