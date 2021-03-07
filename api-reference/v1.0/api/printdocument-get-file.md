---
title: 下载 printDocument 二进制文件
description: 下载与文档关联的二进制文件。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7bde42e03af509f101515dc847283fc1e354c478
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517281"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="16dd3-103">下载 printDocument 二进制文件</span><span class="sxs-lookup"><span data-stu-id="16dd3-103">Download printDocument binary file</span></span>

<span data-ttu-id="16dd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16dd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="16dd3-105">下载与 [printDocument 关联的二进制文件](../resources/printdocument.md)。</span><span class="sxs-lookup"><span data-stu-id="16dd3-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="16dd3-106">调用此方法会生成重定向响应，该响应具有可用于下载有效负载的预身份验证 URL。</span><span class="sxs-lookup"><span data-stu-id="16dd3-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="16dd3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="16dd3-107">Permissions</span></span>
<span data-ttu-id="16dd3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16dd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="16dd3-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予获取打印机[访问权限的权限。](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="16dd3-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="16dd3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16dd3-111">Permission type</span></span>                        | <span data-ttu-id="16dd3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16dd3-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="16dd3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16dd3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="16dd3-114">PrintJob.Read、PrintJob.Read.All、PrintJob.ReadWrite、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dd3-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="16dd3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16dd3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16dd3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16dd3-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="16dd3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16dd3-117">Application</span></span>                            | <span data-ttu-id="16dd3-118">PrintJob.Read.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dd3-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="16dd3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16dd3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
## <a name="request-headers"></a><span data-ttu-id="16dd3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="16dd3-120">Request headers</span></span>
| <span data-ttu-id="16dd3-121">名称</span><span class="sxs-lookup"><span data-stu-id="16dd3-121">Name</span></span>          | <span data-ttu-id="16dd3-122">说明</span><span class="sxs-lookup"><span data-stu-id="16dd3-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="16dd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16dd3-123">Authorization</span></span> | <span data-ttu-id="16dd3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16dd3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16dd3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16dd3-126">Request body</span></span>
<span data-ttu-id="16dd3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16dd3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16dd3-128">响应</span><span class="sxs-lookup"><span data-stu-id="16dd3-128">Response</span></span>
<span data-ttu-id="16dd3-129">如果成功，此方法在位置标头中返回和 `302 Found` 预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="16dd3-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="16dd3-130">示例</span><span class="sxs-lookup"><span data-stu-id="16dd3-130">Examples</span></span>
<span data-ttu-id="16dd3-131">以下示例演示如何调用此 API 以获取预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="16dd3-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="16dd3-132">若要开始下载，请按照响应中的重定向 URL 执行。</span><span class="sxs-lookup"><span data-stu-id="16dd3-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="16dd3-133">请求</span><span class="sxs-lookup"><span data-stu-id="16dd3-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```

### <a name="response"></a><span data-ttu-id="16dd3-134">响应</span><span class="sxs-lookup"><span data-stu-id="16dd3-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
