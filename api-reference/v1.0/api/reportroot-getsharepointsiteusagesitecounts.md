---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c4b9e5c24bc30e73336941f0a5fe9cee571bf879
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957968"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="4adc0-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="4adc0-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="4adc0-105">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="4adc0-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="4adc0-106">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="4adc0-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="4adc0-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="4adc0-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="4adc0-108">权限</span><span class="sxs-lookup"><span data-stu-id="4adc0-108">Permissions</span></span>

<span data-ttu-id="4adc0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4adc0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4adc0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4adc0-111">Permission type</span></span>                        | <span data-ttu-id="4adc0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4adc0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4adc0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4adc0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4adc0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4adc0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4adc0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4adc0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4adc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4adc0-116">Not supported.</span></span>                           |
| <span data-ttu-id="4adc0-117">应用</span><span class="sxs-lookup"><span data-stu-id="4adc0-117">Application</span></span>                            | <span data-ttu-id="4adc0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4adc0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4adc0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4adc0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4adc0-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="4adc0-120">Function parameters</span></span>

<span data-ttu-id="4adc0-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4adc0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4adc0-122">参数</span><span class="sxs-lookup"><span data-stu-id="4adc0-122">Parameter</span></span> | <span data-ttu-id="4adc0-123">类型</span><span class="sxs-lookup"><span data-stu-id="4adc0-123">Type</span></span>   | <span data-ttu-id="4adc0-124">说明</span><span class="sxs-lookup"><span data-stu-id="4adc0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4adc0-125">period</span><span class="sxs-lookup"><span data-stu-id="4adc0-125">period</span></span>    | <span data-ttu-id="4adc0-126">string</span><span class="sxs-lookup"><span data-stu-id="4adc0-126">string</span></span> | <span data-ttu-id="4adc0-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4adc0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4adc0-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4adc0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4adc0-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4adc0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4adc0-130">必需。</span><span class="sxs-lookup"><span data-stu-id="4adc0-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4adc0-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="4adc0-131">Request headers</span></span>

| <span data-ttu-id="4adc0-132">名称</span><span class="sxs-lookup"><span data-stu-id="4adc0-132">Name</span></span>          | <span data-ttu-id="4adc0-133">说明</span><span class="sxs-lookup"><span data-stu-id="4adc0-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4adc0-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="4adc0-134">Authorization</span></span> | <span data-ttu-id="4adc0-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="4adc0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4adc0-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4adc0-137">If-None-Match</span></span> | <span data-ttu-id="4adc0-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4adc0-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4adc0-139">可选。</span><span class="sxs-lookup"><span data-stu-id="4adc0-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4adc0-140">响应</span><span class="sxs-lookup"><span data-stu-id="4adc0-140">Response</span></span>

<span data-ttu-id="4adc0-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4adc0-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4adc0-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4adc0-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4adc0-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4adc0-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4adc0-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4adc0-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4adc0-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4adc0-145">Report Refresh Date</span></span>
- <span data-ttu-id="4adc0-146">网站类型</span><span class="sxs-lookup"><span data-stu-id="4adc0-146">Site Type</span></span>
- <span data-ttu-id="4adc0-147">总计</span><span class="sxs-lookup"><span data-stu-id="4adc0-147">Total</span></span>
- <span data-ttu-id="4adc0-148">活跃</span><span class="sxs-lookup"><span data-stu-id="4adc0-148">Active</span></span>
- <span data-ttu-id="4adc0-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="4adc0-149">Report Date</span></span>
- <span data-ttu-id="4adc0-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="4adc0-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4adc0-151">示例</span><span class="sxs-lookup"><span data-stu-id="4adc0-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4adc0-152">请求</span><span class="sxs-lookup"><span data-stu-id="4adc0-152">Request</span></span>

<span data-ttu-id="4adc0-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4adc0-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4adc0-154">响应</span><span class="sxs-lookup"><span data-stu-id="4adc0-154">Response</span></span>

<span data-ttu-id="4adc0-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4adc0-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="4adc0-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4adc0-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
