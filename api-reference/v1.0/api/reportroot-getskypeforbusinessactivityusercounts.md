---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d39f96a27bdbf8a81c660621728b4ff6e821a98
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573324"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="608e0-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="608e0-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="608e0-105">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="608e0-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="608e0-106">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="608e0-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="608e0-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="608e0-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="608e0-108">权限</span><span class="sxs-lookup"><span data-stu-id="608e0-108">Permissions</span></span>

<span data-ttu-id="608e0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="608e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="608e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="608e0-111">Permission type</span></span>                        | <span data-ttu-id="608e0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="608e0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="608e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="608e0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="608e0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="608e0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="608e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="608e0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="608e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="608e0-116">Not supported.</span></span>                           |
| <span data-ttu-id="608e0-117">应用</span><span class="sxs-lookup"><span data-stu-id="608e0-117">Application</span></span>                            | <span data-ttu-id="608e0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="608e0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="608e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="608e0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="608e0-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="608e0-120">Function parameters</span></span>

<span data-ttu-id="608e0-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="608e0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="608e0-122">参数</span><span class="sxs-lookup"><span data-stu-id="608e0-122">Parameter</span></span> | <span data-ttu-id="608e0-123">类型</span><span class="sxs-lookup"><span data-stu-id="608e0-123">Type</span></span>   | <span data-ttu-id="608e0-124">说明</span><span class="sxs-lookup"><span data-stu-id="608e0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="608e0-125">period</span><span class="sxs-lookup"><span data-stu-id="608e0-125">period</span></span>    | <span data-ttu-id="608e0-126">string</span><span class="sxs-lookup"><span data-stu-id="608e0-126">string</span></span> | <span data-ttu-id="608e0-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="608e0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="608e0-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="608e0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="608e0-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="608e0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="608e0-130">必需。</span><span class="sxs-lookup"><span data-stu-id="608e0-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="608e0-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="608e0-131">Request headers</span></span>

| <span data-ttu-id="608e0-132">名称</span><span class="sxs-lookup"><span data-stu-id="608e0-132">Name</span></span>          | <span data-ttu-id="608e0-133">说明</span><span class="sxs-lookup"><span data-stu-id="608e0-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="608e0-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="608e0-134">Authorization</span></span> | <span data-ttu-id="608e0-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="608e0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="608e0-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="608e0-137">If-None-Match</span></span> | <span data-ttu-id="608e0-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="608e0-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="608e0-139">可选。</span><span class="sxs-lookup"><span data-stu-id="608e0-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="608e0-140">响应</span><span class="sxs-lookup"><span data-stu-id="608e0-140">Response</span></span>

<span data-ttu-id="608e0-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="608e0-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="608e0-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="608e0-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="608e0-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="608e0-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="608e0-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="608e0-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="608e0-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="608e0-145">Report Refresh Date</span></span>
- <span data-ttu-id="608e0-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="608e0-146">Report Date</span></span>
- <span data-ttu-id="608e0-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="608e0-147">Report Period</span></span>
- <span data-ttu-id="608e0-148">对等</span><span class="sxs-lookup"><span data-stu-id="608e0-148">Peer-to-peer</span></span>
- <span data-ttu-id="608e0-149">组织</span><span class="sxs-lookup"><span data-stu-id="608e0-149">Organized</span></span>
- <span data-ttu-id="608e0-150">参与</span><span class="sxs-lookup"><span data-stu-id="608e0-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="608e0-151">示例</span><span class="sxs-lookup"><span data-stu-id="608e0-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="608e0-152">请求</span><span class="sxs-lookup"><span data-stu-id="608e0-152">Request</span></span>

<span data-ttu-id="608e0-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="608e0-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="608e0-154">响应</span><span class="sxs-lookup"><span data-stu-id="608e0-154">Response</span></span>

<span data-ttu-id="608e0-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="608e0-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="608e0-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="608e0-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```
