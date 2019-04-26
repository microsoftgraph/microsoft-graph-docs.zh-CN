---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c8834d59abd186a6a9c20b6ef4a3a6c6674bffba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336741"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="c17cf-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="c17cf-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c17cf-104">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="c17cf-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="c17cf-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="c17cf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c17cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="c17cf-106">Permissions</span></span>

<span data-ttu-id="c17cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c17cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c17cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c17cf-109">Permission type</span></span>                        | <span data-ttu-id="c17cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c17cf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c17cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c17cf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c17cf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c17cf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c17cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c17cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c17cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c17cf-114">Not supported.</span></span>                           |
| <span data-ttu-id="c17cf-115">应用</span><span class="sxs-lookup"><span data-stu-id="c17cf-115">Application</span></span>                            | <span data-ttu-id="c17cf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c17cf-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c17cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c17cf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c17cf-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="c17cf-118">Function parameters</span></span>

<span data-ttu-id="c17cf-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c17cf-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c17cf-120">参数</span><span class="sxs-lookup"><span data-stu-id="c17cf-120">Parameter</span></span> | <span data-ttu-id="c17cf-121">类型</span><span class="sxs-lookup"><span data-stu-id="c17cf-121">Type</span></span>   | <span data-ttu-id="c17cf-122">说明</span><span class="sxs-lookup"><span data-stu-id="c17cf-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c17cf-123">period</span><span class="sxs-lookup"><span data-stu-id="c17cf-123">period</span></span>    | <span data-ttu-id="c17cf-124">string</span><span class="sxs-lookup"><span data-stu-id="c17cf-124">string</span></span> | <span data-ttu-id="c17cf-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c17cf-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c17cf-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c17cf-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c17cf-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c17cf-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c17cf-128">必需。</span><span class="sxs-lookup"><span data-stu-id="c17cf-128">Required.</span></span> |

<span data-ttu-id="c17cf-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c17cf-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c17cf-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="c17cf-130">The default output type is text/csv.</span></span> <span data-ttu-id="c17cf-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="c17cf-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c17cf-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="c17cf-132">Request headers</span></span>

| <span data-ttu-id="c17cf-133">名称</span><span class="sxs-lookup"><span data-stu-id="c17cf-133">Name</span></span>          | <span data-ttu-id="c17cf-134">说明</span><span class="sxs-lookup"><span data-stu-id="c17cf-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c17cf-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c17cf-135">Authorization</span></span> | <span data-ttu-id="c17cf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c17cf-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c17cf-138">响应</span><span class="sxs-lookup"><span data-stu-id="c17cf-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c17cf-139">CSV</span><span class="sxs-lookup"><span data-stu-id="c17cf-139">CSV</span></span>

<span data-ttu-id="c17cf-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c17cf-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c17cf-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c17cf-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c17cf-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="c17cf-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c17cf-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="c17cf-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c17cf-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c17cf-144">Report Refresh Date</span></span>
- <span data-ttu-id="c17cf-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="c17cf-145">Office 365</span></span>
- <span data-ttu-id="c17cf-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="c17cf-146">Exchange</span></span>
- <span data-ttu-id="c17cf-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="c17cf-147">OneDrive</span></span>
- <span data-ttu-id="c17cf-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="c17cf-148">SharePoint</span></span>
- <span data-ttu-id="c17cf-149">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="c17cf-149">Skype For Business</span></span> 
- <span data-ttu-id="c17cf-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="c17cf-150">Yammer</span></span>
- <span data-ttu-id="c17cf-151">Teams</span><span class="sxs-lookup"><span data-stu-id="c17cf-151">Teams</span></span>
- <span data-ttu-id="c17cf-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="c17cf-152">Report Date</span></span>
- <span data-ttu-id="c17cf-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="c17cf-153">Report Period</span></span>

<span data-ttu-id="c17cf-154">由世纪互联运营的 Microsoft Graph 中国不支持以下各列:</span><span class="sxs-lookup"><span data-stu-id="c17cf-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c17cf-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="c17cf-155">Yammer</span></span>
- <span data-ttu-id="c17cf-156">Teams</span><span class="sxs-lookup"><span data-stu-id="c17cf-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="c17cf-157">JSON</span><span class="sxs-lookup"><span data-stu-id="c17cf-157">JSON</span></span>

<span data-ttu-id="c17cf-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="c17cf-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="c17cf-159">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象中的以下属性:</span><span class="sxs-lookup"><span data-stu-id="c17cf-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="c17cf-160">yammer</span><span class="sxs-lookup"><span data-stu-id="c17cf-160">yammer</span></span>
- <span data-ttu-id="c17cf-161">协作</span><span class="sxs-lookup"><span data-stu-id="c17cf-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="c17cf-162">示例</span><span class="sxs-lookup"><span data-stu-id="c17cf-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c17cf-163">CSV</span><span class="sxs-lookup"><span data-stu-id="c17cf-163">CSV</span></span>

<span data-ttu-id="c17cf-164">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="c17cf-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c17cf-165">请求</span><span class="sxs-lookup"><span data-stu-id="c17cf-165">Request</span></span>

<span data-ttu-id="c17cf-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c17cf-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c17cf-167">响应</span><span class="sxs-lookup"><span data-stu-id="c17cf-167">Response</span></span>

<span data-ttu-id="c17cf-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c17cf-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c17cf-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c17cf-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="c17cf-170">JSON</span><span class="sxs-lookup"><span data-stu-id="c17cf-170">JSON</span></span>

<span data-ttu-id="c17cf-171">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="c17cf-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c17cf-172">请求</span><span class="sxs-lookup"><span data-stu-id="c17cf-172">Request</span></span>

<span data-ttu-id="c17cf-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c17cf-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c17cf-174">响应</span><span class="sxs-lookup"><span data-stu-id="c17cf-174">Response</span></span>

<span data-ttu-id="c17cf-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c17cf-175">The following is an example of the response.</span></span>

> <span data-ttu-id="c17cf-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c17cf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
```
