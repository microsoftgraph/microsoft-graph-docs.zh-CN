---
title: 'reportRoot: getSharePointSiteUsagePages'
description: 获取跨所有网站浏览的页面数。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d8194e26ff60ae925100b9d77cf18145218d465c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914218"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="dc61b-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="dc61b-103">reportRoot: getSharePointSiteUsagePages</span></span>

<span data-ttu-id="dc61b-104">获取跨所有网站浏览的页面数。</span><span class="sxs-lookup"><span data-stu-id="dc61b-104">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="dc61b-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="dc61b-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc61b-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc61b-106">Permissions</span></span>

<span data-ttu-id="dc61b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc61b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc61b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc61b-109">Permission type</span></span>                        | <span data-ttu-id="dc61b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc61b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dc61b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc61b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc61b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc61b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dc61b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc61b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc61b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc61b-114">Not supported.</span></span>                           |
| <span data-ttu-id="dc61b-115">应用</span><span class="sxs-lookup"><span data-stu-id="dc61b-115">Application</span></span>                            | <span data-ttu-id="dc61b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc61b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dc61b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc61b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dc61b-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="dc61b-118">Function parameters</span></span>

<span data-ttu-id="dc61b-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="dc61b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dc61b-120">参数</span><span class="sxs-lookup"><span data-stu-id="dc61b-120">Parameter</span></span> | <span data-ttu-id="dc61b-121">类型</span><span class="sxs-lookup"><span data-stu-id="dc61b-121">Type</span></span>   | <span data-ttu-id="dc61b-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc61b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dc61b-123">period</span><span class="sxs-lookup"><span data-stu-id="dc61b-123">period</span></span>    | <span data-ttu-id="dc61b-124">string</span><span class="sxs-lookup"><span data-stu-id="dc61b-124">string</span></span> | <span data-ttu-id="dc61b-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dc61b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dc61b-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="dc61b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dc61b-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dc61b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dc61b-128">必需。</span><span class="sxs-lookup"><span data-stu-id="dc61b-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dc61b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc61b-129">Request headers</span></span>

| <span data-ttu-id="dc61b-130">名称</span><span class="sxs-lookup"><span data-stu-id="dc61b-130">Name</span></span>          | <span data-ttu-id="dc61b-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc61b-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dc61b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc61b-132">Authorization</span></span> | <span data-ttu-id="dc61b-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc61b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dc61b-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dc61b-135">If-None-Match</span></span> | <span data-ttu-id="dc61b-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dc61b-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dc61b-137">可选。</span><span class="sxs-lookup"><span data-stu-id="dc61b-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dc61b-138">响应</span><span class="sxs-lookup"><span data-stu-id="dc61b-138">Response</span></span>

<span data-ttu-id="dc61b-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="dc61b-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dc61b-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="dc61b-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dc61b-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="dc61b-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dc61b-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="dc61b-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dc61b-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="dc61b-143">Report Refresh Date</span></span>
- <span data-ttu-id="dc61b-144">网站类型</span><span class="sxs-lookup"><span data-stu-id="dc61b-144">Site Type</span></span>
- <span data-ttu-id="dc61b-145">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="dc61b-145">Page View Count</span></span>
- <span data-ttu-id="dc61b-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="dc61b-146">Report Date</span></span>
- <span data-ttu-id="dc61b-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="dc61b-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dc61b-148">示例</span><span class="sxs-lookup"><span data-stu-id="dc61b-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dc61b-149">请求</span><span class="sxs-lookup"><span data-stu-id="dc61b-149">Request</span></span>

<span data-ttu-id="dc61b-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dc61b-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagepages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsagePages(period='D7')
```

#### <a name="response"></a><span data-ttu-id="dc61b-151">响应</span><span class="sxs-lookup"><span data-stu-id="dc61b-151">Response</span></span>

<span data-ttu-id="dc61b-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dc61b-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="dc61b-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="dc61b-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```
