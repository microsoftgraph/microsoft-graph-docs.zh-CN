---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 43df5c8bc681fae23493c8a578b95e894fed107d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327190"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="b62fd-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="b62fd-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="b62fd-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="b62fd-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="b62fd-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="b62fd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b62fd-106">权限</span><span class="sxs-lookup"><span data-stu-id="b62fd-106">Permissions</span></span>

<span data-ttu-id="b62fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b62fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b62fd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b62fd-109">Permission type</span></span>                        | <span data-ttu-id="b62fd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b62fd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b62fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b62fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b62fd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b62fd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b62fd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b62fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b62fd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b62fd-114">Not supported.</span></span>                           |
| <span data-ttu-id="b62fd-115">应用</span><span class="sxs-lookup"><span data-stu-id="b62fd-115">Application</span></span>                            | <span data-ttu-id="b62fd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b62fd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b62fd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b62fd-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="b62fd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b62fd-118">Request headers</span></span>

| <span data-ttu-id="b62fd-119">名称</span><span class="sxs-lookup"><span data-stu-id="b62fd-119">Name</span></span>          | <span data-ttu-id="b62fd-120">说明</span><span class="sxs-lookup"><span data-stu-id="b62fd-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b62fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b62fd-121">Authorization</span></span> | <span data-ttu-id="b62fd-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b62fd-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b62fd-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b62fd-124">If-None-Match</span></span> | <span data-ttu-id="b62fd-125">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b62fd-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b62fd-126">可选。</span><span class="sxs-lookup"><span data-stu-id="b62fd-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b62fd-127">响应</span><span class="sxs-lookup"><span data-stu-id="b62fd-127">Response</span></span>

<span data-ttu-id="b62fd-128">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b62fd-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b62fd-129">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b62fd-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b62fd-130">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b62fd-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b62fd-131">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b62fd-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b62fd-132">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b62fd-132">Report Refresh Date</span></span>
- <span data-ttu-id="b62fd-133">产品类型</span><span class="sxs-lookup"><span data-stu-id="b62fd-133">Product Type</span></span>
- <span data-ttu-id="b62fd-134">Windows</span><span class="sxs-lookup"><span data-stu-id="b62fd-134">Windows</span></span>
- <span data-ttu-id="b62fd-135">Mac</span><span class="sxs-lookup"><span data-stu-id="b62fd-135">Mac</span></span>
- <span data-ttu-id="b62fd-136">Android</span><span class="sxs-lookup"><span data-stu-id="b62fd-136">Android</span></span>
- <span data-ttu-id="b62fd-137">iOS</span><span class="sxs-lookup"><span data-stu-id="b62fd-137">iOS</span></span>
- <span data-ttu-id="b62fd-138">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="b62fd-138">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="b62fd-139">示例</span><span class="sxs-lookup"><span data-stu-id="b62fd-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b62fd-140">请求</span><span class="sxs-lookup"><span data-stu-id="b62fd-140">Request</span></span>

<span data-ttu-id="b62fd-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b62fd-141">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b62fd-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b62fd-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b62fd-143">C#</span><span class="sxs-lookup"><span data-stu-id="b62fd-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b62fd-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b62fd-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b62fd-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="b62fd-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b62fd-146">Java</span><span class="sxs-lookup"><span data-stu-id="b62fd-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b62fd-147">响应</span><span class="sxs-lookup"><span data-stu-id="b62fd-147">Response</span></span>

<span data-ttu-id="b62fd-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b62fd-148">The following is an example of the response.</span></span>

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

<span data-ttu-id="b62fd-149">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b62fd-149">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
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
