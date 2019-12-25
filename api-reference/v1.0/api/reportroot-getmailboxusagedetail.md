---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f46c11171e053af741beebb8d999fdbc43aedc4f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864472"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="1999c-103">reportRoot：getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="1999c-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="1999c-104">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1999c-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="1999c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="1999c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="1999c-106">权限</span><span class="sxs-lookup"><span data-stu-id="1999c-106">Permissions</span></span>

<span data-ttu-id="1999c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1999c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1999c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1999c-109">Permission type</span></span>                        | <span data-ttu-id="1999c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1999c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1999c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1999c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1999c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1999c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1999c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1999c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1999c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1999c-114">Not supported.</span></span>                           |
| <span data-ttu-id="1999c-115">应用</span><span class="sxs-lookup"><span data-stu-id="1999c-115">Application</span></span>                            | <span data-ttu-id="1999c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1999c-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="1999c-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="1999c-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1999c-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="1999c-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1999c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1999c-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1999c-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="1999c-120">Function parameters</span></span>

<span data-ttu-id="1999c-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1999c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1999c-122">参数</span><span class="sxs-lookup"><span data-stu-id="1999c-122">Parameter</span></span> | <span data-ttu-id="1999c-123">类型</span><span class="sxs-lookup"><span data-stu-id="1999c-123">Type</span></span>   | <span data-ttu-id="1999c-124">说明</span><span class="sxs-lookup"><span data-stu-id="1999c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1999c-125">period</span><span class="sxs-lookup"><span data-stu-id="1999c-125">period</span></span>    | <span data-ttu-id="1999c-126">string</span><span class="sxs-lookup"><span data-stu-id="1999c-126">string</span></span> | <span data-ttu-id="1999c-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1999c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1999c-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1999c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1999c-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1999c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1999c-130">必需。</span><span class="sxs-lookup"><span data-stu-id="1999c-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1999c-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="1999c-131">Request headers</span></span>

| <span data-ttu-id="1999c-132">名称</span><span class="sxs-lookup"><span data-stu-id="1999c-132">Name</span></span>          | <span data-ttu-id="1999c-133">说明</span><span class="sxs-lookup"><span data-stu-id="1999c-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1999c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1999c-134">Authorization</span></span> | <span data-ttu-id="1999c-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="1999c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1999c-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1999c-137">If-None-Match</span></span> | <span data-ttu-id="1999c-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1999c-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1999c-139">可选。</span><span class="sxs-lookup"><span data-stu-id="1999c-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1999c-140">响应</span><span class="sxs-lookup"><span data-stu-id="1999c-140">Response</span></span>

<span data-ttu-id="1999c-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1999c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1999c-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1999c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1999c-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1999c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1999c-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1999c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1999c-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1999c-145">Report Refresh Date</span></span>
- <span data-ttu-id="1999c-146">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1999c-146">User Principal Name</span></span>
- <span data-ttu-id="1999c-147">显示名称</span><span class="sxs-lookup"><span data-stu-id="1999c-147">Display Name</span></span>
- <span data-ttu-id="1999c-148">已删除</span><span class="sxs-lookup"><span data-stu-id="1999c-148">Is Deleted</span></span>
- <span data-ttu-id="1999c-149">删除日期</span><span class="sxs-lookup"><span data-stu-id="1999c-149">Deleted Date</span></span>
- <span data-ttu-id="1999c-150">创建日期</span><span class="sxs-lookup"><span data-stu-id="1999c-150">Created Date</span></span>
- <span data-ttu-id="1999c-151">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="1999c-151">Last Activity Date</span></span>
- <span data-ttu-id="1999c-152">项数</span><span class="sxs-lookup"><span data-stu-id="1999c-152">Item Count</span></span>
- <span data-ttu-id="1999c-153">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="1999c-153">Storage Used (Byte)</span></span>
- <span data-ttu-id="1999c-154">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="1999c-154">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="1999c-155">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="1999c-155">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="1999c-156">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="1999c-156">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="1999c-157">删除项目计数</span><span class="sxs-lookup"><span data-stu-id="1999c-157">Deleted Item Count</span></span>
- <span data-ttu-id="1999c-158">删除项目大小（字节）</span><span class="sxs-lookup"><span data-stu-id="1999c-158">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="1999c-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="1999c-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1999c-160">示例</span><span class="sxs-lookup"><span data-stu-id="1999c-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1999c-161">请求</span><span class="sxs-lookup"><span data-stu-id="1999c-161">Request</span></span>

<span data-ttu-id="1999c-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1999c-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1999c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="1999c-163">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1999c-164">C#</span><span class="sxs-lookup"><span data-stu-id="1999c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1999c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1999c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1999c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1999c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1999c-167">Java</span><span class="sxs-lookup"><span data-stu-id="1999c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1999c-168">响应</span><span class="sxs-lookup"><span data-stu-id="1999c-168">Response</span></span>

<span data-ttu-id="1999c-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1999c-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="1999c-170">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1999c-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
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
