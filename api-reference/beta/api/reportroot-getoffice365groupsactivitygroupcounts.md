---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: 获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9ea971361975113a472670ae68fb94dcc2c153f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964632"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="d2e50-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="d2e50-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

> <span data-ttu-id="d2e50-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2e50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2e50-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2e50-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2e50-106">获取每日总组数和活跃组数（以电子邮件对话、Yammer 帖子和 SharePoint 文件活动为依据）。</span><span class="sxs-lookup"><span data-stu-id="d2e50-106">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="d2e50-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="d2e50-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e50-108">权限</span><span class="sxs-lookup"><span data-stu-id="d2e50-108">Permissions</span></span>

<span data-ttu-id="d2e50-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2e50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2e50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2e50-111">Permission type</span></span>                        | <span data-ttu-id="d2e50-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2e50-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d2e50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e50-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2e50-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2e50-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d2e50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2e50-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2e50-116">Not supported.</span></span>                           |
| <span data-ttu-id="d2e50-117">应用</span><span class="sxs-lookup"><span data-stu-id="d2e50-117">Application</span></span>                            | <span data-ttu-id="d2e50-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2e50-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d2e50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2e50-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d2e50-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d2e50-120">Function parameters</span></span>

<span data-ttu-id="d2e50-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d2e50-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d2e50-122">参数</span><span class="sxs-lookup"><span data-stu-id="d2e50-122">Parameter</span></span> | <span data-ttu-id="d2e50-123">类型</span><span class="sxs-lookup"><span data-stu-id="d2e50-123">Type</span></span>   | <span data-ttu-id="d2e50-124">说明</span><span class="sxs-lookup"><span data-stu-id="d2e50-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d2e50-125">period</span><span class="sxs-lookup"><span data-stu-id="d2e50-125">period</span></span>    | <span data-ttu-id="d2e50-126">string</span><span class="sxs-lookup"><span data-stu-id="d2e50-126">string</span></span> | <span data-ttu-id="d2e50-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d2e50-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d2e50-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d2e50-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d2e50-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d2e50-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d2e50-130">必需。</span><span class="sxs-lookup"><span data-stu-id="d2e50-130">Required.</span></span> |

<span data-ttu-id="d2e50-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d2e50-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d2e50-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="d2e50-132">The default output type is text/csv.</span></span> <span data-ttu-id="d2e50-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="d2e50-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2e50-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2e50-134">Request headers</span></span>

| <span data-ttu-id="d2e50-135">名称</span><span class="sxs-lookup"><span data-stu-id="d2e50-135">Name</span></span>          | <span data-ttu-id="d2e50-136">说明</span><span class="sxs-lookup"><span data-stu-id="d2e50-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d2e50-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2e50-137">Authorization</span></span> | <span data-ttu-id="d2e50-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2e50-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d2e50-140">响应</span><span class="sxs-lookup"><span data-stu-id="d2e50-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d2e50-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d2e50-141">CSV</span></span>

<span data-ttu-id="d2e50-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d2e50-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d2e50-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d2e50-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d2e50-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d2e50-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d2e50-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d2e50-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d2e50-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d2e50-146">Report Refresh Date</span></span>
- <span data-ttu-id="d2e50-147">总计</span><span class="sxs-lookup"><span data-stu-id="d2e50-147">Total</span></span>
- <span data-ttu-id="d2e50-148">活跃</span><span class="sxs-lookup"><span data-stu-id="d2e50-148">Active</span></span>
- <span data-ttu-id="d2e50-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="d2e50-149">Report Date</span></span>
- <span data-ttu-id="d2e50-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="d2e50-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d2e50-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d2e50-151">JSON</span></span>

<span data-ttu-id="d2e50-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d2e50-152">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e50-153">示例</span><span class="sxs-lookup"><span data-stu-id="d2e50-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d2e50-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d2e50-154">CSV</span></span>

<span data-ttu-id="d2e50-155">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="d2e50-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d2e50-156">请求</span><span class="sxs-lookup"><span data-stu-id="d2e50-156">Request</span></span>

<span data-ttu-id="d2e50-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2e50-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d2e50-158">响应</span><span class="sxs-lookup"><span data-stu-id="d2e50-158">Response</span></span>

<span data-ttu-id="d2e50-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2e50-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d2e50-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d2e50-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="d2e50-161">JSON</span><span class="sxs-lookup"><span data-stu-id="d2e50-161">JSON</span></span>

<span data-ttu-id="d2e50-162">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d2e50-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d2e50-163">请求</span><span class="sxs-lookup"><span data-stu-id="d2e50-163">Request</span></span>

<span data-ttu-id="d2e50-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2e50-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d2e50-165">响应</span><span class="sxs-lookup"><span data-stu-id="d2e50-165">Response</span></span>

<span data-ttu-id="d2e50-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2e50-166">The following is an example of the response.</span></span>

> <span data-ttu-id="d2e50-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d2e50-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 5344, 
      "active": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
