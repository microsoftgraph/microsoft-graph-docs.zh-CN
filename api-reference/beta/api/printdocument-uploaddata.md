---
title: printDocument： uploadData
description: 上载 printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 62277a2b933edf9161a51b114c765fde948b4d26
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674013"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="e921a-103">printDocument： uploadData</span><span class="sxs-lookup"><span data-stu-id="e921a-103">printDocument: uploadData</span></span>

<span data-ttu-id="e921a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e921a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e921a-105">上载 **printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="e921a-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="e921a-106">您可以上传整个文件，或将文件拆分为多个字节范围，前提是没有请求大于 1 MB。</span><span class="sxs-lookup"><span data-stu-id="e921a-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="e921a-107">可以按任意顺序上载文件的各个部分，并且可以并行上传，最大并发请求数为四个。</span><span class="sxs-lookup"><span data-stu-id="e921a-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="e921a-108">当上载文档的所有二进制片段时，二进制文件将链接到 **printJob**。</span><span class="sxs-lookup"><span data-stu-id="e921a-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e921a-109">权限</span><span class="sxs-lookup"><span data-stu-id="e921a-109">Permissions</span></span>
<span data-ttu-id="e921a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e921a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e921a-112">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="e921a-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="e921a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e921a-113">Permission type</span></span> | <span data-ttu-id="e921a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e921a-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e921a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e921a-115">Delegated (work or school account)</span></span>| <span data-ttu-id="e921a-116">PrintJob，PrintJob。</span><span class="sxs-lookup"><span data-stu-id="e921a-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e921a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e921a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e921a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e921a-118">Not Supported.</span></span>|
|<span data-ttu-id="e921a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e921a-119">Application</span></span>| <span data-ttu-id="e921a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e921a-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e921a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e921a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="e921a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e921a-122">Request headers</span></span>
| <span data-ttu-id="e921a-123">名称</span><span class="sxs-lookup"><span data-stu-id="e921a-123">Name</span></span>          | <span data-ttu-id="e921a-124">说明</span><span class="sxs-lookup"><span data-stu-id="e921a-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e921a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e921a-125">Authorization</span></span> | <span data-ttu-id="e921a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e921a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e921a-128">Range</span><span class="sxs-lookup"><span data-stu-id="e921a-128">Range</span></span> | <span data-ttu-id="e921a-129">bytes = {startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="e921a-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="e921a-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="e921a-130">Content-Length</span></span> | <span data-ttu-id="e921a-131">{contentLength}‬</span><span class="sxs-lookup"><span data-stu-id="e921a-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="e921a-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="e921a-132">Content-type</span></span>  | <span data-ttu-id="e921a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e921a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e921a-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="e921a-135">Request body</span></span>
<span data-ttu-id="e921a-136">请求正文是一个二进制 blob，其中包含指定为标头中的非独占字节范围的文档的字节数 `Range` 。</span><span class="sxs-lookup"><span data-stu-id="e921a-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="e921a-137">响应</span><span class="sxs-lookup"><span data-stu-id="e921a-137">Response</span></span>
<span data-ttu-id="e921a-138">如果成功，此方法将返回以下响应之一。</span><span class="sxs-lookup"><span data-stu-id="e921a-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="e921a-139">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e921a-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="e921a-140">Condition</span><span class="sxs-lookup"><span data-stu-id="e921a-140">Condition</span></span>     | <span data-ttu-id="e921a-141">响应代码</span><span class="sxs-lookup"><span data-stu-id="e921a-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="e921a-142">仍需上载一个或多个二进制段</span><span class="sxs-lookup"><span data-stu-id="e921a-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="e921a-143">已成功上载所有二进制段</span><span class="sxs-lookup"><span data-stu-id="e921a-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="e921a-144">示例</span><span class="sxs-lookup"><span data-stu-id="e921a-144">Example</span></span>
<span data-ttu-id="e921a-145">下面的示例演示如何调用此 API 以上载文档的前72797个字节。</span><span class="sxs-lookup"><span data-stu-id="e921a-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="e921a-146">请求</span><span class="sxs-lookup"><span data-stu-id="e921a-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e921a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e921a-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="e921a-148">C#</span><span class="sxs-lookup"><span data-stu-id="e921a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e921a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e921a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e921a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e921a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e921a-151">响应</span><span class="sxs-lookup"><span data-stu-id="e921a-151">Response</span></span>

<span data-ttu-id="e921a-152">缺少一个或多个段：</span><span class="sxs-lookup"><span data-stu-id="e921a-152">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="e921a-153">接收的所有段：</span><span class="sxs-lookup"><span data-stu-id="e921a-153">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```
