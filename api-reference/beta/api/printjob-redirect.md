---
title: printJob： redirect
description: 将打印作业重定向到其他打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 916725283b86c59907ddd89e5441902fa0f8c756
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080174"
---
# <a name="printjob-redirect"></a><span data-ttu-id="22eba-103">printJob： redirect</span><span class="sxs-lookup"><span data-stu-id="22eba-103">printJob: redirect</span></span>

<span data-ttu-id="22eba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22eba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22eba-105">将 [打印作业重定向到](../resources/printjob.md) 其他 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="22eba-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="22eba-106">只有在关联的打印作业上存在由请求应用创建的触发器启动的 [printTask](../resources/printTask.md) 状态时，重定向打印作业才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="22eba-106">Redirecting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> 

<span data-ttu-id="22eba-107">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="22eba-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="22eba-108">权限</span><span class="sxs-lookup"><span data-stu-id="22eba-108">Permissions</span></span>
<span data-ttu-id="22eba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22eba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="22eba-111">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="22eba-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="22eba-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="22eba-112">Permission type</span></span> | <span data-ttu-id="22eba-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22eba-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="22eba-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22eba-114">Delegated (work or school account)</span></span>| <span data-ttu-id="22eba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22eba-115">Not supported.</span></span> |
|<span data-ttu-id="22eba-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22eba-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22eba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22eba-117">Not Supported.</span></span>|
|<span data-ttu-id="22eba-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="22eba-118">Application</span></span>| <span data-ttu-id="22eba-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="22eba-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22eba-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22eba-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="22eba-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22eba-121">Request headers</span></span>
| <span data-ttu-id="22eba-122">名称</span><span class="sxs-lookup"><span data-stu-id="22eba-122">Name</span></span>          | <span data-ttu-id="22eba-123">说明</span><span class="sxs-lookup"><span data-stu-id="22eba-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22eba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22eba-124">Authorization</span></span> | <span data-ttu-id="22eba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22eba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22eba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22eba-127">Request body</span></span>
<span data-ttu-id="22eba-128">在请求正文中，提供打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="22eba-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="22eba-129">属性</span><span class="sxs-lookup"><span data-stu-id="22eba-129">Property</span></span>     | <span data-ttu-id="22eba-130">类型</span><span class="sxs-lookup"><span data-stu-id="22eba-130">Type</span></span>        | <span data-ttu-id="22eba-131">说明</span><span class="sxs-lookup"><span data-stu-id="22eba-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22eba-132">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="22eba-132">destinationPrinterId</span></span>|<span data-ttu-id="22eba-133">String</span><span class="sxs-lookup"><span data-stu-id="22eba-133">String</span></span>|<span data-ttu-id="22eba-134">打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="22eba-134">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="22eba-135">configuration</span><span class="sxs-lookup"><span data-stu-id="22eba-135">configuration</span></span>|<span data-ttu-id="22eba-136">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="22eba-136">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="22eba-137">更新了打印作业的配置。</span><span class="sxs-lookup"><span data-stu-id="22eba-137">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="22eba-138">响应</span><span class="sxs-lookup"><span data-stu-id="22eba-138">Response</span></span>
<span data-ttu-id="22eba-139">如果成功，此方法返回响应 `200 OK` 代码和一个 [printJob](../resources/printjob.md) 对象排队等待目标打印机。</span><span class="sxs-lookup"><span data-stu-id="22eba-139">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="22eba-140">示例</span><span class="sxs-lookup"><span data-stu-id="22eba-140">Example</span></span>
<span data-ttu-id="22eba-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="22eba-141">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="22eba-142">请求</span><span class="sxs-lookup"><span data-stu-id="22eba-142">Request</span></span>
<span data-ttu-id="22eba-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22eba-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22eba-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="22eba-144">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="22eba-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="22eba-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="22eba-146">C#</span><span class="sxs-lookup"><span data-stu-id="22eba-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22eba-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22eba-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22eba-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22eba-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22eba-149">Java</span><span class="sxs-lookup"><span data-stu-id="22eba-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="22eba-150">响应</span><span class="sxs-lookup"><span data-stu-id="22eba-150">Response</span></span>
<span data-ttu-id="22eba-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22eba-151">The following is an example of the response.</span></span> 
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


