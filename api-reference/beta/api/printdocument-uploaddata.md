---
title: printDocument： uploadData
description: Upload printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6435a36e7713435dce3f38145d48083bdabcc532
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787595"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="a4973-103">printDocument： uploadData</span><span class="sxs-lookup"><span data-stu-id="a4973-103">printDocument: uploadData</span></span>

<span data-ttu-id="a4973-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4973-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4973-105">Upload printDocument 的单个二 **进制段**。</span><span class="sxs-lookup"><span data-stu-id="a4973-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="a4973-106">您可以上载整个文件，或将文件拆分为多个字节范围，只要请求不超过 1 MB。</span><span class="sxs-lookup"><span data-stu-id="a4973-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="a4973-107">可按任意顺序上传文件的片段，并且最多可并行上传四个并发请求。</span><span class="sxs-lookup"><span data-stu-id="a4973-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="a4973-108">当上载文档的所有二进制段时，二进制文件将链接到 **printJob**。</span><span class="sxs-lookup"><span data-stu-id="a4973-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4973-109">权限</span><span class="sxs-lookup"><span data-stu-id="a4973-109">Permissions</span></span>
<span data-ttu-id="a4973-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4973-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a4973-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取](printer-get.md) 打印机访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="a4973-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="a4973-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4973-113">Permission type</span></span> | <span data-ttu-id="a4973-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4973-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a4973-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4973-115">Delegated (work or school account)</span></span>| <span data-ttu-id="a4973-116">PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4973-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="a4973-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4973-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4973-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4973-118">Not Supported.</span></span>|
|<span data-ttu-id="a4973-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4973-119">Application</span></span>| <span data-ttu-id="a4973-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4973-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4973-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4973-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="a4973-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4973-122">Request headers</span></span>
| <span data-ttu-id="a4973-123">名称</span><span class="sxs-lookup"><span data-stu-id="a4973-123">Name</span></span>          | <span data-ttu-id="a4973-124">说明</span><span class="sxs-lookup"><span data-stu-id="a4973-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a4973-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4973-125">Authorization</span></span> | <span data-ttu-id="a4973-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4973-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4973-128">范围</span><span class="sxs-lookup"><span data-stu-id="a4973-128">Range</span></span> | <span data-ttu-id="a4973-129">bytes={startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="a4973-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="a4973-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="a4973-130">Content-Length</span></span> | <span data-ttu-id="a4973-131">{contentLength}</span><span class="sxs-lookup"><span data-stu-id="a4973-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="a4973-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="a4973-132">Content-type</span></span>  | <span data-ttu-id="a4973-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a4973-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4973-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4973-135">Request body</span></span>
<span data-ttu-id="a4973-136">请求正文是一个二进制 blob，其中包含在 `Range` 标头中指定为 非独占 字节范围的文档的字节数。</span><span class="sxs-lookup"><span data-stu-id="a4973-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="a4973-137">响应</span><span class="sxs-lookup"><span data-stu-id="a4973-137">Response</span></span>
<span data-ttu-id="a4973-138">如果成功，此方法将返回以下响应之一。</span><span class="sxs-lookup"><span data-stu-id="a4973-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="a4973-139">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a4973-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="a4973-140">条件</span><span class="sxs-lookup"><span data-stu-id="a4973-140">Condition</span></span>     | <span data-ttu-id="a4973-141">响应代码</span><span class="sxs-lookup"><span data-stu-id="a4973-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="a4973-142">仍然需要上载一个或多个二进制段</span><span class="sxs-lookup"><span data-stu-id="a4973-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="a4973-143">已成功上载所有二进制段</span><span class="sxs-lookup"><span data-stu-id="a4973-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="a4973-144">示例</span><span class="sxs-lookup"><span data-stu-id="a4973-144">Example</span></span>
<span data-ttu-id="a4973-145">以下示例演示如何调用此 API 上载文档前 72797 个字节。</span><span class="sxs-lookup"><span data-stu-id="a4973-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="a4973-146">请求</span><span class="sxs-lookup"><span data-stu-id="a4973-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4973-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4973-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="a4973-148">C#</span><span class="sxs-lookup"><span data-stu-id="a4973-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4973-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4973-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4973-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4973-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4973-151">Java</span><span class="sxs-lookup"><span data-stu-id="a4973-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-uploaddata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4973-152">响应</span><span class="sxs-lookup"><span data-stu-id="a4973-152">Response</span></span>

<span data-ttu-id="a4973-153">缺少一个或多个分段：</span><span class="sxs-lookup"><span data-stu-id="a4973-153">One or more segments missing:</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="a4973-154">收到的所有分段：</span><span class="sxs-lookup"><span data-stu-id="a4973-154">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


