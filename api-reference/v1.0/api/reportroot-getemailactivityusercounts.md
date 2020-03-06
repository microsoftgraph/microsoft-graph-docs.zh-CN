---
title: 'reportRoot: getEmailActivityUserCounts'
description: 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a34a840955372f3f1a467d6dd15a29de135c8be6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510443"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="bbf56-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="bbf56-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="bbf56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbf56-105">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="bbf56-105">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="bbf56-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="bbf56-106">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf56-107">权限</span><span class="sxs-lookup"><span data-stu-id="bbf56-107">Permissions</span></span>

<span data-ttu-id="bbf56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbf56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbf56-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbf56-110">Permission type</span></span>                        | <span data-ttu-id="bbf56-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbf56-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bbf56-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf56-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbf56-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf56-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bbf56-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf56-115">Not supported.</span></span>                           |
| <span data-ttu-id="bbf56-116">应用</span><span class="sxs-lookup"><span data-stu-id="bbf56-116">Application</span></span>                            | <span data-ttu-id="bbf56-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf56-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="bbf56-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="bbf56-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bbf56-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="bbf56-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bbf56-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbf56-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bbf56-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="bbf56-121">Function parameters</span></span>

<span data-ttu-id="bbf56-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bbf56-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bbf56-123">参数</span><span class="sxs-lookup"><span data-stu-id="bbf56-123">Parameter</span></span> | <span data-ttu-id="bbf56-124">类型</span><span class="sxs-lookup"><span data-stu-id="bbf56-124">Type</span></span>   | <span data-ttu-id="bbf56-125">说明</span><span class="sxs-lookup"><span data-stu-id="bbf56-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bbf56-126">period</span><span class="sxs-lookup"><span data-stu-id="bbf56-126">period</span></span>    | <span data-ttu-id="bbf56-127">string</span><span class="sxs-lookup"><span data-stu-id="bbf56-127">string</span></span> | <span data-ttu-id="bbf56-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bbf56-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bbf56-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bbf56-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bbf56-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bbf56-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bbf56-131">必需。</span><span class="sxs-lookup"><span data-stu-id="bbf56-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bbf56-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbf56-132">Request headers</span></span>

| <span data-ttu-id="bbf56-133">名称</span><span class="sxs-lookup"><span data-stu-id="bbf56-133">Name</span></span>          | <span data-ttu-id="bbf56-134">说明</span><span class="sxs-lookup"><span data-stu-id="bbf56-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bbf56-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf56-135">Authorization</span></span> | <span data-ttu-id="bbf56-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbf56-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bbf56-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bbf56-138">If-None-Match</span></span> | <span data-ttu-id="bbf56-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bbf56-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bbf56-140">可选。</span><span class="sxs-lookup"><span data-stu-id="bbf56-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bbf56-141">响应</span><span class="sxs-lookup"><span data-stu-id="bbf56-141">Response</span></span>

<span data-ttu-id="bbf56-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bbf56-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bbf56-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bbf56-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bbf56-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bbf56-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bbf56-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bbf56-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bbf56-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bbf56-146">Report Refresh Date</span></span>
- <span data-ttu-id="bbf56-147">已发送</span><span class="sxs-lookup"><span data-stu-id="bbf56-147">Send</span></span>
- <span data-ttu-id="bbf56-148">已接收</span><span class="sxs-lookup"><span data-stu-id="bbf56-148">Receive</span></span>
- <span data-ttu-id="bbf56-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="bbf56-149">Read</span></span>
- <span data-ttu-id="bbf56-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="bbf56-150">Report Date</span></span>
- <span data-ttu-id="bbf56-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="bbf56-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bbf56-152">示例</span><span class="sxs-lookup"><span data-stu-id="bbf56-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bbf56-153">请求</span><span class="sxs-lookup"><span data-stu-id="bbf56-153">Request</span></span>

<span data-ttu-id="bbf56-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bbf56-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbf56-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf56-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="bbf56-156">C#</span><span class="sxs-lookup"><span data-stu-id="bbf56-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbf56-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbf56-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbf56-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbf56-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbf56-159">Java</span><span class="sxs-lookup"><span data-stu-id="bbf56-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bbf56-160">响应</span><span class="sxs-lookup"><span data-stu-id="bbf56-160">Response</span></span>

<span data-ttu-id="bbf56-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bbf56-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="bbf56-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bbf56-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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
