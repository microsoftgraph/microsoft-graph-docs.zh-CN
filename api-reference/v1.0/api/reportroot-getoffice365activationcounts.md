---
title: 'reportRoot: getOffice365ActivationCounts'
description: 获取桌面和设备上激活的 Office 365 订阅数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a59825fdc53f761fd6b38e664db632334c9ab055
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881077"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="60395-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="60395-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="60395-104">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="60395-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="60395-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="60395-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="60395-106">权限</span><span class="sxs-lookup"><span data-stu-id="60395-106">Permissions</span></span>

<span data-ttu-id="60395-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60395-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60395-109">Permission type</span></span>                        | <span data-ttu-id="60395-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60395-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="60395-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60395-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60395-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60395-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="60395-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60395-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60395-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60395-114">Not supported.</span></span>                           |
| <span data-ttu-id="60395-115">应用</span><span class="sxs-lookup"><span data-stu-id="60395-115">Application</span></span>                            | <span data-ttu-id="60395-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60395-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60395-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60395-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60395-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="60395-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="60395-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="60395-119">Request headers</span></span>

| <span data-ttu-id="60395-120">名称</span><span class="sxs-lookup"><span data-stu-id="60395-120">Name</span></span>          | <span data-ttu-id="60395-121">说明</span><span class="sxs-lookup"><span data-stu-id="60395-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="60395-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60395-122">Authorization</span></span> | <span data-ttu-id="60395-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="60395-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="60395-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="60395-125">If-None-Match</span></span> | <span data-ttu-id="60395-126">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="60395-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="60395-127">可选。</span><span class="sxs-lookup"><span data-stu-id="60395-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="60395-128">响应</span><span class="sxs-lookup"><span data-stu-id="60395-128">Response</span></span>

<span data-ttu-id="60395-129">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="60395-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="60395-130">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="60395-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="60395-131">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="60395-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="60395-132">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="60395-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="60395-133">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="60395-133">Report Refresh Date</span></span>
- <span data-ttu-id="60395-134">产品类型</span><span class="sxs-lookup"><span data-stu-id="60395-134">Product Type</span></span>
- <span data-ttu-id="60395-135">Windows</span><span class="sxs-lookup"><span data-stu-id="60395-135">Windows</span></span>
- <span data-ttu-id="60395-136">Mac</span><span class="sxs-lookup"><span data-stu-id="60395-136">Mac</span></span>
- <span data-ttu-id="60395-137">Android</span><span class="sxs-lookup"><span data-stu-id="60395-137">Android</span></span>
- <span data-ttu-id="60395-138">iOS</span><span class="sxs-lookup"><span data-stu-id="60395-138">iOS</span></span>
- <span data-ttu-id="60395-139">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="60395-139">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="60395-140">示例</span><span class="sxs-lookup"><span data-stu-id="60395-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="60395-141">请求</span><span class="sxs-lookup"><span data-stu-id="60395-141">Request</span></span>

<span data-ttu-id="60395-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="60395-142">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60395-143">C#</span><span class="sxs-lookup"><span data-stu-id="60395-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60395-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="60395-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60395-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="60395-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60395-146">Java</span><span class="sxs-lookup"><span data-stu-id="60395-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60395-147">响应</span><span class="sxs-lookup"><span data-stu-id="60395-147">Response</span></span>

<span data-ttu-id="60395-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60395-148">The following is an example of the response.</span></span>

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

<span data-ttu-id="60395-149">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="60395-149">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
