---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4517a9955e976bbefe5369fc64dc0c485f7d67f7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336770"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="aa4ca-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="aa4ca-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa4ca-104">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="aa4ca-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa4ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa4ca-106">Permissions</span></span>

<span data-ttu-id="aa4ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa4ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa4ca-109">Permission type</span></span>                        | <span data-ttu-id="aa4ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa4ca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aa4ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa4ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa4ca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa4ca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aa4ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa4ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa4ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-114">Not supported.</span></span>                           |
| <span data-ttu-id="aa4ca-115">应用</span><span class="sxs-lookup"><span data-stu-id="aa4ca-115">Application</span></span>                            | <span data-ttu-id="aa4ca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa4ca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aa4ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa4ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="aa4ca-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="aa4ca-118">Function parameters</span></span>

<span data-ttu-id="aa4ca-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aa4ca-120">参数</span><span class="sxs-lookup"><span data-stu-id="aa4ca-120">Parameter</span></span> | <span data-ttu-id="aa4ca-121">类型</span><span class="sxs-lookup"><span data-stu-id="aa4ca-121">Type</span></span>   | <span data-ttu-id="aa4ca-122">说明</span><span class="sxs-lookup"><span data-stu-id="aa4ca-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aa4ca-123">period</span><span class="sxs-lookup"><span data-stu-id="aa4ca-123">period</span></span>    | <span data-ttu-id="aa4ca-124">string</span><span class="sxs-lookup"><span data-stu-id="aa4ca-124">string</span></span> | <span data-ttu-id="aa4ca-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aa4ca-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aa4ca-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aa4ca-128">必需。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-128">Required.</span></span> |

<span data-ttu-id="aa4ca-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aa4ca-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-130">The default output type is text/csv.</span></span> <span data-ttu-id="aa4ca-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa4ca-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa4ca-132">Request headers</span></span>

| <span data-ttu-id="aa4ca-133">名称</span><span class="sxs-lookup"><span data-stu-id="aa4ca-133">Name</span></span>          | <span data-ttu-id="aa4ca-134">说明</span><span class="sxs-lookup"><span data-stu-id="aa4ca-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aa4ca-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa4ca-135">Authorization</span></span> | <span data-ttu-id="aa4ca-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aa4ca-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa4ca-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aa4ca-139">CSV</span><span class="sxs-lookup"><span data-stu-id="aa4ca-139">CSV</span></span>

<span data-ttu-id="aa4ca-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aa4ca-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aa4ca-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aa4ca-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aa4ca-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="aa4ca-144">Report Refresh Date</span></span>
- <span data-ttu-id="aa4ca-145">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="aa4ca-145">Mail For Mac</span></span>
- <span data-ttu-id="aa4ca-146">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="aa4ca-146">Outlook For Mac</span></span>
- <span data-ttu-id="aa4ca-147">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="aa4ca-147">Outlook For Windows</span></span>
- <span data-ttu-id="aa4ca-148">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="aa4ca-148">Outlook For Mobile</span></span>
- <span data-ttu-id="aa4ca-149">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="aa4ca-149">Other For Mobile</span></span>
- <span data-ttu-id="aa4ca-150">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="aa4ca-150">Outlook For Web</span></span>
- <span data-ttu-id="aa4ca-151">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="aa4ca-151">POP3 App</span></span>
- <span data-ttu-id="aa4ca-152">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="aa4ca-152">IMAP4 App</span></span>
- <span data-ttu-id="aa4ca-153">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="aa4ca-153">SMTP App</span></span>
- <span data-ttu-id="aa4ca-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="aa4ca-154">Report Date</span></span>
- <span data-ttu-id="aa4ca-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="aa4ca-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aa4ca-156">JSON</span><span class="sxs-lookup"><span data-stu-id="aa4ca-156">JSON</span></span>

<span data-ttu-id="aa4ca-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa4ca-158">示例</span><span class="sxs-lookup"><span data-stu-id="aa4ca-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aa4ca-159">CSV</span><span class="sxs-lookup"><span data-stu-id="aa4ca-159">CSV</span></span>

<span data-ttu-id="aa4ca-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aa4ca-161">请求</span><span class="sxs-lookup"><span data-stu-id="aa4ca-161">Request</span></span>

<span data-ttu-id="aa4ca-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="aa4ca-163">响应</span><span class="sxs-lookup"><span data-stu-id="aa4ca-163">Response</span></span>

<span data-ttu-id="aa4ca-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aa4ca-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="aa4ca-166">JSON</span><span class="sxs-lookup"><span data-stu-id="aa4ca-166">JSON</span></span>

<span data-ttu-id="aa4ca-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aa4ca-168">请求</span><span class="sxs-lookup"><span data-stu-id="aa4ca-168">Request</span></span>

<span data-ttu-id="aa4ca-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="aa4ca-170">响应</span><span class="sxs-lookup"><span data-stu-id="aa4ca-170">Response</span></span>

<span data-ttu-id="aa4ca-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-171">The following is an example of the response.</span></span>

> <span data-ttu-id="aa4ca-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa4ca-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
