---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5a2fa39fd0c6ead0c602d2a171b35842e35c4eed
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571056"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="30aaa-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="30aaa-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="30aaa-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="30aaa-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="30aaa-106">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="30aaa-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="30aaa-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="30aaa-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="30aaa-108">权限</span><span class="sxs-lookup"><span data-stu-id="30aaa-108">Permissions</span></span>

<span data-ttu-id="30aaa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30aaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30aaa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="30aaa-111">Permission type</span></span>                        | <span data-ttu-id="30aaa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30aaa-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="30aaa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30aaa-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="30aaa-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30aaa-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="30aaa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30aaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30aaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="30aaa-116">Not supported.</span></span>                           |
| <span data-ttu-id="30aaa-117">应用</span><span class="sxs-lookup"><span data-stu-id="30aaa-117">Application</span></span>                            | <span data-ttu-id="30aaa-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30aaa-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="30aaa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30aaa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="30aaa-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="30aaa-120">Function parameters</span></span>

<span data-ttu-id="30aaa-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="30aaa-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="30aaa-122">参数</span><span class="sxs-lookup"><span data-stu-id="30aaa-122">Parameter</span></span> | <span data-ttu-id="30aaa-123">类型</span><span class="sxs-lookup"><span data-stu-id="30aaa-123">Type</span></span>   | <span data-ttu-id="30aaa-124">说明</span><span class="sxs-lookup"><span data-stu-id="30aaa-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="30aaa-125">period</span><span class="sxs-lookup"><span data-stu-id="30aaa-125">period</span></span>    | <span data-ttu-id="30aaa-126">string</span><span class="sxs-lookup"><span data-stu-id="30aaa-126">string</span></span> | <span data-ttu-id="30aaa-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="30aaa-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="30aaa-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="30aaa-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="30aaa-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="30aaa-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="30aaa-130">必需。</span><span class="sxs-lookup"><span data-stu-id="30aaa-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="30aaa-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="30aaa-131">Request headers</span></span>

| <span data-ttu-id="30aaa-132">名称</span><span class="sxs-lookup"><span data-stu-id="30aaa-132">Name</span></span>          | <span data-ttu-id="30aaa-133">说明</span><span class="sxs-lookup"><span data-stu-id="30aaa-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="30aaa-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="30aaa-134">Authorization</span></span> | <span data-ttu-id="30aaa-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="30aaa-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="30aaa-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="30aaa-137">If-None-Match</span></span> | <span data-ttu-id="30aaa-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="30aaa-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="30aaa-139">可选。</span><span class="sxs-lookup"><span data-stu-id="30aaa-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="30aaa-140">响应</span><span class="sxs-lookup"><span data-stu-id="30aaa-140">Response</span></span>

<span data-ttu-id="30aaa-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="30aaa-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="30aaa-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="30aaa-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="30aaa-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="30aaa-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="30aaa-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="30aaa-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="30aaa-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="30aaa-145">Report Refresh Date</span></span>
- <span data-ttu-id="30aaa-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="30aaa-146">Report Date</span></span>
- <span data-ttu-id="30aaa-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="30aaa-147">Report Period</span></span>
- <span data-ttu-id="30aaa-148">IM</span><span class="sxs-lookup"><span data-stu-id="30aaa-148">IM</span></span>
- <span data-ttu-id="30aaa-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="30aaa-149">Audio/Video</span></span>
- <span data-ttu-id="30aaa-150">应用共享</span><span class="sxs-lookup"><span data-stu-id="30aaa-150">App Sharing</span></span>
- <span data-ttu-id="30aaa-151">Web</span><span class="sxs-lookup"><span data-stu-id="30aaa-151">Web</span></span>
- <span data-ttu-id="30aaa-152">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="30aaa-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="30aaa-153">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="30aaa-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="30aaa-154">示例</span><span class="sxs-lookup"><span data-stu-id="30aaa-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="30aaa-155">请求</span><span class="sxs-lookup"><span data-stu-id="30aaa-155">Request</span></span>

<span data-ttu-id="30aaa-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="30aaa-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="30aaa-157">响应</span><span class="sxs-lookup"><span data-stu-id="30aaa-157">Response</span></span>

<span data-ttu-id="30aaa-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="30aaa-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="30aaa-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="30aaa-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
