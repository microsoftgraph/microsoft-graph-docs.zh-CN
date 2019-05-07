---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 440b766b9f1790945ee31b29b3d2228b40f61198
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604090"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="f2dbf-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="f2dbf-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="f2dbf-104">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2dbf-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2dbf-105">Permissions</span></span>

<span data-ttu-id="f2dbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2dbf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2dbf-108">Permission type</span></span>                        | <span data-ttu-id="f2dbf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2dbf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f2dbf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2dbf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2dbf-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2dbf-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f2dbf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2dbf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-113">Not supported.</span></span>                           |
| <span data-ttu-id="f2dbf-114">应用</span><span class="sxs-lookup"><span data-stu-id="f2dbf-114">Application</span></span>                            | <span data-ttu-id="f2dbf-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2dbf-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f2dbf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2dbf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f2dbf-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="f2dbf-117">Function parameters</span></span>

<span data-ttu-id="f2dbf-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f2dbf-119">参数</span><span class="sxs-lookup"><span data-stu-id="f2dbf-119">Parameter</span></span> | <span data-ttu-id="f2dbf-120">类型</span><span class="sxs-lookup"><span data-stu-id="f2dbf-120">Type</span></span>   | <span data-ttu-id="f2dbf-121">说明</span><span class="sxs-lookup"><span data-stu-id="f2dbf-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f2dbf-122">period</span><span class="sxs-lookup"><span data-stu-id="f2dbf-122">period</span></span>    | <span data-ttu-id="f2dbf-123">string</span><span class="sxs-lookup"><span data-stu-id="f2dbf-123">string</span></span> | <span data-ttu-id="f2dbf-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f2dbf-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f2dbf-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f2dbf-127">必需。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f2dbf-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2dbf-128">Request headers</span></span>

| <span data-ttu-id="f2dbf-129">名称</span><span class="sxs-lookup"><span data-stu-id="f2dbf-129">Name</span></span>          | <span data-ttu-id="f2dbf-130">说明</span><span class="sxs-lookup"><span data-stu-id="f2dbf-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f2dbf-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2dbf-131">Authorization</span></span> | <span data-ttu-id="f2dbf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f2dbf-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2dbf-134">Response</span></span>

<span data-ttu-id="f2dbf-135">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f2dbf-136">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f2dbf-137">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f2dbf-138">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="f2dbf-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="f2dbf-139">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f2dbf-139">Report Refresh Date</span></span>
- <span data-ttu-id="f2dbf-140">Web</span><span class="sxs-lookup"><span data-stu-id="f2dbf-140">Web</span></span>
- <span data-ttu-id="f2dbf-141">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="f2dbf-141">Windows Phone</span></span>
- <span data-ttu-id="f2dbf-142">Android 手机</span><span class="sxs-lookup"><span data-stu-id="f2dbf-142">Android Phone</span></span>
- <span data-ttu-id="f2dbf-143">iOS</span><span class="sxs-lookup"><span data-stu-id="f2dbf-143">iOS</span></span>
- <span data-ttu-id="f2dbf-144">Mac</span><span class="sxs-lookup"><span data-stu-id="f2dbf-144">Mac</span></span>
- <span data-ttu-id="f2dbf-145">Windows</span><span class="sxs-lookup"><span data-stu-id="f2dbf-145">Windows</span></span>
- <span data-ttu-id="f2dbf-146">报表周期</span><span class="sxs-lookup"><span data-stu-id="f2dbf-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f2dbf-147">示例</span><span class="sxs-lookup"><span data-stu-id="f2dbf-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f2dbf-148">请求</span><span class="sxs-lookup"><span data-stu-id="f2dbf-148">Request</span></span>

<span data-ttu-id="f2dbf-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f2dbf-150">响应</span><span class="sxs-lookup"><span data-stu-id="f2dbf-150">Response</span></span>

<span data-ttu-id="f2dbf-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-151">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2dbf-152">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f2dbf-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2dbf-153">语言</span><span class="sxs-lookup"><span data-stu-id="f2dbf-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2dbf-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2dbf-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f2dbf-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f2dbf-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
