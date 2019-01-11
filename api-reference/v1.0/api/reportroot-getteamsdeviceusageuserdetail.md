---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.openlocfilehash: 8e3f19d0e95c5b69109787208b4d75613922bd91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840801"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="23b77-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="23b77-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="23b77-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23b77-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="23b77-105">权限</span><span class="sxs-lookup"><span data-stu-id="23b77-105">Permissions</span></span>

<span data-ttu-id="23b77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23b77-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23b77-108">Permission type</span></span>                        | <span data-ttu-id="23b77-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23b77-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23b77-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23b77-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23b77-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b77-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23b77-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23b77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b77-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="23b77-113">Not supported.</span></span>                           |
| <span data-ttu-id="23b77-114">应用</span><span class="sxs-lookup"><span data-stu-id="23b77-114">Application</span></span>                            | <span data-ttu-id="23b77-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23b77-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="23b77-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23b77-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="23b77-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="23b77-117">Function parameters</span></span>

<span data-ttu-id="23b77-118">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="23b77-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="23b77-119">参数</span><span class="sxs-lookup"><span data-stu-id="23b77-119">Parameter</span></span> | <span data-ttu-id="23b77-120">类型</span><span class="sxs-lookup"><span data-stu-id="23b77-120">Type</span></span>   | <span data-ttu-id="23b77-121">说明</span><span class="sxs-lookup"><span data-stu-id="23b77-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23b77-122">period</span><span class="sxs-lookup"><span data-stu-id="23b77-122">period</span></span>    | <span data-ttu-id="23b77-123">string</span><span class="sxs-lookup"><span data-stu-id="23b77-123">string</span></span> | <span data-ttu-id="23b77-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="23b77-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23b77-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="23b77-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23b77-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="23b77-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="23b77-127">date</span><span class="sxs-lookup"><span data-stu-id="23b77-127">date</span></span>      | <span data-ttu-id="23b77-128">Date</span><span class="sxs-lookup"><span data-stu-id="23b77-128">Date</span></span>   | <span data-ttu-id="23b77-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="23b77-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="23b77-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="23b77-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="23b77-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="23b77-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="23b77-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="23b77-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b77-133">请求头</span><span class="sxs-lookup"><span data-stu-id="23b77-133">Request headers</span></span>

| <span data-ttu-id="23b77-134">名称</span><span class="sxs-lookup"><span data-stu-id="23b77-134">Name</span></span>          | <span data-ttu-id="23b77-135">说明</span><span class="sxs-lookup"><span data-stu-id="23b77-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23b77-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="23b77-136">Authorization</span></span> | <span data-ttu-id="23b77-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23b77-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23b77-139">响应</span><span class="sxs-lookup"><span data-stu-id="23b77-139">Response</span></span>

<span data-ttu-id="23b77-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="23b77-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23b77-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="23b77-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23b77-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="23b77-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23b77-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="23b77-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="23b77-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="23b77-144">Report Refresh Date</span></span>
- <span data-ttu-id="23b77-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="23b77-145">User Principal Name</span></span>
- <span data-ttu-id="23b77-146">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="23b77-146">Last Activity Date</span></span>
- <span data-ttu-id="23b77-147">已删除</span><span class="sxs-lookup"><span data-stu-id="23b77-147">Is Deleted</span></span>
- <span data-ttu-id="23b77-148">删除日期</span><span class="sxs-lookup"><span data-stu-id="23b77-148">Deleted Date</span></span>
- <span data-ttu-id="23b77-149">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="23b77-149">Used Web</span></span>
- <span data-ttu-id="23b77-150">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="23b77-150">Used Windows Phone</span></span>
- <span data-ttu-id="23b77-151">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="23b77-151">Used iOS</span></span>
- <span data-ttu-id="23b77-152">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="23b77-152">Used Mac</span></span>
- <span data-ttu-id="23b77-153">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="23b77-153">Used Android Phone</span></span>
- <span data-ttu-id="23b77-154">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="23b77-154">Used Windows</span></span>
- <span data-ttu-id="23b77-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="23b77-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="23b77-156">示例</span><span class="sxs-lookup"><span data-stu-id="23b77-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="23b77-157">请求</span><span class="sxs-lookup"><span data-stu-id="23b77-157">Request</span></span>

<span data-ttu-id="23b77-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="23b77-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="23b77-159">响应</span><span class="sxs-lookup"><span data-stu-id="23b77-159">Response</span></span>

<span data-ttu-id="23b77-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="23b77-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="23b77-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="23b77-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```
