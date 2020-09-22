---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f98fa0886174126817eda13a7f658cf3de870fe3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067815"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="c7a74-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c7a74-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="c7a74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7a74-105">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="c7a74-105">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="c7a74-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-电子邮件应用程序使用](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="c7a74-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7a74-107">权限</span><span class="sxs-lookup"><span data-stu-id="c7a74-107">Permissions</span></span>

<span data-ttu-id="c7a74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7a74-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7a74-110">Permission type</span></span>                        | <span data-ttu-id="c7a74-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7a74-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c7a74-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a74-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7a74-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7a74-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c7a74-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7a74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7a74-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7a74-115">Not supported.</span></span>                           |
| <span data-ttu-id="c7a74-116">应用</span><span class="sxs-lookup"><span data-stu-id="c7a74-116">Application</span></span>                            | <span data-ttu-id="c7a74-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7a74-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="c7a74-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="c7a74-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c7a74-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="c7a74-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c7a74-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7a74-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c7a74-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="c7a74-121">Function parameters</span></span>

<span data-ttu-id="c7a74-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c7a74-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c7a74-123">参数</span><span class="sxs-lookup"><span data-stu-id="c7a74-123">Parameter</span></span> | <span data-ttu-id="c7a74-124">类型</span><span class="sxs-lookup"><span data-stu-id="c7a74-124">Type</span></span>   | <span data-ttu-id="c7a74-125">说明</span><span class="sxs-lookup"><span data-stu-id="c7a74-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c7a74-126">period</span><span class="sxs-lookup"><span data-stu-id="c7a74-126">period</span></span>    | <span data-ttu-id="c7a74-127">string</span><span class="sxs-lookup"><span data-stu-id="c7a74-127">string</span></span> | <span data-ttu-id="c7a74-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c7a74-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c7a74-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c7a74-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c7a74-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c7a74-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c7a74-131">必需。</span><span class="sxs-lookup"><span data-stu-id="c7a74-131">Required.</span></span> |

<span data-ttu-id="c7a74-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7a74-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c7a74-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="c7a74-133">The default output type is text/csv.</span></span> <span data-ttu-id="c7a74-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="c7a74-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7a74-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7a74-135">Request headers</span></span>

| <span data-ttu-id="c7a74-136">名称</span><span class="sxs-lookup"><span data-stu-id="c7a74-136">Name</span></span>          | <span data-ttu-id="c7a74-137">说明</span><span class="sxs-lookup"><span data-stu-id="c7a74-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c7a74-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7a74-138">Authorization</span></span> | <span data-ttu-id="c7a74-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7a74-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c7a74-141">响应</span><span class="sxs-lookup"><span data-stu-id="c7a74-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c7a74-142">CSV</span><span class="sxs-lookup"><span data-stu-id="c7a74-142">CSV</span></span>

<span data-ttu-id="c7a74-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c7a74-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c7a74-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c7a74-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c7a74-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="c7a74-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c7a74-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="c7a74-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c7a74-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c7a74-147">Report Refresh Date</span></span>
- <span data-ttu-id="c7a74-148">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="c7a74-148">Mail For Mac</span></span>
- <span data-ttu-id="c7a74-149">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="c7a74-149">Outlook For Mac</span></span>
- <span data-ttu-id="c7a74-150">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="c7a74-150">Outlook For Windows</span></span>
- <span data-ttu-id="c7a74-151">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="c7a74-151">Outlook For Mobile</span></span>
- <span data-ttu-id="c7a74-152">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="c7a74-152">Other For Mobile</span></span>
- <span data-ttu-id="c7a74-153">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="c7a74-153">Outlook For Web</span></span>
- <span data-ttu-id="c7a74-154">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="c7a74-154">POP3 App</span></span>
- <span data-ttu-id="c7a74-155">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="c7a74-155">IMAP4 App</span></span>
- <span data-ttu-id="c7a74-156">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="c7a74-156">SMTP App</span></span>
- <span data-ttu-id="c7a74-157">报表日期</span><span class="sxs-lookup"><span data-stu-id="c7a74-157">Report Date</span></span>
- <span data-ttu-id="c7a74-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="c7a74-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c7a74-159">JSON</span><span class="sxs-lookup"><span data-stu-id="c7a74-159">JSON</span></span>

<span data-ttu-id="c7a74-160">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="c7a74-160">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7a74-161">示例</span><span class="sxs-lookup"><span data-stu-id="c7a74-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c7a74-162">CSV</span><span class="sxs-lookup"><span data-stu-id="c7a74-162">CSV</span></span>

<span data-ttu-id="c7a74-163">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="c7a74-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c7a74-164">请求</span><span class="sxs-lookup"><span data-stu-id="c7a74-164">Request</span></span>

<span data-ttu-id="c7a74-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7a74-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="c7a74-166">响应</span><span class="sxs-lookup"><span data-stu-id="c7a74-166">Response</span></span>

<span data-ttu-id="c7a74-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7a74-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c7a74-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c7a74-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c7a74-169">JSON</span><span class="sxs-lookup"><span data-stu-id="c7a74-169">JSON</span></span>

<span data-ttu-id="c7a74-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="c7a74-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c7a74-171">请求</span><span class="sxs-lookup"><span data-stu-id="c7a74-171">Request</span></span>

<span data-ttu-id="c7a74-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7a74-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="c7a74-173">响应</span><span class="sxs-lookup"><span data-stu-id="c7a74-173">Response</span></span>

<span data-ttu-id="c7a74-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7a74-174">The following is an example of the response.</span></span>

> <span data-ttu-id="c7a74-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7a74-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


