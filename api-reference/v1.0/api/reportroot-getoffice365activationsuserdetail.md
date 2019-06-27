---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: 获取已激活 Office 365 的用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a6b8e47017f42762dfd9e3e6f8b2792c562004b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268703"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="b136e-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="b136e-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="b136e-104">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b136e-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="b136e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="b136e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b136e-106">权限</span><span class="sxs-lookup"><span data-stu-id="b136e-106">Permissions</span></span>

<span data-ttu-id="b136e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b136e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b136e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b136e-109">Permission type</span></span>                        | <span data-ttu-id="b136e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b136e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b136e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b136e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b136e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b136e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b136e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b136e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b136e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b136e-114">Not supported.</span></span>                           |
| <span data-ttu-id="b136e-115">应用</span><span class="sxs-lookup"><span data-stu-id="b136e-115">Application</span></span>                            | <span data-ttu-id="b136e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b136e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b136e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b136e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="b136e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b136e-118">Request headers</span></span>

| <span data-ttu-id="b136e-119">名称</span><span class="sxs-lookup"><span data-stu-id="b136e-119">Name</span></span>          | <span data-ttu-id="b136e-120">说明</span><span class="sxs-lookup"><span data-stu-id="b136e-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b136e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b136e-121">Authorization</span></span> | <span data-ttu-id="b136e-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b136e-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b136e-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b136e-124">If-None-Match</span></span> | <span data-ttu-id="b136e-125">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b136e-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b136e-126">可选。</span><span class="sxs-lookup"><span data-stu-id="b136e-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b136e-127">响应</span><span class="sxs-lookup"><span data-stu-id="b136e-127">Response</span></span>

<span data-ttu-id="b136e-128">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b136e-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b136e-129">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b136e-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b136e-130">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b136e-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b136e-131">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b136e-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b136e-132">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b136e-132">Report Refresh Date</span></span>
- <span data-ttu-id="b136e-133">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b136e-133">User Principal Name</span></span>
- <span data-ttu-id="b136e-134">显示名称</span><span class="sxs-lookup"><span data-stu-id="b136e-134">Display Name</span></span>
- <span data-ttu-id="b136e-135">产品类型</span><span class="sxs-lookup"><span data-stu-id="b136e-135">Product Type</span></span>
- <span data-ttu-id="b136e-136">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="b136e-136">Last Activated Date</span></span>
- <span data-ttu-id="b136e-137">Windows</span><span class="sxs-lookup"><span data-stu-id="b136e-137">Windows</span></span>
- <span data-ttu-id="b136e-138">Mac</span><span class="sxs-lookup"><span data-stu-id="b136e-138">Mac</span></span>
- <span data-ttu-id="b136e-139">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="b136e-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="b136e-140">iOS</span><span class="sxs-lookup"><span data-stu-id="b136e-140">iOS</span></span>
- <span data-ttu-id="b136e-141">Android</span><span class="sxs-lookup"><span data-stu-id="b136e-141">Android</span></span>
- <span data-ttu-id="b136e-142">在共享计算机上激活</span><span class="sxs-lookup"><span data-stu-id="b136e-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="b136e-143">示例</span><span class="sxs-lookup"><span data-stu-id="b136e-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b136e-144">请求</span><span class="sxs-lookup"><span data-stu-id="b136e-144">Request</span></span>

<span data-ttu-id="b136e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b136e-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="b136e-146">响应</span><span class="sxs-lookup"><span data-stu-id="b136e-146">Response</span></span>

<span data-ttu-id="b136e-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b136e-147">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b136e-148">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b136e-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b136e-149">C#</span><span class="sxs-lookup"><span data-stu-id="b136e-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b136e-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="b136e-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b136e-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="b136e-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b136e-152">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b136e-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
