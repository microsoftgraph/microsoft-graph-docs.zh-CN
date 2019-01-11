---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: 获取用户执行的 OneDrive 活动的详细信息。
localization_priority: Normal
ms.openlocfilehash: 279c7f4e417b9314d0ed7b6a5dbcf85454d4f0c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826423"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="4dd47-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4dd47-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="4dd47-104">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4dd47-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="4dd47-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="4dd47-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="4dd47-106">权限</span><span class="sxs-lookup"><span data-stu-id="4dd47-106">Permissions</span></span>

<span data-ttu-id="4dd47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dd47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4dd47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dd47-109">Permission type</span></span>                        | <span data-ttu-id="4dd47-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dd47-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4dd47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4dd47-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4dd47-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4dd47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dd47-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dd47-114">Not supported.</span></span>                           |
| <span data-ttu-id="4dd47-115">应用</span><span class="sxs-lookup"><span data-stu-id="4dd47-115">Application</span></span>                            | <span data-ttu-id="4dd47-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4dd47-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4dd47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dd47-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4dd47-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="4dd47-118">Function parameters</span></span>

<span data-ttu-id="4dd47-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="4dd47-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4dd47-120">参数</span><span class="sxs-lookup"><span data-stu-id="4dd47-120">Parameter</span></span> | <span data-ttu-id="4dd47-121">类型</span><span class="sxs-lookup"><span data-stu-id="4dd47-121">Type</span></span>   | <span data-ttu-id="4dd47-122">说明</span><span class="sxs-lookup"><span data-stu-id="4dd47-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4dd47-123">period</span><span class="sxs-lookup"><span data-stu-id="4dd47-123">period</span></span>    | <span data-ttu-id="4dd47-124">string</span><span class="sxs-lookup"><span data-stu-id="4dd47-124">string</span></span> | <span data-ttu-id="4dd47-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4dd47-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4dd47-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4dd47-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4dd47-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4dd47-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4dd47-128">date</span><span class="sxs-lookup"><span data-stu-id="4dd47-128">date</span></span>      | <span data-ttu-id="4dd47-129">Date</span><span class="sxs-lookup"><span data-stu-id="4dd47-129">Date</span></span>   | <span data-ttu-id="4dd47-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="4dd47-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4dd47-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="4dd47-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4dd47-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="4dd47-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4dd47-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="4dd47-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dd47-134">请求头</span><span class="sxs-lookup"><span data-stu-id="4dd47-134">Request headers</span></span>

| <span data-ttu-id="4dd47-135">名称</span><span class="sxs-lookup"><span data-stu-id="4dd47-135">Name</span></span>          | <span data-ttu-id="4dd47-136">说明</span><span class="sxs-lookup"><span data-stu-id="4dd47-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4dd47-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dd47-137">Authorization</span></span> | <span data-ttu-id="4dd47-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dd47-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4dd47-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4dd47-140">If-None-Match</span></span> | <span data-ttu-id="4dd47-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4dd47-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4dd47-142">可选。</span><span class="sxs-lookup"><span data-stu-id="4dd47-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4dd47-143">响应</span><span class="sxs-lookup"><span data-stu-id="4dd47-143">Response</span></span>

<span data-ttu-id="4dd47-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4dd47-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4dd47-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4dd47-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4dd47-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4dd47-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4dd47-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4dd47-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4dd47-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4dd47-148">Report Refresh Date</span></span>
- <span data-ttu-id="4dd47-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4dd47-149">User Principal Name</span></span>
- <span data-ttu-id="4dd47-150">已删除</span><span class="sxs-lookup"><span data-stu-id="4dd47-150">Is Deleted</span></span>
- <span data-ttu-id="4dd47-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="4dd47-151">Deleted Date</span></span>
- <span data-ttu-id="4dd47-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="4dd47-152">Last Activity Date</span></span>
- <span data-ttu-id="4dd47-153">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="4dd47-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="4dd47-154">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="4dd47-154">Synced File Count</span></span>
- <span data-ttu-id="4dd47-155">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="4dd47-155">Shared Internally File Count</span></span>
- <span data-ttu-id="4dd47-156">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="4dd47-156">Shared Externally File Count</span></span>
- <span data-ttu-id="4dd47-157">分配的产品</span><span class="sxs-lookup"><span data-stu-id="4dd47-157">Assigned Products</span></span>
- <span data-ttu-id="4dd47-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="4dd47-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4dd47-159">示例</span><span class="sxs-lookup"><span data-stu-id="4dd47-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4dd47-160">请求</span><span class="sxs-lookup"><span data-stu-id="4dd47-160">Request</span></span>

<span data-ttu-id="4dd47-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4dd47-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4dd47-162">响应</span><span class="sxs-lookup"><span data-stu-id="4dd47-162">Response</span></span>

<span data-ttu-id="4dd47-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4dd47-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4dd47-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4dd47-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
