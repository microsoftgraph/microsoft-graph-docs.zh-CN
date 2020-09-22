---
title: printDocument： uploadData
description: 上载 printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a06f00b1ff024e116ed7d16cf416d23089f615e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035811"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="27e6e-103">printDocument： uploadData</span><span class="sxs-lookup"><span data-stu-id="27e6e-103">printDocument: uploadData</span></span>

<span data-ttu-id="27e6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27e6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27e6e-105">上载 **printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="27e6e-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="27e6e-106">您可以上传整个文件，或将文件拆分为多个字节范围，前提是没有请求大于 1 MB。</span><span class="sxs-lookup"><span data-stu-id="27e6e-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="27e6e-107">可以按任意顺序上载文件的各个部分，并且可以并行上传，最大并发请求数为四个。</span><span class="sxs-lookup"><span data-stu-id="27e6e-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="27e6e-108">当上载文档的所有二进制片段时，二进制文件将链接到 **printJob**。</span><span class="sxs-lookup"><span data-stu-id="27e6e-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e6e-109">权限</span><span class="sxs-lookup"><span data-stu-id="27e6e-109">Permissions</span></span>
<span data-ttu-id="27e6e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27e6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="27e6e-112">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="27e6e-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="27e6e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="27e6e-113">Permission type</span></span> | <span data-ttu-id="27e6e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27e6e-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="27e6e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27e6e-115">Delegated (work or school account)</span></span>| <span data-ttu-id="27e6e-116">PrintJob，PrintJob。</span><span class="sxs-lookup"><span data-stu-id="27e6e-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="27e6e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27e6e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27e6e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e6e-118">Not Supported.</span></span>|
|<span data-ttu-id="27e6e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="27e6e-119">Application</span></span>| <span data-ttu-id="27e6e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="27e6e-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27e6e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27e6e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="27e6e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="27e6e-122">Request headers</span></span>
| <span data-ttu-id="27e6e-123">名称</span><span class="sxs-lookup"><span data-stu-id="27e6e-123">Name</span></span>          | <span data-ttu-id="27e6e-124">说明</span><span class="sxs-lookup"><span data-stu-id="27e6e-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27e6e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="27e6e-125">Authorization</span></span> | <span data-ttu-id="27e6e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27e6e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27e6e-128">Range</span><span class="sxs-lookup"><span data-stu-id="27e6e-128">Range</span></span> | <span data-ttu-id="27e6e-129">bytes = {startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="27e6e-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="27e6e-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="27e6e-130">Content-Length</span></span> | <span data-ttu-id="27e6e-131">{contentLength}‬</span><span class="sxs-lookup"><span data-stu-id="27e6e-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="27e6e-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="27e6e-132">Content-type</span></span>  | <span data-ttu-id="27e6e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="27e6e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e6e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="27e6e-135">Request body</span></span>
<span data-ttu-id="27e6e-136">请求正文是一个二进制 blob，其中包含指定为标头中的非独占字节范围的文档的字节数 `Range` 。</span><span class="sxs-lookup"><span data-stu-id="27e6e-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="27e6e-137">响应</span><span class="sxs-lookup"><span data-stu-id="27e6e-137">Response</span></span>
<span data-ttu-id="27e6e-138">如果成功，此方法将返回以下响应之一。</span><span class="sxs-lookup"><span data-stu-id="27e6e-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="27e6e-139">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="27e6e-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="27e6e-140">Condition</span><span class="sxs-lookup"><span data-stu-id="27e6e-140">Condition</span></span>     | <span data-ttu-id="27e6e-141">响应代码</span><span class="sxs-lookup"><span data-stu-id="27e6e-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="27e6e-142">仍需上载一个或多个二进制段</span><span class="sxs-lookup"><span data-stu-id="27e6e-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="27e6e-143">已成功上载所有二进制段</span><span class="sxs-lookup"><span data-stu-id="27e6e-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="27e6e-144">示例</span><span class="sxs-lookup"><span data-stu-id="27e6e-144">Example</span></span>
<span data-ttu-id="27e6e-145">下面的示例演示如何调用此 API 以上载文档的前72797个字节。</span><span class="sxs-lookup"><span data-stu-id="27e6e-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="27e6e-146">请求</span><span class="sxs-lookup"><span data-stu-id="27e6e-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="27e6e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="27e6e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="27e6e-148">C#</span><span class="sxs-lookup"><span data-stu-id="27e6e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27e6e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27e6e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27e6e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27e6e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27e6e-151">响应</span><span class="sxs-lookup"><span data-stu-id="27e6e-151">Response</span></span>

<span data-ttu-id="27e6e-152">缺少一个或多个段：</span><span class="sxs-lookup"><span data-stu-id="27e6e-152">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="27e6e-153">接收的所有段：</span><span class="sxs-lookup"><span data-stu-id="27e6e-153">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


