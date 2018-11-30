---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
ms.openlocfilehash: 58d0ddd884fed70e9fc5cbdd1c3d97c8a5463ccc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011229"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="71138-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="71138-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="71138-105">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="71138-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="71138-106">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="71138-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="71138-107">权限</span><span class="sxs-lookup"><span data-stu-id="71138-107">Permissions</span></span>

<span data-ttu-id="71138-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71138-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71138-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71138-110">Permission type</span></span>                        | <span data-ttu-id="71138-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71138-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="71138-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71138-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="71138-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71138-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="71138-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71138-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71138-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71138-115">Not supported.</span></span>                           |
| <span data-ttu-id="71138-116">应用</span><span class="sxs-lookup"><span data-stu-id="71138-116">Application</span></span>                            | <span data-ttu-id="71138-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71138-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="71138-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71138-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="71138-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="71138-119">Function parameters</span></span>

<span data-ttu-id="71138-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="71138-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="71138-121">参数</span><span class="sxs-lookup"><span data-stu-id="71138-121">Parameter</span></span> | <span data-ttu-id="71138-122">类型</span><span class="sxs-lookup"><span data-stu-id="71138-122">Type</span></span>   | <span data-ttu-id="71138-123">说明</span><span class="sxs-lookup"><span data-stu-id="71138-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="71138-124">period</span><span class="sxs-lookup"><span data-stu-id="71138-124">period</span></span>    | <span data-ttu-id="71138-125">string</span><span class="sxs-lookup"><span data-stu-id="71138-125">string</span></span> | <span data-ttu-id="71138-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="71138-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="71138-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="71138-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="71138-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="71138-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="71138-129">必需。</span><span class="sxs-lookup"><span data-stu-id="71138-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="71138-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="71138-130">Request headers</span></span>

| <span data-ttu-id="71138-131">名称</span><span class="sxs-lookup"><span data-stu-id="71138-131">Name</span></span>          | <span data-ttu-id="71138-132">说明</span><span class="sxs-lookup"><span data-stu-id="71138-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="71138-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="71138-133">Authorization</span></span> | <span data-ttu-id="71138-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71138-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="71138-136">响应</span><span class="sxs-lookup"><span data-stu-id="71138-136">Response</span></span>

<span data-ttu-id="71138-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="71138-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="71138-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="71138-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="71138-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="71138-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="71138-140">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="71138-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="71138-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="71138-141">Report Refresh Date</span></span>
- <span data-ttu-id="71138-142">报表日期</span><span class="sxs-lookup"><span data-stu-id="71138-142">Report Date</span></span>
- <span data-ttu-id="71138-143">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="71138-143">Team Chat Messages</span></span>
- <span data-ttu-id="71138-144">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="71138-144">Private Chat Messages</span></span>
- <span data-ttu-id="71138-145">呼叫</span><span class="sxs-lookup"><span data-stu-id="71138-145">Calls</span></span>
- <span data-ttu-id="71138-146">会议</span><span class="sxs-lookup"><span data-stu-id="71138-146">Meetings</span></span>
- <span data-ttu-id="71138-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="71138-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="71138-148">示例</span><span class="sxs-lookup"><span data-stu-id="71138-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="71138-149">请求</span><span class="sxs-lookup"><span data-stu-id="71138-149">Request</span></span>

<span data-ttu-id="71138-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71138-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="71138-151">响应</span><span class="sxs-lookup"><span data-stu-id="71138-151">Response</span></span>

<span data-ttu-id="71138-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71138-152">The following is an example of the response.</span></span>

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
<span data-ttu-id="71138-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="71138-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```
