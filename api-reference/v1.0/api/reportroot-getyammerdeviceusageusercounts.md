---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: 按设备类型获取每日用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a88b7cae9c11ef814871b39f131d8944f6047de1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864186"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="29d99-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="29d99-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="29d99-104">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="29d99-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="29d99-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="29d99-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="29d99-106">权限</span><span class="sxs-lookup"><span data-stu-id="29d99-106">Permissions</span></span>

<span data-ttu-id="29d99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29d99-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29d99-109">Permission type</span></span>                        | <span data-ttu-id="29d99-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29d99-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="29d99-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29d99-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29d99-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29d99-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="29d99-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29d99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d99-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29d99-114">Not supported.</span></span>                           |
| <span data-ttu-id="29d99-115">应用</span><span class="sxs-lookup"><span data-stu-id="29d99-115">Application</span></span>                            | <span data-ttu-id="29d99-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29d99-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="29d99-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="29d99-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="29d99-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="29d99-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="29d99-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29d99-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="29d99-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="29d99-120">Function parameters</span></span>

<span data-ttu-id="29d99-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="29d99-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="29d99-122">参数</span><span class="sxs-lookup"><span data-stu-id="29d99-122">Parameter</span></span> | <span data-ttu-id="29d99-123">类型</span><span class="sxs-lookup"><span data-stu-id="29d99-123">Type</span></span>   | <span data-ttu-id="29d99-124">说明</span><span class="sxs-lookup"><span data-stu-id="29d99-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="29d99-125">period</span><span class="sxs-lookup"><span data-stu-id="29d99-125">period</span></span>    | <span data-ttu-id="29d99-126">string</span><span class="sxs-lookup"><span data-stu-id="29d99-126">string</span></span> | <span data-ttu-id="29d99-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="29d99-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="29d99-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="29d99-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="29d99-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="29d99-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="29d99-130">必需。</span><span class="sxs-lookup"><span data-stu-id="29d99-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="29d99-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="29d99-131">Request headers</span></span>

| <span data-ttu-id="29d99-132">名称</span><span class="sxs-lookup"><span data-stu-id="29d99-132">Name</span></span>          | <span data-ttu-id="29d99-133">说明</span><span class="sxs-lookup"><span data-stu-id="29d99-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="29d99-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d99-134">Authorization</span></span> | <span data-ttu-id="29d99-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="29d99-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="29d99-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="29d99-137">If-None-Match</span></span> | <span data-ttu-id="29d99-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="29d99-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="29d99-139">可选。</span><span class="sxs-lookup"><span data-stu-id="29d99-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="29d99-140">响应</span><span class="sxs-lookup"><span data-stu-id="29d99-140">Response</span></span>

<span data-ttu-id="29d99-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="29d99-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="29d99-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="29d99-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="29d99-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="29d99-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="29d99-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="29d99-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="29d99-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="29d99-145">Report Refresh Date</span></span>
- <span data-ttu-id="29d99-146">Web</span><span class="sxs-lookup"><span data-stu-id="29d99-146">Web</span></span>
- <span data-ttu-id="29d99-147">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="29d99-147">Windows Phone</span></span>
- <span data-ttu-id="29d99-148">Android 手机</span><span class="sxs-lookup"><span data-stu-id="29d99-148">Android Phone</span></span>
- <span data-ttu-id="29d99-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="29d99-149">iPhone</span></span>
- <span data-ttu-id="29d99-150">iPad</span><span class="sxs-lookup"><span data-stu-id="29d99-150">iPad</span></span>
- <span data-ttu-id="29d99-151">其他</span><span class="sxs-lookup"><span data-stu-id="29d99-151">Other</span></span>
- <span data-ttu-id="29d99-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="29d99-152">Report Date</span></span>
- <span data-ttu-id="29d99-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="29d99-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="29d99-154">示例</span><span class="sxs-lookup"><span data-stu-id="29d99-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="29d99-155">请求</span><span class="sxs-lookup"><span data-stu-id="29d99-155">Request</span></span>

<span data-ttu-id="29d99-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="29d99-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="29d99-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="29d99-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29d99-158">C#</span><span class="sxs-lookup"><span data-stu-id="29d99-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29d99-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29d99-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29d99-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29d99-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29d99-161">Java</span><span class="sxs-lookup"><span data-stu-id="29d99-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29d99-162">响应</span><span class="sxs-lookup"><span data-stu-id="29d99-162">Response</span></span>

<span data-ttu-id="29d99-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="29d99-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="29d99-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="29d99-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
