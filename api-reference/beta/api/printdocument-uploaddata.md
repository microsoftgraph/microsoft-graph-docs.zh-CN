---
title: printDocument： uploadData
description: 上载 printDocument 的单个二进制段。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7592de07f74aa6fb715a90b2becad57a0e14b194
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895703"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="c5822-103">printDocument： uploadData</span><span class="sxs-lookup"><span data-stu-id="c5822-103">printDocument: uploadData</span></span>

<span data-ttu-id="c5822-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5822-105">上载**printDocument**的单个二进制段。</span><span class="sxs-lookup"><span data-stu-id="c5822-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="c5822-106">您可以上传整个文件，或将文件拆分为多个字节范围，前提是没有请求大于 1 MB。</span><span class="sxs-lookup"><span data-stu-id="c5822-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="c5822-107">可以按任意顺序上载文件的各个部分，并且可以并行上传，最大并发请求数为四个。</span><span class="sxs-lookup"><span data-stu-id="c5822-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="c5822-108">当上载文档的所有二进制片段时，二进制文件将链接到**printJob**。</span><span class="sxs-lookup"><span data-stu-id="c5822-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5822-109">权限</span><span class="sxs-lookup"><span data-stu-id="c5822-109">Permissions</span></span>
<span data-ttu-id="c5822-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5822-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c5822-112">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="c5822-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c5822-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5822-113">Permission type</span></span> | <span data-ttu-id="c5822-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5822-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c5822-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5822-115">Delegated (work or school account)</span></span>| <span data-ttu-id="c5822-116">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="c5822-116">Users.Read.All</span></span> |
|<span data-ttu-id="c5822-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5822-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5822-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5822-118">Not Supported.</span></span>|
|<span data-ttu-id="c5822-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5822-119">Application</span></span>|<span data-ttu-id="c5822-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5822-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5822-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5822-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="c5822-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5822-122">Request headers</span></span>
| <span data-ttu-id="c5822-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5822-123">Name</span></span>          | <span data-ttu-id="c5822-124">说明</span><span class="sxs-lookup"><span data-stu-id="c5822-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c5822-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5822-125">Authorization</span></span> | <span data-ttu-id="c5822-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5822-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5822-128">范围</span><span class="sxs-lookup"><span data-stu-id="c5822-128">Range</span></span> | <span data-ttu-id="c5822-129">bytes = {startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="c5822-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="c5822-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="c5822-130">Content-Length</span></span> | <span data-ttu-id="c5822-131">{contentLength}‬</span><span class="sxs-lookup"><span data-stu-id="c5822-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="c5822-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="c5822-132">Content-type</span></span>  | <span data-ttu-id="c5822-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c5822-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5822-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5822-135">Request body</span></span>
<span data-ttu-id="c5822-136">请求正文是一个二进制 blob，其中包含指定为`Range`标头中的非独占字节范围的文档的字节数。</span><span class="sxs-lookup"><span data-stu-id="c5822-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="c5822-137">响应</span><span class="sxs-lookup"><span data-stu-id="c5822-137">Response</span></span>
<span data-ttu-id="c5822-138">如果成功，此方法将返回以下响应之一。</span><span class="sxs-lookup"><span data-stu-id="c5822-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="c5822-139">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c5822-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="c5822-140">条件</span><span class="sxs-lookup"><span data-stu-id="c5822-140">Condition</span></span>     | <span data-ttu-id="c5822-141">响应代码</span><span class="sxs-lookup"><span data-stu-id="c5822-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="c5822-142">仍需上载一个或多个二进制段</span><span class="sxs-lookup"><span data-stu-id="c5822-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="c5822-143">已成功上载所有二进制段</span><span class="sxs-lookup"><span data-stu-id="c5822-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="c5822-144">示例</span><span class="sxs-lookup"><span data-stu-id="c5822-144">Example</span></span>
<span data-ttu-id="c5822-145">下面的示例演示如何调用此 API 以上载文档的前72797个字节。</span><span class="sxs-lookup"><span data-stu-id="c5822-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="c5822-146">请求</span><span class="sxs-lookup"><span data-stu-id="c5822-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
##### <a name="response"></a><span data-ttu-id="c5822-147">响应</span><span class="sxs-lookup"><span data-stu-id="c5822-147">Response</span></span>

<span data-ttu-id="c5822-148">缺少一个或多个段：</span><span class="sxs-lookup"><span data-stu-id="c5822-148">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="c5822-149">接收的所有段：</span><span class="sxs-lookup"><span data-stu-id="c5822-149">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```