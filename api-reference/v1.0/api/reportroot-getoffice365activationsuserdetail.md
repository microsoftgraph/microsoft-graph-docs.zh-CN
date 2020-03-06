---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05c8d9385a9b79e38a57dbbb179cfbdb1b95f29d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510359"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="ec708-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="ec708-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="ec708-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec708-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec708-105">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ec708-105">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="ec708-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="ec708-106">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec708-107">权限</span><span class="sxs-lookup"><span data-stu-id="ec708-107">Permissions</span></span>

<span data-ttu-id="ec708-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec708-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec708-110">Permission type</span></span>                        | <span data-ttu-id="ec708-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec708-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ec708-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec708-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec708-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec708-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ec708-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec708-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec708-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec708-115">Not supported.</span></span>                           |
| <span data-ttu-id="ec708-116">应用</span><span class="sxs-lookup"><span data-stu-id="ec708-116">Application</span></span>                            | <span data-ttu-id="ec708-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec708-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ec708-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="ec708-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ec708-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="ec708-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ec708-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec708-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="ec708-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec708-121">Request headers</span></span>

| <span data-ttu-id="ec708-122">名称</span><span class="sxs-lookup"><span data-stu-id="ec708-122">Name</span></span>          | <span data-ttu-id="ec708-123">说明</span><span class="sxs-lookup"><span data-stu-id="ec708-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ec708-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec708-124">Authorization</span></span> | <span data-ttu-id="ec708-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec708-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ec708-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ec708-127">If-None-Match</span></span> | <span data-ttu-id="ec708-128">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ec708-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ec708-129">可选。</span><span class="sxs-lookup"><span data-stu-id="ec708-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ec708-130">响应</span><span class="sxs-lookup"><span data-stu-id="ec708-130">Response</span></span>

<span data-ttu-id="ec708-131">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ec708-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ec708-132">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ec708-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ec708-133">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ec708-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ec708-134">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ec708-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ec708-135">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ec708-135">Report Refresh Date</span></span>
- <span data-ttu-id="ec708-136">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ec708-136">User Principal Name</span></span>
- <span data-ttu-id="ec708-137">显示名称</span><span class="sxs-lookup"><span data-stu-id="ec708-137">Display Name</span></span>
- <span data-ttu-id="ec708-138">产品类型</span><span class="sxs-lookup"><span data-stu-id="ec708-138">Product Type</span></span>
- <span data-ttu-id="ec708-139">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="ec708-139">Last Activated Date</span></span>
- <span data-ttu-id="ec708-140">Windows</span><span class="sxs-lookup"><span data-stu-id="ec708-140">Windows</span></span>
- <span data-ttu-id="ec708-141">Mac</span><span class="sxs-lookup"><span data-stu-id="ec708-141">Mac</span></span>
- <span data-ttu-id="ec708-142">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="ec708-142">Windows 10 Mobile</span></span>
- <span data-ttu-id="ec708-143">iOS</span><span class="sxs-lookup"><span data-stu-id="ec708-143">iOS</span></span>
- <span data-ttu-id="ec708-144">Android</span><span class="sxs-lookup"><span data-stu-id="ec708-144">Android</span></span>
- <span data-ttu-id="ec708-145">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="ec708-145">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="ec708-146">示例</span><span class="sxs-lookup"><span data-stu-id="ec708-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ec708-147">请求</span><span class="sxs-lookup"><span data-stu-id="ec708-147">Request</span></span>

<span data-ttu-id="ec708-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ec708-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec708-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec708-149">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="c"></a>[<span data-ttu-id="ec708-150">C#</span><span class="sxs-lookup"><span data-stu-id="ec708-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec708-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec708-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec708-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec708-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec708-153">Java</span><span class="sxs-lookup"><span data-stu-id="ec708-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ec708-154">响应</span><span class="sxs-lookup"><span data-stu-id="ec708-154">Response</span></span>

<span data-ttu-id="ec708-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ec708-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="ec708-156">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ec708-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
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
