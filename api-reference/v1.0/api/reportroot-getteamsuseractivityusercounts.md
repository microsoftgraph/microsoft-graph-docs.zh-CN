---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f1f86f4ca0953b0b4b4ef2652c2ff74227ea7878
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458920"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="7c2ed-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7c2ed-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="7c2ed-105">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="7c2ed-106">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c2ed-107">权限</span><span class="sxs-lookup"><span data-stu-id="7c2ed-107">Permissions</span></span>

<span data-ttu-id="7c2ed-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c2ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c2ed-110">Permission type</span></span>                        | <span data-ttu-id="7c2ed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c2ed-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c2ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c2ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c2ed-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c2ed-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c2ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c2ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c2ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-115">Not supported.</span></span>                           |
| <span data-ttu-id="7c2ed-116">应用</span><span class="sxs-lookup"><span data-stu-id="7c2ed-116">Application</span></span>                            | <span data-ttu-id="7c2ed-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c2ed-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c2ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c2ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7c2ed-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="7c2ed-119">Function parameters</span></span>

<span data-ttu-id="7c2ed-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7c2ed-121">参数</span><span class="sxs-lookup"><span data-stu-id="7c2ed-121">Parameter</span></span> | <span data-ttu-id="7c2ed-122">类型</span><span class="sxs-lookup"><span data-stu-id="7c2ed-122">Type</span></span>   | <span data-ttu-id="7c2ed-123">说明</span><span class="sxs-lookup"><span data-stu-id="7c2ed-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c2ed-124">period</span><span class="sxs-lookup"><span data-stu-id="7c2ed-124">period</span></span>    | <span data-ttu-id="7c2ed-125">string</span><span class="sxs-lookup"><span data-stu-id="7c2ed-125">string</span></span> | <span data-ttu-id="7c2ed-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c2ed-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c2ed-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7c2ed-129">必需。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7c2ed-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c2ed-130">Request headers</span></span>

| <span data-ttu-id="7c2ed-131">名称</span><span class="sxs-lookup"><span data-stu-id="7c2ed-131">Name</span></span>          | <span data-ttu-id="7c2ed-132">说明</span><span class="sxs-lookup"><span data-stu-id="7c2ed-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7c2ed-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c2ed-133">Authorization</span></span> | <span data-ttu-id="7c2ed-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c2ed-136">响应</span><span class="sxs-lookup"><span data-stu-id="7c2ed-136">Response</span></span>

<span data-ttu-id="7c2ed-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c2ed-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c2ed-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c2ed-140">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="7c2ed-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="7c2ed-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7c2ed-141">Report Refresh Date</span></span>
- <span data-ttu-id="7c2ed-142">报表日期</span><span class="sxs-lookup"><span data-stu-id="7c2ed-142">Report Date</span></span>
- <span data-ttu-id="7c2ed-143">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="7c2ed-143">Team Chat Messages</span></span>
- <span data-ttu-id="7c2ed-144">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="7c2ed-144">Private Chat Messages</span></span>
- <span data-ttu-id="7c2ed-145">呼叫</span><span class="sxs-lookup"><span data-stu-id="7c2ed-145">Calls</span></span>
- <span data-ttu-id="7c2ed-146">会议</span><span class="sxs-lookup"><span data-stu-id="7c2ed-146">Meetings</span></span>
- <span data-ttu-id="7c2ed-147">其他操作</span><span class="sxs-lookup"><span data-stu-id="7c2ed-147">Other Actions</span></span>
- <span data-ttu-id="7c2ed-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="7c2ed-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7c2ed-149">示例</span><span class="sxs-lookup"><span data-stu-id="7c2ed-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c2ed-150">请求</span><span class="sxs-lookup"><span data-stu-id="7c2ed-150">Request</span></span>

<span data-ttu-id="7c2ed-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7c2ed-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7c2ed-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c2ed-153">C#</span><span class="sxs-lookup"><span data-stu-id="7c2ed-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c2ed-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c2ed-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c2ed-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="7c2ed-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c2ed-156">响应</span><span class="sxs-lookup"><span data-stu-id="7c2ed-156">Response</span></span>

<span data-ttu-id="7c2ed-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="7c2ed-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7c2ed-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
