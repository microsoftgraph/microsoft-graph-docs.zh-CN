---
title: 下载 printDocument 二进制文件
description: 下载与文档关联的二进制文件。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 590b97c01623cba26407ca0a39ad7d0b3b7a1ca3
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034231"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="6cd8d-103">下载 printDocument 二进制文件</span><span class="sxs-lookup"><span data-stu-id="6cd8d-103">Download printDocument binary file</span></span>

<span data-ttu-id="6cd8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cd8d-105">下载与 [printDocument 关联的二进制文件](../resources/printdocument.md)。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="6cd8d-106">调用此方法会生成具有预身份验证 URL 的重定向响应，该 URL 可用于下载负载。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cd8d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6cd8d-107">Permissions</span></span>
<span data-ttu-id="6cd8d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6cd8d-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予获取打印机[访问权限的权限。](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="6cd8d-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="6cd8d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cd8d-111">Permission type</span></span>                        | <span data-ttu-id="6cd8d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cd8d-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6cd8d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cd8d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cd8d-114">PrintJob.Read、PrintJob.Read.All、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd8d-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="6cd8d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cd8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cd8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="6cd8d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cd8d-117">Application</span></span>                            | <span data-ttu-id="6cd8d-118">PrintJob.Read.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd8d-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="6cd8d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cd8d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="6cd8d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cd8d-120">Request headers</span></span>
| <span data-ttu-id="6cd8d-121">名称</span><span class="sxs-lookup"><span data-stu-id="6cd8d-121">Name</span></span>          | <span data-ttu-id="6cd8d-122">说明</span><span class="sxs-lookup"><span data-stu-id="6cd8d-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6cd8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cd8d-123">Authorization</span></span> | <span data-ttu-id="6cd8d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cd8d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cd8d-126">Request body</span></span>
<span data-ttu-id="6cd8d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cd8d-128">响应</span><span class="sxs-lookup"><span data-stu-id="6cd8d-128">Response</span></span>
<span data-ttu-id="6cd8d-129">如果成功，此方法在位置标头中返回和预先 `302 Found` 验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="6cd8d-130">示例</span><span class="sxs-lookup"><span data-stu-id="6cd8d-130">Examples</span></span>
<span data-ttu-id="6cd8d-131">以下示例演示如何调用此 API 以获取预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="6cd8d-132">若要开始下载，请按照响应中的重定向 URL 执行。</span><span class="sxs-lookup"><span data-stu-id="6cd8d-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="6cd8d-133">请求</span><span class="sxs-lookup"><span data-stu-id="6cd8d-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6cd8d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cd8d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[<span data-ttu-id="6cd8d-135">C#</span><span class="sxs-lookup"><span data-stu-id="6cd8d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cd8d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cd8d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cd8d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cd8d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cd8d-138">Java</span><span class="sxs-lookup"><span data-stu-id="6cd8d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6cd8d-139">响应</span><span class="sxs-lookup"><span data-stu-id="6cd8d-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
