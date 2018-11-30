---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
ms.openlocfilehash: 3c2b0d927fcf98f5191c3e4ec60980af10af9405
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011716"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="ee87a-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ee87a-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="ee87a-105">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="ee87a-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="ee87a-106">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="ee87a-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee87a-107">权限</span><span class="sxs-lookup"><span data-stu-id="ee87a-107">Permissions</span></span>

<span data-ttu-id="ee87a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee87a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee87a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee87a-110">Permission type</span></span>                        | <span data-ttu-id="ee87a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee87a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee87a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee87a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee87a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee87a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee87a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee87a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee87a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee87a-115">Not supported.</span></span>                           |
| <span data-ttu-id="ee87a-116">应用</span><span class="sxs-lookup"><span data-stu-id="ee87a-116">Application</span></span>                            | <span data-ttu-id="ee87a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee87a-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee87a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee87a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ee87a-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="ee87a-119">Function parameters</span></span>

<span data-ttu-id="ee87a-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ee87a-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ee87a-121">参数</span><span class="sxs-lookup"><span data-stu-id="ee87a-121">Parameter</span></span> | <span data-ttu-id="ee87a-122">类型</span><span class="sxs-lookup"><span data-stu-id="ee87a-122">Type</span></span>   | <span data-ttu-id="ee87a-123">说明</span><span class="sxs-lookup"><span data-stu-id="ee87a-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee87a-124">period</span><span class="sxs-lookup"><span data-stu-id="ee87a-124">period</span></span>    | <span data-ttu-id="ee87a-125">string</span><span class="sxs-lookup"><span data-stu-id="ee87a-125">string</span></span> | <span data-ttu-id="ee87a-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ee87a-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee87a-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ee87a-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee87a-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ee87a-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ee87a-129">必需。</span><span class="sxs-lookup"><span data-stu-id="ee87a-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ee87a-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee87a-130">Request headers</span></span>

| <span data-ttu-id="ee87a-131">名称</span><span class="sxs-lookup"><span data-stu-id="ee87a-131">Name</span></span>          | <span data-ttu-id="ee87a-132">说明</span><span class="sxs-lookup"><span data-stu-id="ee87a-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ee87a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee87a-133">Authorization</span></span> | <span data-ttu-id="ee87a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee87a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee87a-136">响应</span><span class="sxs-lookup"><span data-stu-id="ee87a-136">Response</span></span>

<span data-ttu-id="ee87a-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ee87a-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee87a-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ee87a-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee87a-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ee87a-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee87a-140">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="ee87a-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ee87a-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ee87a-141">Report Refresh Date</span></span>
- <span data-ttu-id="ee87a-142">报表日期</span><span class="sxs-lookup"><span data-stu-id="ee87a-142">Report Date</span></span>
- <span data-ttu-id="ee87a-143">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="ee87a-143">Team Chat Messages</span></span>
- <span data-ttu-id="ee87a-144">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="ee87a-144">Private Chat Messages</span></span>
- <span data-ttu-id="ee87a-145">呼叫</span><span class="sxs-lookup"><span data-stu-id="ee87a-145">Calls</span></span>
- <span data-ttu-id="ee87a-146">会议</span><span class="sxs-lookup"><span data-stu-id="ee87a-146">Meetings</span></span>
- <span data-ttu-id="ee87a-147">其他操作</span><span class="sxs-lookup"><span data-stu-id="ee87a-147">Other Actions</span></span>
- <span data-ttu-id="ee87a-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="ee87a-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ee87a-149">示例</span><span class="sxs-lookup"><span data-stu-id="ee87a-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee87a-150">请求</span><span class="sxs-lookup"><span data-stu-id="ee87a-150">Request</span></span>

<span data-ttu-id="ee87a-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee87a-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ee87a-152">响应</span><span class="sxs-lookup"><span data-stu-id="ee87a-152">Response</span></span>

<span data-ttu-id="ee87a-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee87a-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="ee87a-154">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ee87a-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
