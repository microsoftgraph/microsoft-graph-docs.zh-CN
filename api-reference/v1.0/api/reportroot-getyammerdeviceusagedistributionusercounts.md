---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: 按设备类型获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 89d267e7a17f97256a3ca45e63415d5f8b26f7fb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865205"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="ffaa7-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ffaa7-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="ffaa7-104">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="ffaa7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffaa7-106">权限</span><span class="sxs-lookup"><span data-stu-id="ffaa7-106">Permissions</span></span>

<span data-ttu-id="ffaa7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffaa7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffaa7-109">Permission type</span></span>                        | <span data-ttu-id="ffaa7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffaa7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ffaa7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffaa7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffaa7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffaa7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ffaa7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffaa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffaa7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-114">Not supported.</span></span>                           |
| <span data-ttu-id="ffaa7-115">应用</span><span class="sxs-lookup"><span data-stu-id="ffaa7-115">Application</span></span>                            | <span data-ttu-id="ffaa7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffaa7-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ffaa7-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ffaa7-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ffaa7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffaa7-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ffaa7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="ffaa7-120">Function parameters</span></span>

<span data-ttu-id="ffaa7-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ffaa7-122">参数</span><span class="sxs-lookup"><span data-stu-id="ffaa7-122">Parameter</span></span> | <span data-ttu-id="ffaa7-123">类型</span><span class="sxs-lookup"><span data-stu-id="ffaa7-123">Type</span></span>   | <span data-ttu-id="ffaa7-124">说明</span><span class="sxs-lookup"><span data-stu-id="ffaa7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ffaa7-125">period</span><span class="sxs-lookup"><span data-stu-id="ffaa7-125">period</span></span>    | <span data-ttu-id="ffaa7-126">string</span><span class="sxs-lookup"><span data-stu-id="ffaa7-126">string</span></span> | <span data-ttu-id="ffaa7-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ffaa7-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ffaa7-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ffaa7-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ffaa7-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffaa7-131">Request headers</span></span>

| <span data-ttu-id="ffaa7-132">名称</span><span class="sxs-lookup"><span data-stu-id="ffaa7-132">Name</span></span>          | <span data-ttu-id="ffaa7-133">说明</span><span class="sxs-lookup"><span data-stu-id="ffaa7-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ffaa7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffaa7-134">Authorization</span></span> | <span data-ttu-id="ffaa7-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ffaa7-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ffaa7-137">If-None-Match</span></span> | <span data-ttu-id="ffaa7-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ffaa7-139">可选。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ffaa7-140">响应</span><span class="sxs-lookup"><span data-stu-id="ffaa7-140">Response</span></span>

<span data-ttu-id="ffaa7-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ffaa7-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ffaa7-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ffaa7-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ffaa7-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ffaa7-145">Report Refresh Date</span></span>
- <span data-ttu-id="ffaa7-146">Web</span><span class="sxs-lookup"><span data-stu-id="ffaa7-146">Web</span></span>
- <span data-ttu-id="ffaa7-147">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="ffaa7-147">Windows Phone</span></span>
- <span data-ttu-id="ffaa7-148">Android 手机</span><span class="sxs-lookup"><span data-stu-id="ffaa7-148">Android Phone</span></span>
- <span data-ttu-id="ffaa7-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="ffaa7-149">iPhone</span></span>
- <span data-ttu-id="ffaa7-150">iPad</span><span class="sxs-lookup"><span data-stu-id="ffaa7-150">iPad</span></span>
- <span data-ttu-id="ffaa7-151">其他</span><span class="sxs-lookup"><span data-stu-id="ffaa7-151">Other</span></span>
- <span data-ttu-id="ffaa7-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="ffaa7-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ffaa7-153">示例</span><span class="sxs-lookup"><span data-stu-id="ffaa7-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ffaa7-154">请求</span><span class="sxs-lookup"><span data-stu-id="ffaa7-154">Request</span></span>

<span data-ttu-id="ffaa7-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ffaa7-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffaa7-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ffaa7-157">C#</span><span class="sxs-lookup"><span data-stu-id="ffaa7-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffaa7-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffaa7-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ffaa7-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffaa7-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ffaa7-160">Java</span><span class="sxs-lookup"><span data-stu-id="ffaa7-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ffaa7-161">响应</span><span class="sxs-lookup"><span data-stu-id="ffaa7-161">Response</span></span>

<span data-ttu-id="ffaa7-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="ffaa7-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ffaa7-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
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
