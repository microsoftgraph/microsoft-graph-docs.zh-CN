---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 6106acc1c7f2cf8366d9fe366831465df43e3d4c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865236"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="0de44-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0de44-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="0de44-105">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="0de44-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="0de44-106">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="0de44-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="0de44-107">权限</span><span class="sxs-lookup"><span data-stu-id="0de44-107">Permissions</span></span>

<span data-ttu-id="0de44-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0de44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0de44-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0de44-110">Permission type</span></span>                        | <span data-ttu-id="0de44-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0de44-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0de44-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0de44-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0de44-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0de44-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0de44-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0de44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0de44-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0de44-115">Not supported.</span></span>                           |
| <span data-ttu-id="0de44-116">应用</span><span class="sxs-lookup"><span data-stu-id="0de44-116">Application</span></span>                            | <span data-ttu-id="0de44-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0de44-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0de44-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="0de44-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0de44-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="0de44-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0de44-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0de44-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0de44-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="0de44-121">Function parameters</span></span>

<span data-ttu-id="0de44-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0de44-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0de44-123">参数</span><span class="sxs-lookup"><span data-stu-id="0de44-123">Parameter</span></span> | <span data-ttu-id="0de44-124">类型</span><span class="sxs-lookup"><span data-stu-id="0de44-124">Type</span></span>   | <span data-ttu-id="0de44-125">说明</span><span class="sxs-lookup"><span data-stu-id="0de44-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0de44-126">period</span><span class="sxs-lookup"><span data-stu-id="0de44-126">period</span></span>    | <span data-ttu-id="0de44-127">string</span><span class="sxs-lookup"><span data-stu-id="0de44-127">string</span></span> | <span data-ttu-id="0de44-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0de44-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0de44-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0de44-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0de44-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0de44-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0de44-131">必需。</span><span class="sxs-lookup"><span data-stu-id="0de44-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0de44-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="0de44-132">Request headers</span></span>

| <span data-ttu-id="0de44-133">名称</span><span class="sxs-lookup"><span data-stu-id="0de44-133">Name</span></span>          | <span data-ttu-id="0de44-134">说明</span><span class="sxs-lookup"><span data-stu-id="0de44-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0de44-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="0de44-135">Authorization</span></span> | <span data-ttu-id="0de44-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0de44-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0de44-138">响应</span><span class="sxs-lookup"><span data-stu-id="0de44-138">Response</span></span>

<span data-ttu-id="0de44-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0de44-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0de44-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0de44-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0de44-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="0de44-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0de44-142">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="0de44-142">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="0de44-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0de44-143">Report Refresh Date</span></span>
- <span data-ttu-id="0de44-144">报表日期</span><span class="sxs-lookup"><span data-stu-id="0de44-144">Report Date</span></span>
- <span data-ttu-id="0de44-145">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="0de44-145">Team Chat Messages</span></span>
- <span data-ttu-id="0de44-146">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="0de44-146">Private Chat Messages</span></span>
- <span data-ttu-id="0de44-147">呼叫</span><span class="sxs-lookup"><span data-stu-id="0de44-147">Calls</span></span>
- <span data-ttu-id="0de44-148">会议</span><span class="sxs-lookup"><span data-stu-id="0de44-148">Meetings</span></span>
- <span data-ttu-id="0de44-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="0de44-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0de44-150">示例</span><span class="sxs-lookup"><span data-stu-id="0de44-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0de44-151">请求</span><span class="sxs-lookup"><span data-stu-id="0de44-151">Request</span></span>

<span data-ttu-id="0de44-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0de44-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0de44-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de44-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0de44-154">C#</span><span class="sxs-lookup"><span data-stu-id="0de44-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0de44-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de44-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0de44-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de44-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0de44-157">Java</span><span class="sxs-lookup"><span data-stu-id="0de44-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de44-158">响应</span><span class="sxs-lookup"><span data-stu-id="0de44-158">Response</span></span>

<span data-ttu-id="0de44-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0de44-159">The following is an example of the response.</span></span>

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
<span data-ttu-id="0de44-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0de44-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
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
