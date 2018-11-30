---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: 按 Outlook 桌面版获取唯一用户数。
ms.openlocfilehash: fd172e97b5c7c036fb33e3d4ab0e8088d9d0af7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048368"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="faa0f-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="faa0f-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

> <span data-ttu-id="faa0f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="faa0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faa0f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="faa0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faa0f-106">按 Outlook 桌面版获取唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="faa0f-106">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="faa0f-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="faa0f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="faa0f-108">权限</span><span class="sxs-lookup"><span data-stu-id="faa0f-108">Permissions</span></span>

<span data-ttu-id="faa0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faa0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="faa0f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="faa0f-111">Permission type</span></span>                        | <span data-ttu-id="faa0f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="faa0f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="faa0f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faa0f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="faa0f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="faa0f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="faa0f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faa0f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faa0f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="faa0f-116">Not supported.</span></span>                           |
| <span data-ttu-id="faa0f-117">应用</span><span class="sxs-lookup"><span data-stu-id="faa0f-117">Application</span></span>                            | <span data-ttu-id="faa0f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="faa0f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="faa0f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faa0f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="faa0f-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="faa0f-120">Function parameters</span></span>

<span data-ttu-id="faa0f-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="faa0f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="faa0f-122">参数</span><span class="sxs-lookup"><span data-stu-id="faa0f-122">Parameter</span></span> | <span data-ttu-id="faa0f-123">类型</span><span class="sxs-lookup"><span data-stu-id="faa0f-123">Type</span></span>   | <span data-ttu-id="faa0f-124">说明</span><span class="sxs-lookup"><span data-stu-id="faa0f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="faa0f-125">period</span><span class="sxs-lookup"><span data-stu-id="faa0f-125">period</span></span>    | <span data-ttu-id="faa0f-126">string</span><span class="sxs-lookup"><span data-stu-id="faa0f-126">string</span></span> | <span data-ttu-id="faa0f-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="faa0f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="faa0f-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="faa0f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="faa0f-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="faa0f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="faa0f-130">必需。</span><span class="sxs-lookup"><span data-stu-id="faa0f-130">Required.</span></span> |

<span data-ttu-id="faa0f-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="faa0f-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="faa0f-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="faa0f-132">The default output type is text/csv.</span></span> <span data-ttu-id="faa0f-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="faa0f-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="faa0f-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="faa0f-134">Request headers</span></span>

| <span data-ttu-id="faa0f-135">名称</span><span class="sxs-lookup"><span data-stu-id="faa0f-135">Name</span></span>          | <span data-ttu-id="faa0f-136">说明</span><span class="sxs-lookup"><span data-stu-id="faa0f-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="faa0f-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="faa0f-137">Authorization</span></span> | <span data-ttu-id="faa0f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="faa0f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="faa0f-140">响应</span><span class="sxs-lookup"><span data-stu-id="faa0f-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="faa0f-141">CSV</span><span class="sxs-lookup"><span data-stu-id="faa0f-141">CSV</span></span>

<span data-ttu-id="faa0f-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="faa0f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="faa0f-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="faa0f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="faa0f-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="faa0f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="faa0f-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="faa0f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="faa0f-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="faa0f-146">Report Refresh Date</span></span>
- <span data-ttu-id="faa0f-147">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="faa0f-147">Outlook 2016</span></span>
- <span data-ttu-id="faa0f-148">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="faa0f-148">Outlook 2013</span></span>
- <span data-ttu-id="faa0f-149">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="faa0f-149">Outlook 2010</span></span>
- <span data-ttu-id="faa0f-150">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="faa0f-150">Outlook 2007</span></span>
- <span data-ttu-id="faa0f-151">不确定</span><span class="sxs-lookup"><span data-stu-id="faa0f-151">Undetermined</span></span>
- <span data-ttu-id="faa0f-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="faa0f-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="faa0f-153">JSON</span><span class="sxs-lookup"><span data-stu-id="faa0f-153">JSON</span></span>

<span data-ttu-id="faa0f-154">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="faa0f-154">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faa0f-155">示例</span><span class="sxs-lookup"><span data-stu-id="faa0f-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="faa0f-156">CSV</span><span class="sxs-lookup"><span data-stu-id="faa0f-156">CSV</span></span>

<span data-ttu-id="faa0f-157">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="faa0f-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="faa0f-158">请求</span><span class="sxs-lookup"><span data-stu-id="faa0f-158">Request</span></span>

<span data-ttu-id="faa0f-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="faa0f-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="faa0f-160">响应</span><span class="sxs-lookup"><span data-stu-id="faa0f-160">Response</span></span>

<span data-ttu-id="faa0f-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="faa0f-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="faa0f-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="faa0f-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="faa0f-163">JSON</span><span class="sxs-lookup"><span data-stu-id="faa0f-163">JSON</span></span>

<span data-ttu-id="faa0f-164">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="faa0f-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="faa0f-165">请求</span><span class="sxs-lookup"><span data-stu-id="faa0f-165">Request</span></span>

<span data-ttu-id="faa0f-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="faa0f-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="faa0f-167">响应</span><span class="sxs-lookup"><span data-stu-id="faa0f-167">Response</span></span>

<span data-ttu-id="faa0f-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="faa0f-168">The following is an example of the response.</span></span>

> <span data-ttu-id="faa0f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="faa0f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
