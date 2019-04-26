---
title: 'reportRoot: getEmailActivityUserCounts'
description: 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b38506b30969882b817092225439a23249164981
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331739"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="f6493-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f6493-103">reportRoot: getEmailActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6493-104">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="f6493-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="f6493-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="f6493-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6493-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6493-106">Permissions</span></span>

<span data-ttu-id="f6493-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6493-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6493-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6493-109">Permission type</span></span>                        | <span data-ttu-id="f6493-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6493-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f6493-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6493-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6493-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6493-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f6493-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6493-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6493-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6493-114">Not supported.</span></span>                           |
| <span data-ttu-id="f6493-115">应用</span><span class="sxs-lookup"><span data-stu-id="f6493-115">Application</span></span>                            | <span data-ttu-id="f6493-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6493-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f6493-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6493-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f6493-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="f6493-118">Function parameters</span></span>

<span data-ttu-id="f6493-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f6493-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f6493-120">参数</span><span class="sxs-lookup"><span data-stu-id="f6493-120">Parameter</span></span> | <span data-ttu-id="f6493-121">类型</span><span class="sxs-lookup"><span data-stu-id="f6493-121">Type</span></span>   | <span data-ttu-id="f6493-122">说明</span><span class="sxs-lookup"><span data-stu-id="f6493-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f6493-123">period</span><span class="sxs-lookup"><span data-stu-id="f6493-123">period</span></span>    | <span data-ttu-id="f6493-124">string</span><span class="sxs-lookup"><span data-stu-id="f6493-124">string</span></span> | <span data-ttu-id="f6493-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f6493-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f6493-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f6493-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f6493-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f6493-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f6493-128">必需。</span><span class="sxs-lookup"><span data-stu-id="f6493-128">Required.</span></span> |

<span data-ttu-id="f6493-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6493-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f6493-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="f6493-130">The default output type is text/csv.</span></span> <span data-ttu-id="f6493-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="f6493-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6493-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6493-132">Request headers</span></span>

| <span data-ttu-id="f6493-133">名称</span><span class="sxs-lookup"><span data-stu-id="f6493-133">Name</span></span>          | <span data-ttu-id="f6493-134">说明</span><span class="sxs-lookup"><span data-stu-id="f6493-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f6493-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6493-135">Authorization</span></span> | <span data-ttu-id="f6493-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6493-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f6493-138">响应</span><span class="sxs-lookup"><span data-stu-id="f6493-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f6493-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f6493-139">CSV</span></span>

<span data-ttu-id="f6493-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f6493-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f6493-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f6493-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f6493-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f6493-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f6493-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f6493-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f6493-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f6493-144">Report Refresh Date</span></span>
- <span data-ttu-id="f6493-145">已发送</span><span class="sxs-lookup"><span data-stu-id="f6493-145">Send</span></span>
- <span data-ttu-id="f6493-146">已接收</span><span class="sxs-lookup"><span data-stu-id="f6493-146">Receive</span></span>
- <span data-ttu-id="f6493-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="f6493-147">Read</span></span>
- <span data-ttu-id="f6493-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="f6493-148">Report Date</span></span>
- <span data-ttu-id="f6493-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="f6493-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f6493-150">JSON</span><span class="sxs-lookup"><span data-stu-id="f6493-150">JSON</span></span>

<span data-ttu-id="f6493-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailActivitySummary](../resources/emailactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="f6493-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6493-152">示例</span><span class="sxs-lookup"><span data-stu-id="f6493-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f6493-153">CSV</span><span class="sxs-lookup"><span data-stu-id="f6493-153">CSV</span></span>

<span data-ttu-id="f6493-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="f6493-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f6493-155">请求</span><span class="sxs-lookup"><span data-stu-id="f6493-155">Request</span></span>

<span data-ttu-id="f6493-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6493-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f6493-157">响应</span><span class="sxs-lookup"><span data-stu-id="f6493-157">Response</span></span>

<span data-ttu-id="f6493-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6493-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f6493-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f6493-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f6493-160">JSON</span><span class="sxs-lookup"><span data-stu-id="f6493-160">JSON</span></span>

<span data-ttu-id="f6493-161">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="f6493-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f6493-162">请求</span><span class="sxs-lookup"><span data-stu-id="f6493-162">Request</span></span>

<span data-ttu-id="f6493-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6493-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f6493-164">响应</span><span class="sxs-lookup"><span data-stu-id="f6493-164">Response</span></span>

<span data-ttu-id="f6493-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f6493-165">The following is an example of the response.</span></span>

> <span data-ttu-id="f6493-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6493-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
