---
title: 下载 printDocument 二进制文件
description: 下载与文档相关联的二进制文件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7e7de914d8549472e08c23f65af25ca99542a58
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273654"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="5a6c6-103">下载 printDocument 二进制文件</span><span class="sxs-lookup"><span data-stu-id="5a6c6-103">Download printDocument binary file</span></span>

<span data-ttu-id="5a6c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a6c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a6c6-105">下载与 [printDocument](../resources/printdocument.md)相关联的二进制文件。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="5a6c6-106">调用此方法将生成一个重定向响应，该响应具有可用于下载有效负载的预验证的 URL。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a6c6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a6c6-107">Permissions</span></span>
<span data-ttu-id="5a6c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5a6c6-110">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="5a6c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a6c6-111">Permission type</span></span>                        | <span data-ttu-id="5a6c6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a6c6-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5a6c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a6c6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a6c6-114">PrintJob、PrintJob、PrintJob、PrintJob、All 和 All</span><span class="sxs-lookup"><span data-stu-id="5a6c6-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="5a6c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a6c6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a6c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="5a6c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a6c6-117">Application</span></span>                            | <span data-ttu-id="5a6c6-118">PrintJob、PrintJob 和所有</span><span class="sxs-lookup"><span data-stu-id="5a6c6-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="5a6c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a6c6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="5a6c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a6c6-120">Request headers</span></span>
| <span data-ttu-id="5a6c6-121">名称</span><span class="sxs-lookup"><span data-stu-id="5a6c6-121">Name</span></span>          | <span data-ttu-id="5a6c6-122">说明</span><span class="sxs-lookup"><span data-stu-id="5a6c6-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5a6c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a6c6-123">Authorization</span></span> | <span data-ttu-id="5a6c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a6c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a6c6-126">Request body</span></span>
<span data-ttu-id="5a6c6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a6c6-128">响应</span><span class="sxs-lookup"><span data-stu-id="5a6c6-128">Response</span></span>
<span data-ttu-id="5a6c6-129">如果成功，此方法 `302 Found` 将在位置标头中返回和预验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="5a6c6-130">示例</span><span class="sxs-lookup"><span data-stu-id="5a6c6-130">Examples</span></span>
<span data-ttu-id="5a6c6-131">下面的示例演示如何调用此 API 以获取预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="5a6c6-132">若要开始下载，请遵循响应中的重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="5a6c6-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="5a6c6-133">请求</span><span class="sxs-lookup"><span data-stu-id="5a6c6-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```

### <a name="response"></a><span data-ttu-id="5a6c6-134">响应</span><span class="sxs-lookup"><span data-stu-id="5a6c6-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
