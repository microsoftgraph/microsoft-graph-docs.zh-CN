---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e3171ed3e6e62758828cc37a1e2f2e494a22b8a9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729712"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="d2d5e-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="d2d5e-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="d2d5e-104">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="d2d5e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2d5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2d5e-106">Permissions</span></span>

<span data-ttu-id="d2d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2d5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2d5e-109">Permission type</span></span>                        | <span data-ttu-id="d2d5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2d5e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d2d5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2d5e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2d5e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d2d5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-114">Not supported.</span></span>                           |
| <span data-ttu-id="d2d5e-115">应用</span><span class="sxs-lookup"><span data-stu-id="d2d5e-115">Application</span></span>                            | <span data-ttu-id="d2d5e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2d5e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d2d5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2d5e-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="d2d5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2d5e-118">Request headers</span></span>

| <span data-ttu-id="d2d5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="d2d5e-119">Name</span></span>          | <span data-ttu-id="d2d5e-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2d5e-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d2d5e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d5e-121">Authorization</span></span> | <span data-ttu-id="d2d5e-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d2d5e-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d2d5e-124">If-None-Match</span></span> | <span data-ttu-id="d2d5e-125">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d2d5e-126">可选。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d2d5e-127">响应</span><span class="sxs-lookup"><span data-stu-id="d2d5e-127">Response</span></span>

<span data-ttu-id="d2d5e-128">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d2d5e-129">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d2d5e-130">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d2d5e-131">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d2d5e-132">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d2d5e-132">Report Refresh Date</span></span>
- <span data-ttu-id="d2d5e-133">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d2d5e-133">User Principal Name</span></span>
- <span data-ttu-id="d2d5e-134">显示名称</span><span class="sxs-lookup"><span data-stu-id="d2d5e-134">Display Name</span></span>
- <span data-ttu-id="d2d5e-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="d2d5e-135">Product Type</span></span>
- <span data-ttu-id="d2d5e-136">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="d2d5e-136">Last Activated Date</span></span>
- <span data-ttu-id="d2d5e-137">Windows</span><span class="sxs-lookup"><span data-stu-id="d2d5e-137">Windows</span></span>
- <span data-ttu-id="d2d5e-138">Mac</span><span class="sxs-lookup"><span data-stu-id="d2d5e-138">Mac</span></span>
- <span data-ttu-id="d2d5e-139">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="d2d5e-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="d2d5e-140">iOS</span><span class="sxs-lookup"><span data-stu-id="d2d5e-140">iOS</span></span>
- <span data-ttu-id="d2d5e-141">Android</span><span class="sxs-lookup"><span data-stu-id="d2d5e-141">Android</span></span>
- <span data-ttu-id="d2d5e-142">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="d2d5e-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="d2d5e-143">示例</span><span class="sxs-lookup"><span data-stu-id="d2d5e-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d2d5e-144">请求</span><span class="sxs-lookup"><span data-stu-id="d2d5e-144">Request</span></span>

<span data-ttu-id="d2d5e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-145">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d2d5e-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d2d5e-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2d5e-147">C#</span><span class="sxs-lookup"><span data-stu-id="d2d5e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2d5e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2d5e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2d5e-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="d2d5e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2d5e-150">Java</span><span class="sxs-lookup"><span data-stu-id="d2d5e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2d5e-151">响应</span><span class="sxs-lookup"><span data-stu-id="d2d5e-151">Response</span></span>

<span data-ttu-id="d2d5e-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="d2d5e-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d2d5e-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
