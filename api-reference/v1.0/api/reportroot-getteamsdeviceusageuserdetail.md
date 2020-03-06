---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9007db3b297683f2af98716ffd9c9145ce84b1af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510065"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="f4200-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f4200-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="f4200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4200-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4200-105">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4200-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4200-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4200-106">Permissions</span></span>

<span data-ttu-id="f4200-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4200-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4200-109">Permission type</span></span>                        | <span data-ttu-id="f4200-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4200-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f4200-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4200-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4200-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4200-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f4200-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4200-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4200-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4200-114">Not supported.</span></span>                           |
| <span data-ttu-id="f4200-115">应用</span><span class="sxs-lookup"><span data-stu-id="f4200-115">Application</span></span>                            | <span data-ttu-id="f4200-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4200-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="f4200-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f4200-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f4200-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="f4200-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f4200-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4200-119">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f4200-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="f4200-120">Function parameters</span></span>

<span data-ttu-id="f4200-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f4200-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f4200-122">参数</span><span class="sxs-lookup"><span data-stu-id="f4200-122">Parameter</span></span> | <span data-ttu-id="f4200-123">类型</span><span class="sxs-lookup"><span data-stu-id="f4200-123">Type</span></span>   | <span data-ttu-id="f4200-124">说明</span><span class="sxs-lookup"><span data-stu-id="f4200-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f4200-125">period</span><span class="sxs-lookup"><span data-stu-id="f4200-125">period</span></span>    | <span data-ttu-id="f4200-126">string</span><span class="sxs-lookup"><span data-stu-id="f4200-126">string</span></span> | <span data-ttu-id="f4200-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f4200-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f4200-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f4200-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f4200-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f4200-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f4200-130">date</span><span class="sxs-lookup"><span data-stu-id="f4200-130">date</span></span>      | <span data-ttu-id="f4200-131">Date</span><span class="sxs-lookup"><span data-stu-id="f4200-131">Date</span></span>   | <span data-ttu-id="f4200-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="f4200-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f4200-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="f4200-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f4200-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="f4200-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f4200-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="f4200-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4200-136">请求头</span><span class="sxs-lookup"><span data-stu-id="f4200-136">Request headers</span></span>

| <span data-ttu-id="f4200-137">名称</span><span class="sxs-lookup"><span data-stu-id="f4200-137">Name</span></span>          | <span data-ttu-id="f4200-138">说明</span><span class="sxs-lookup"><span data-stu-id="f4200-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f4200-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4200-139">Authorization</span></span> | <span data-ttu-id="f4200-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4200-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f4200-142">响应</span><span class="sxs-lookup"><span data-stu-id="f4200-142">Response</span></span>

<span data-ttu-id="f4200-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f4200-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f4200-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f4200-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f4200-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="f4200-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f4200-146">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="f4200-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="f4200-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f4200-147">Report Refresh Date</span></span>
- <span data-ttu-id="f4200-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f4200-148">User Principal Name</span></span>
- <span data-ttu-id="f4200-149">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="f4200-149">Last Activity Date</span></span>
- <span data-ttu-id="f4200-150">已删除</span><span class="sxs-lookup"><span data-stu-id="f4200-150">Is Deleted</span></span>
- <span data-ttu-id="f4200-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="f4200-151">Deleted Date</span></span>
- <span data-ttu-id="f4200-152">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="f4200-152">Used Web</span></span>
- <span data-ttu-id="f4200-153">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="f4200-153">Used Windows Phone</span></span>
- <span data-ttu-id="f4200-154">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="f4200-154">Used iOS</span></span>
- <span data-ttu-id="f4200-155">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="f4200-155">Used Mac</span></span>
- <span data-ttu-id="f4200-156">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="f4200-156">Used Android Phone</span></span>
- <span data-ttu-id="f4200-157">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="f4200-157">Used Windows</span></span>
- <span data-ttu-id="f4200-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="f4200-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f4200-159">示例</span><span class="sxs-lookup"><span data-stu-id="f4200-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f4200-160">请求</span><span class="sxs-lookup"><span data-stu-id="f4200-160">Request</span></span>

<span data-ttu-id="f4200-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4200-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4200-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4200-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="f4200-163">C#</span><span class="sxs-lookup"><span data-stu-id="f4200-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4200-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4200-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4200-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4200-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4200-166">Java</span><span class="sxs-lookup"><span data-stu-id="f4200-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4200-167">响应</span><span class="sxs-lookup"><span data-stu-id="f4200-167">Response</span></span>

<span data-ttu-id="f4200-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4200-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="f4200-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f4200-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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
