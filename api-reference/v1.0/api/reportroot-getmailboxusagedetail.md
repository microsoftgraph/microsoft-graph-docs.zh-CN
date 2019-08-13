---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a59a75304702b5e8174d051a4f943233043442d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327220"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="67ec7-103">reportRoot：getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="67ec7-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="67ec7-104">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="67ec7-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="67ec7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="67ec7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="67ec7-106">权限</span><span class="sxs-lookup"><span data-stu-id="67ec7-106">Permissions</span></span>

<span data-ttu-id="67ec7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67ec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67ec7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67ec7-109">Permission type</span></span>                        | <span data-ttu-id="67ec7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67ec7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="67ec7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67ec7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="67ec7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67ec7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="67ec7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67ec7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ec7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="67ec7-114">Not supported.</span></span>                           |
| <span data-ttu-id="67ec7-115">应用</span><span class="sxs-lookup"><span data-stu-id="67ec7-115">Application</span></span>                            | <span data-ttu-id="67ec7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67ec7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="67ec7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67ec7-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="67ec7-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="67ec7-118">Function parameters</span></span>

<span data-ttu-id="67ec7-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="67ec7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="67ec7-120">参数</span><span class="sxs-lookup"><span data-stu-id="67ec7-120">Parameter</span></span> | <span data-ttu-id="67ec7-121">类型</span><span class="sxs-lookup"><span data-stu-id="67ec7-121">Type</span></span>   | <span data-ttu-id="67ec7-122">说明</span><span class="sxs-lookup"><span data-stu-id="67ec7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="67ec7-123">period</span><span class="sxs-lookup"><span data-stu-id="67ec7-123">period</span></span>    | <span data-ttu-id="67ec7-124">string</span><span class="sxs-lookup"><span data-stu-id="67ec7-124">string</span></span> | <span data-ttu-id="67ec7-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="67ec7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="67ec7-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="67ec7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="67ec7-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="67ec7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="67ec7-128">必需。</span><span class="sxs-lookup"><span data-stu-id="67ec7-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="67ec7-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="67ec7-129">Request headers</span></span>

| <span data-ttu-id="67ec7-130">名称</span><span class="sxs-lookup"><span data-stu-id="67ec7-130">Name</span></span>          | <span data-ttu-id="67ec7-131">说明</span><span class="sxs-lookup"><span data-stu-id="67ec7-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="67ec7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="67ec7-132">Authorization</span></span> | <span data-ttu-id="67ec7-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="67ec7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="67ec7-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="67ec7-135">If-None-Match</span></span> | <span data-ttu-id="67ec7-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="67ec7-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="67ec7-137">可选。</span><span class="sxs-lookup"><span data-stu-id="67ec7-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="67ec7-138">响应</span><span class="sxs-lookup"><span data-stu-id="67ec7-138">Response</span></span>

<span data-ttu-id="67ec7-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="67ec7-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="67ec7-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="67ec7-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="67ec7-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="67ec7-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="67ec7-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="67ec7-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="67ec7-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="67ec7-143">Report Refresh Date</span></span>
- <span data-ttu-id="67ec7-144">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="67ec7-144">User Principal Name</span></span>
- <span data-ttu-id="67ec7-145">显示名称</span><span class="sxs-lookup"><span data-stu-id="67ec7-145">Display Name</span></span>
- <span data-ttu-id="67ec7-146">已删除</span><span class="sxs-lookup"><span data-stu-id="67ec7-146">Is Deleted</span></span>
- <span data-ttu-id="67ec7-147">删除日期</span><span class="sxs-lookup"><span data-stu-id="67ec7-147">Deleted Date</span></span>
- <span data-ttu-id="67ec7-148">创建日期</span><span class="sxs-lookup"><span data-stu-id="67ec7-148">Created Date</span></span>
- <span data-ttu-id="67ec7-149">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="67ec7-149">Last Activity Date</span></span>
- <span data-ttu-id="67ec7-150">项数</span><span class="sxs-lookup"><span data-stu-id="67ec7-150">Item Count</span></span>
- <span data-ttu-id="67ec7-151">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="67ec7-151">Storage Used (Byte)</span></span>
- <span data-ttu-id="67ec7-152">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="67ec7-152">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="67ec7-153">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="67ec7-153">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="67ec7-154">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="67ec7-154">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="67ec7-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="67ec7-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="67ec7-156">示例</span><span class="sxs-lookup"><span data-stu-id="67ec7-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="67ec7-157">请求</span><span class="sxs-lookup"><span data-stu-id="67ec7-157">Request</span></span>

<span data-ttu-id="67ec7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67ec7-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="67ec7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ec7-159">--Http</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67ec7-160">C#</span><span class="sxs-lookup"><span data-stu-id="67ec7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67ec7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ec7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67ec7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ec7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="67ec7-163">Java</span><span class="sxs-lookup"><span data-stu-id="67ec7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67ec7-164">响应</span><span class="sxs-lookup"><span data-stu-id="67ec7-164">Response</span></span>

<span data-ttu-id="67ec7-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67ec7-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="67ec7-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="67ec7-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
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
