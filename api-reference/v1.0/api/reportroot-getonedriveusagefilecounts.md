---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f53a0c980e163996eaef5cc2f7a0574c53a32aee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083188"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="e3034-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="e3034-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="e3034-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3034-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3034-106">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="e3034-106">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="e3034-107">如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。</span><span class="sxs-lookup"><span data-stu-id="e3034-107">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="e3034-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-OneDrive For business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="e3034-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3034-109">权限</span><span class="sxs-lookup"><span data-stu-id="e3034-109">Permissions</span></span>

<span data-ttu-id="e3034-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3034-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3034-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3034-112">Permission type</span></span>                        | <span data-ttu-id="e3034-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3034-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e3034-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3034-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3034-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3034-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e3034-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3034-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3034-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3034-117">Not supported.</span></span>                           |
| <span data-ttu-id="e3034-118">应用</span><span class="sxs-lookup"><span data-stu-id="e3034-118">Application</span></span>                            | <span data-ttu-id="e3034-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3034-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="e3034-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e3034-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e3034-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="e3034-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e3034-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3034-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e3034-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="e3034-123">Function parameters</span></span>

<span data-ttu-id="e3034-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e3034-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e3034-125">参数</span><span class="sxs-lookup"><span data-stu-id="e3034-125">Parameter</span></span> | <span data-ttu-id="e3034-126">类型</span><span class="sxs-lookup"><span data-stu-id="e3034-126">Type</span></span>   | <span data-ttu-id="e3034-127">说明</span><span class="sxs-lookup"><span data-stu-id="e3034-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e3034-128">period</span><span class="sxs-lookup"><span data-stu-id="e3034-128">period</span></span>    | <span data-ttu-id="e3034-129">string</span><span class="sxs-lookup"><span data-stu-id="e3034-129">string</span></span> | <span data-ttu-id="e3034-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e3034-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e3034-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e3034-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e3034-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e3034-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e3034-133">必需。</span><span class="sxs-lookup"><span data-stu-id="e3034-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e3034-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3034-134">Request headers</span></span>

| <span data-ttu-id="e3034-135">名称</span><span class="sxs-lookup"><span data-stu-id="e3034-135">Name</span></span>          | <span data-ttu-id="e3034-136">说明</span><span class="sxs-lookup"><span data-stu-id="e3034-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e3034-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3034-137">Authorization</span></span> | <span data-ttu-id="e3034-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3034-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e3034-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e3034-140">If-None-Match</span></span> | <span data-ttu-id="e3034-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e3034-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e3034-142">可选。</span><span class="sxs-lookup"><span data-stu-id="e3034-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e3034-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3034-143">Response</span></span>

<span data-ttu-id="e3034-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e3034-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e3034-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e3034-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e3034-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e3034-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e3034-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e3034-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e3034-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e3034-148">Report Refresh Date</span></span>
- <span data-ttu-id="e3034-149">网站类型</span><span class="sxs-lookup"><span data-stu-id="e3034-149">Site Type</span></span>
- <span data-ttu-id="e3034-150">总计</span><span class="sxs-lookup"><span data-stu-id="e3034-150">Total</span></span>
- <span data-ttu-id="e3034-151">活跃</span><span class="sxs-lookup"><span data-stu-id="e3034-151">Active</span></span>
- <span data-ttu-id="e3034-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="e3034-152">Report Date</span></span>
- <span data-ttu-id="e3034-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="e3034-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e3034-154">示例</span><span class="sxs-lookup"><span data-stu-id="e3034-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e3034-155">请求</span><span class="sxs-lookup"><span data-stu-id="e3034-155">Request</span></span>

<span data-ttu-id="e3034-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3034-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="e3034-157">响应</span><span class="sxs-lookup"><span data-stu-id="e3034-157">Response</span></span>

<span data-ttu-id="e3034-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3034-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="e3034-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e3034-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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

