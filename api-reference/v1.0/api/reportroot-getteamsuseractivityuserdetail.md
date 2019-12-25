---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e10862bbefc091f6d8e8bbbaeba502734637965e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865228"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="144bb-103">reportRoot：getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="144bb-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="144bb-104">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="144bb-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="144bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="144bb-105">Permissions</span></span>

<span data-ttu-id="144bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="144bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="144bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="144bb-108">Permission type</span></span>                        | <span data-ttu-id="144bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="144bb-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="144bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="144bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="144bb-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="144bb-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="144bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="144bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144bb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="144bb-113">Not supported.</span></span>                           |
| <span data-ttu-id="144bb-114">应用</span><span class="sxs-lookup"><span data-stu-id="144bb-114">Application</span></span>                            | <span data-ttu-id="144bb-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="144bb-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="144bb-116">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="144bb-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="144bb-117">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="144bb-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="144bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="144bb-118">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="144bb-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="144bb-119">Function parameters</span></span>

<span data-ttu-id="144bb-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="144bb-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="144bb-121">参数</span><span class="sxs-lookup"><span data-stu-id="144bb-121">Parameter</span></span> | <span data-ttu-id="144bb-122">类型</span><span class="sxs-lookup"><span data-stu-id="144bb-122">Type</span></span>   | <span data-ttu-id="144bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="144bb-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="144bb-124">period</span><span class="sxs-lookup"><span data-stu-id="144bb-124">period</span></span>    | <span data-ttu-id="144bb-125">string</span><span class="sxs-lookup"><span data-stu-id="144bb-125">string</span></span> | <span data-ttu-id="144bb-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="144bb-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="144bb-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="144bb-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="144bb-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="144bb-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="144bb-129">date</span><span class="sxs-lookup"><span data-stu-id="144bb-129">date</span></span>      | <span data-ttu-id="144bb-130">Date</span><span class="sxs-lookup"><span data-stu-id="144bb-130">Date</span></span>   | <span data-ttu-id="144bb-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="144bb-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="144bb-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="144bb-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="144bb-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="144bb-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="144bb-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="144bb-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="144bb-135">请求头</span><span class="sxs-lookup"><span data-stu-id="144bb-135">Request headers</span></span>

| <span data-ttu-id="144bb-136">名称</span><span class="sxs-lookup"><span data-stu-id="144bb-136">Name</span></span>          | <span data-ttu-id="144bb-137">说明</span><span class="sxs-lookup"><span data-stu-id="144bb-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="144bb-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="144bb-138">Authorization</span></span> | <span data-ttu-id="144bb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="144bb-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="144bb-141">响应</span><span class="sxs-lookup"><span data-stu-id="144bb-141">Response</span></span>

<span data-ttu-id="144bb-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="144bb-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="144bb-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="144bb-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="144bb-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="144bb-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="144bb-145">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="144bb-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="144bb-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="144bb-146">Report Refresh Date</span></span>
- <span data-ttu-id="144bb-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="144bb-147">User Principal Name</span></span>
- <span data-ttu-id="144bb-148">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="144bb-148">Last Activity Date</span></span>
- <span data-ttu-id="144bb-149">已删除</span><span class="sxs-lookup"><span data-stu-id="144bb-149">Is Deleted</span></span>
- <span data-ttu-id="144bb-150">删除日期</span><span class="sxs-lookup"><span data-stu-id="144bb-150">Deleted Date</span></span>
- <span data-ttu-id="144bb-151">分配的产品</span><span class="sxs-lookup"><span data-stu-id="144bb-151">Assigned Products</span></span>
- <span data-ttu-id="144bb-152">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="144bb-152">Team Chat Message Count</span></span>
- <span data-ttu-id="144bb-153">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="144bb-153">Private Chat Message Count</span></span>
- <span data-ttu-id="144bb-154">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="144bb-154">Call Count</span></span>
- <span data-ttu-id="144bb-155">会议计数</span><span class="sxs-lookup"><span data-stu-id="144bb-155">Meeting Count</span></span>
- <span data-ttu-id="144bb-156">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="144bb-156">Has Other Action</span></span>
- <span data-ttu-id="144bb-157">报表周期</span><span class="sxs-lookup"><span data-stu-id="144bb-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="144bb-158">示例</span><span class="sxs-lookup"><span data-stu-id="144bb-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="144bb-159">请求</span><span class="sxs-lookup"><span data-stu-id="144bb-159">Request</span></span>

<span data-ttu-id="144bb-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="144bb-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="144bb-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="144bb-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="144bb-162">C#</span><span class="sxs-lookup"><span data-stu-id="144bb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="144bb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="144bb-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="144bb-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="144bb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="144bb-165">Java</span><span class="sxs-lookup"><span data-stu-id="144bb-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="144bb-166">响应</span><span class="sxs-lookup"><span data-stu-id="144bb-166">Response</span></span>

<span data-ttu-id="144bb-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="144bb-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="144bb-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="144bb-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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
