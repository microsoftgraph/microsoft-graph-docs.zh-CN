---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: 获取用户的 Skype for Business 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9f76f961093f91f2e058fe84321b2c1c62dcb40d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44893646"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="11b96-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="11b96-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="11b96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11b96-105">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="11b96-105">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="11b96-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-使用的 Skype For business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="11b96-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="11b96-107">权限</span><span class="sxs-lookup"><span data-stu-id="11b96-107">Permissions</span></span>

<span data-ttu-id="11b96-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="11b96-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="11b96-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b96-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11b96-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11b96-110">Permission type</span></span>                        | <span data-ttu-id="11b96-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11b96-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11b96-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11b96-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="11b96-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11b96-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11b96-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11b96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b96-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11b96-115">Not supported.</span></span>                           |
| <span data-ttu-id="11b96-116">应用</span><span class="sxs-lookup"><span data-stu-id="11b96-116">Application</span></span>                            | <span data-ttu-id="11b96-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11b96-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="11b96-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="11b96-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="11b96-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="11b96-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="11b96-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11b96-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="11b96-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="11b96-121">Function parameters</span></span>

<span data-ttu-id="11b96-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="11b96-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="11b96-123">参数</span><span class="sxs-lookup"><span data-stu-id="11b96-123">Parameter</span></span> | <span data-ttu-id="11b96-124">类型</span><span class="sxs-lookup"><span data-stu-id="11b96-124">Type</span></span>   | <span data-ttu-id="11b96-125">说明</span><span class="sxs-lookup"><span data-stu-id="11b96-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11b96-126">period</span><span class="sxs-lookup"><span data-stu-id="11b96-126">period</span></span>    | <span data-ttu-id="11b96-127">string</span><span class="sxs-lookup"><span data-stu-id="11b96-127">string</span></span> | <span data-ttu-id="11b96-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="11b96-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11b96-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="11b96-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11b96-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="11b96-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="11b96-131">date</span><span class="sxs-lookup"><span data-stu-id="11b96-131">date</span></span>      | <span data-ttu-id="11b96-132">Date</span><span class="sxs-lookup"><span data-stu-id="11b96-132">Date</span></span>   | <span data-ttu-id="11b96-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="11b96-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="11b96-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="11b96-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="11b96-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="11b96-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="11b96-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="11b96-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11b96-137">请求头</span><span class="sxs-lookup"><span data-stu-id="11b96-137">Request headers</span></span>

| <span data-ttu-id="11b96-138">名称</span><span class="sxs-lookup"><span data-stu-id="11b96-138">Name</span></span>          | <span data-ttu-id="11b96-139">说明</span><span class="sxs-lookup"><span data-stu-id="11b96-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="11b96-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="11b96-140">Authorization</span></span> | <span data-ttu-id="11b96-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="11b96-141">Bearer {token}.</span></span> <span data-ttu-id="11b96-142">Required.</span><span class="sxs-lookup"><span data-stu-id="11b96-142">Required.</span></span>                |
| <span data-ttu-id="11b96-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="11b96-143">If-None-Match</span></span> | <span data-ttu-id="11b96-144">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="11b96-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="11b96-145">可选。</span><span class="sxs-lookup"><span data-stu-id="11b96-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="11b96-146">响应</span><span class="sxs-lookup"><span data-stu-id="11b96-146">Response</span></span>

<span data-ttu-id="11b96-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="11b96-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11b96-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="11b96-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11b96-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="11b96-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11b96-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="11b96-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11b96-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="11b96-151">Report Refresh Date</span></span>
- <span data-ttu-id="11b96-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="11b96-152">User Principal Name</span></span>
- <span data-ttu-id="11b96-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="11b96-153">Last Activity Date</span></span>
- <span data-ttu-id="11b96-154">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="11b96-154">Used Windows</span></span>
- <span data-ttu-id="11b96-155">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="11b96-155">Used Windows Phone</span></span>
- <span data-ttu-id="11b96-156">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="11b96-156">Used Android Phone</span></span>
- <span data-ttu-id="11b96-157">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="11b96-157">Used iPhone</span></span>
- <span data-ttu-id="11b96-158">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="11b96-158">Used iPad</span></span>
- <span data-ttu-id="11b96-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="11b96-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="11b96-160">示例</span><span class="sxs-lookup"><span data-stu-id="11b96-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11b96-161">请求</span><span class="sxs-lookup"><span data-stu-id="11b96-161">Request</span></span>

<span data-ttu-id="11b96-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11b96-162">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="11b96-163">响应</span><span class="sxs-lookup"><span data-stu-id="11b96-163">Response</span></span>

<span data-ttu-id="11b96-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11b96-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="11b96-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="11b96-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
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
