---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: 获取每个电子邮件应用的唯一用户数。
localization_priority: Normal
ms.openlocfilehash: 7aab9765092218c5f0555ec84099c826ae29fa94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826955"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="1d6ae-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="1d6ae-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

> <span data-ttu-id="1d6ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d6ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d6ae-106">获取每个电子邮件应用的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-106">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="1d6ae-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d6ae-108">权限</span><span class="sxs-lookup"><span data-stu-id="1d6ae-108">Permissions</span></span>

<span data-ttu-id="1d6ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d6ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d6ae-111">Permission type</span></span>                        | <span data-ttu-id="1d6ae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d6ae-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1d6ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d6ae-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d6ae-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d6ae-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1d6ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d6ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d6ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-116">Not supported.</span></span>                           |
| <span data-ttu-id="1d6ae-117">应用</span><span class="sxs-lookup"><span data-stu-id="1d6ae-117">Application</span></span>                            | <span data-ttu-id="1d6ae-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d6ae-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1d6ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d6ae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1d6ae-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="1d6ae-120">Function parameters</span></span>

<span data-ttu-id="1d6ae-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1d6ae-122">参数</span><span class="sxs-lookup"><span data-stu-id="1d6ae-122">Parameter</span></span> | <span data-ttu-id="1d6ae-123">类型</span><span class="sxs-lookup"><span data-stu-id="1d6ae-123">Type</span></span>   | <span data-ttu-id="1d6ae-124">说明</span><span class="sxs-lookup"><span data-stu-id="1d6ae-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1d6ae-125">period</span><span class="sxs-lookup"><span data-stu-id="1d6ae-125">period</span></span>    | <span data-ttu-id="1d6ae-126">string</span><span class="sxs-lookup"><span data-stu-id="1d6ae-126">string</span></span> | <span data-ttu-id="1d6ae-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1d6ae-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1d6ae-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1d6ae-130">必需。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-130">Required.</span></span> |

<span data-ttu-id="1d6ae-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1d6ae-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-132">The default output type is text/csv.</span></span> <span data-ttu-id="1d6ae-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d6ae-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d6ae-134">Request headers</span></span>

| <span data-ttu-id="1d6ae-135">名称</span><span class="sxs-lookup"><span data-stu-id="1d6ae-135">Name</span></span>          | <span data-ttu-id="1d6ae-136">说明</span><span class="sxs-lookup"><span data-stu-id="1d6ae-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1d6ae-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d6ae-137">Authorization</span></span> | <span data-ttu-id="1d6ae-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1d6ae-140">响应</span><span class="sxs-lookup"><span data-stu-id="1d6ae-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1d6ae-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1d6ae-141">CSV</span></span>

<span data-ttu-id="1d6ae-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1d6ae-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1d6ae-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1d6ae-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1d6ae-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1d6ae-146">Report Refresh Date</span></span>
- <span data-ttu-id="1d6ae-147">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="1d6ae-147">Mail For Mac</span></span>
- <span data-ttu-id="1d6ae-148">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="1d6ae-148">Outlook For Mac</span></span>
- <span data-ttu-id="1d6ae-149">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="1d6ae-149">Outlook For Windows</span></span>
- <span data-ttu-id="1d6ae-150">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="1d6ae-150">Outlook For Mobile</span></span>
- <span data-ttu-id="1d6ae-151">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="1d6ae-151">Other For Mobile</span></span>
- <span data-ttu-id="1d6ae-152">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="1d6ae-152">Outlook For Web</span></span>
- <span data-ttu-id="1d6ae-153">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="1d6ae-153">POP3 App</span></span>
- <span data-ttu-id="1d6ae-154">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="1d6ae-154">IMAP4 App</span></span>
- <span data-ttu-id="1d6ae-155">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="1d6ae-155">SMTP App</span></span>
- <span data-ttu-id="1d6ae-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="1d6ae-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1d6ae-157">JSON</span><span class="sxs-lookup"><span data-stu-id="1d6ae-157">JSON</span></span>

<span data-ttu-id="1d6ae-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-158">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d6ae-159">示例</span><span class="sxs-lookup"><span data-stu-id="1d6ae-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1d6ae-160">CSV</span><span class="sxs-lookup"><span data-stu-id="1d6ae-160">CSV</span></span>

<span data-ttu-id="1d6ae-161">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1d6ae-162">请求</span><span class="sxs-lookup"><span data-stu-id="1d6ae-162">Request</span></span>

<span data-ttu-id="1d6ae-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1d6ae-164">响应</span><span class="sxs-lookup"><span data-stu-id="1d6ae-164">Response</span></span>

<span data-ttu-id="1d6ae-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1d6ae-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="1d6ae-167">JSON</span><span class="sxs-lookup"><span data-stu-id="1d6ae-167">JSON</span></span>

<span data-ttu-id="1d6ae-168">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1d6ae-169">请求</span><span class="sxs-lookup"><span data-stu-id="1d6ae-169">Request</span></span>

<span data-ttu-id="1d6ae-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1d6ae-171">响应</span><span class="sxs-lookup"><span data-stu-id="1d6ae-171">Response</span></span>

<span data-ttu-id="1d6ae-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-172">The following is an example of the response.</span></span>

> <span data-ttu-id="1d6ae-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1d6ae-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageAppsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 4, 
      "outlookForMac": 105, 
      "outlookForWindows": 1589, 
      "outlookForMobile": 1116, 
      "otherForMobile": 485, 
      "outlookForWeb": 753, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
