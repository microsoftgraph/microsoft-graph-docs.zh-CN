---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。
ms.openlocfilehash: e467fac8d6836df002e6c8f13cd3a9fab207b8c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011711"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="ee929-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="ee929-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="ee929-105">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="ee929-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="ee929-106">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="ee929-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="ee929-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="ee929-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee929-108">权限</span><span class="sxs-lookup"><span data-stu-id="ee929-108">Permissions</span></span>

<span data-ttu-id="ee929-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee929-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee929-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee929-111">Permission type</span></span>                        | <span data-ttu-id="ee929-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee929-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee929-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee929-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee929-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee929-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee929-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee929-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee929-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee929-116">Not supported.</span></span>                           |
| <span data-ttu-id="ee929-117">应用</span><span class="sxs-lookup"><span data-stu-id="ee929-117">Application</span></span>                            | <span data-ttu-id="ee929-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee929-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee929-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee929-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ee929-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="ee929-120">Function parameters</span></span>

<span data-ttu-id="ee929-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ee929-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ee929-122">参数</span><span class="sxs-lookup"><span data-stu-id="ee929-122">Parameter</span></span> | <span data-ttu-id="ee929-123">类型</span><span class="sxs-lookup"><span data-stu-id="ee929-123">Type</span></span>   | <span data-ttu-id="ee929-124">说明</span><span class="sxs-lookup"><span data-stu-id="ee929-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee929-125">period</span><span class="sxs-lookup"><span data-stu-id="ee929-125">period</span></span>    | <span data-ttu-id="ee929-126">string</span><span class="sxs-lookup"><span data-stu-id="ee929-126">string</span></span> | <span data-ttu-id="ee929-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ee929-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee929-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ee929-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee929-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ee929-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ee929-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ee929-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ee929-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee929-131">Request headers</span></span>

| <span data-ttu-id="ee929-132">名称</span><span class="sxs-lookup"><span data-stu-id="ee929-132">Name</span></span>          | <span data-ttu-id="ee929-133">说明</span><span class="sxs-lookup"><span data-stu-id="ee929-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ee929-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee929-134">Authorization</span></span> | <span data-ttu-id="ee929-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee929-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ee929-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ee929-137">If-None-Match</span></span> | <span data-ttu-id="ee929-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ee929-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ee929-139">可选。</span><span class="sxs-lookup"><span data-stu-id="ee929-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ee929-140">响应</span><span class="sxs-lookup"><span data-stu-id="ee929-140">Response</span></span>

<span data-ttu-id="ee929-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ee929-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee929-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ee929-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee929-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ee929-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee929-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ee929-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee929-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ee929-145">Report Refresh Date</span></span>
- <span data-ttu-id="ee929-146">网站类型</span><span class="sxs-lookup"><span data-stu-id="ee929-146">Site Type</span></span>
- <span data-ttu-id="ee929-147">总计</span><span class="sxs-lookup"><span data-stu-id="ee929-147">Total</span></span>
- <span data-ttu-id="ee929-148">活跃</span><span class="sxs-lookup"><span data-stu-id="ee929-148">Active</span></span>
- <span data-ttu-id="ee929-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="ee929-149">Report Date</span></span>
- <span data-ttu-id="ee929-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="ee929-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ee929-151">示例</span><span class="sxs-lookup"><span data-stu-id="ee929-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee929-152">请求</span><span class="sxs-lookup"><span data-stu-id="ee929-152">Request</span></span>

<span data-ttu-id="ee929-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee929-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ee929-154">响应</span><span class="sxs-lookup"><span data-stu-id="ee929-154">Response</span></span>

<span data-ttu-id="ee929-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee929-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="ee929-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ee929-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
