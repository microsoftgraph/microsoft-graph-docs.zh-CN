---
title: printJob： redirect
description: 将打印作业重定向到其他打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7317ba399c284ff0f953a1e14787409f7e0e9939
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921950"
---
# <a name="printjob-redirect"></a><span data-ttu-id="7ebae-103">printJob： redirect</span><span class="sxs-lookup"><span data-stu-id="7ebae-103">printJob: redirect</span></span>

<span data-ttu-id="7ebae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ebae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ebae-105">将 [打印作业重定向到](../resources/printjob.md) 其他 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebae-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="7ebae-106">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="7ebae-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ebae-107">权限</span><span class="sxs-lookup"><span data-stu-id="7ebae-107">Permissions</span></span>
<span data-ttu-id="7ebae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ebae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7ebae-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebae-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="7ebae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ebae-111">Permission type</span></span> | <span data-ttu-id="7ebae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ebae-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7ebae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ebae-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7ebae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ebae-114">Not supported.</span></span> |
|<span data-ttu-id="7ebae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ebae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ebae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ebae-116">Not Supported.</span></span>|
|<span data-ttu-id="7ebae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ebae-117">Application</span></span>| <span data-ttu-id="7ebae-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7ebae-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ebae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ebae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="7ebae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ebae-120">Request headers</span></span>
| <span data-ttu-id="7ebae-121">名称</span><span class="sxs-lookup"><span data-stu-id="7ebae-121">Name</span></span>          | <span data-ttu-id="7ebae-122">说明</span><span class="sxs-lookup"><span data-stu-id="7ebae-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7ebae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ebae-123">Authorization</span></span> | <span data-ttu-id="7ebae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ebae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ebae-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ebae-126">Request body</span></span>
<span data-ttu-id="7ebae-127">在请求正文中，提供打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="7ebae-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="7ebae-128">属性</span><span class="sxs-lookup"><span data-stu-id="7ebae-128">Property</span></span>     | <span data-ttu-id="7ebae-129">类型</span><span class="sxs-lookup"><span data-stu-id="7ebae-129">Type</span></span>        | <span data-ttu-id="7ebae-130">说明</span><span class="sxs-lookup"><span data-stu-id="7ebae-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ebae-131">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="7ebae-131">destinationPrinterId</span></span>|<span data-ttu-id="7ebae-132">String</span><span class="sxs-lookup"><span data-stu-id="7ebae-132">String</span></span>|<span data-ttu-id="7ebae-133">打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="7ebae-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="7ebae-134">configuration</span><span class="sxs-lookup"><span data-stu-id="7ebae-134">configuration</span></span>|<span data-ttu-id="7ebae-135">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ebae-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="7ebae-136">更新了打印作业的配置。</span><span class="sxs-lookup"><span data-stu-id="7ebae-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="7ebae-137">响应</span><span class="sxs-lookup"><span data-stu-id="7ebae-137">Response</span></span>
<span data-ttu-id="7ebae-138">如果成功，此方法返回响应 `200 OK` 代码和一个 [printJob](../resources/printjob.md) 对象排队等待目标打印机。</span><span class="sxs-lookup"><span data-stu-id="7ebae-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="7ebae-139">示例</span><span class="sxs-lookup"><span data-stu-id="7ebae-139">Example</span></span>
<span data-ttu-id="7ebae-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7ebae-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="7ebae-141">请求</span><span class="sxs-lookup"><span data-stu-id="7ebae-141">Request</span></span>
<span data-ttu-id="7ebae-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ebae-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7ebae-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ebae-143">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="7ebae-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ebae-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea",
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7ebae-145">C#</span><span class="sxs-lookup"><span data-stu-id="7ebae-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ebae-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ebae-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ebae-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ebae-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ebae-148">Java</span><span class="sxs-lookup"><span data-stu-id="7ebae-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="7ebae-149">响应</span><span class="sxs-lookup"><span data-stu-id="7ebae-149">Response</span></span>
<span data-ttu-id="7ebae-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7ebae-150">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "processing",
    "description": "The print job is currently being processed by the printer.",
    "details": ["interpreting"]
  },
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


