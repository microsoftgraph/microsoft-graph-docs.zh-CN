---
title: printJob： redirect
description: 将打印作业重定向到其他打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2b99f9e2e6d0def97c1f2a23837f79e61b8e3341
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689313"
---
# <a name="printjob-redirect"></a><span data-ttu-id="8541f-103">printJob： redirect</span><span class="sxs-lookup"><span data-stu-id="8541f-103">printJob: redirect</span></span>

<span data-ttu-id="8541f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8541f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8541f-105">将打印 [作业重定向到](../resources/printjob.md) 其他 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="8541f-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="8541f-106">有关如何使用此 API 向通用打印添加下拉打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="8541f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8541f-107">权限</span><span class="sxs-lookup"><span data-stu-id="8541f-107">Permissions</span></span>
<span data-ttu-id="8541f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8541f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8541f-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅、授予获取打印机访问权限的权限以及下表中列出的权限之一[](printer-get.md)。</span><span class="sxs-lookup"><span data-stu-id="8541f-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="8541f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8541f-111">Permission type</span></span> | <span data-ttu-id="8541f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8541f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8541f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8541f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8541f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8541f-114">Not supported.</span></span> |
|<span data-ttu-id="8541f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8541f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8541f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8541f-116">Not Supported.</span></span>|
|<span data-ttu-id="8541f-117">Application</span><span class="sxs-lookup"><span data-stu-id="8541f-117">Application</span></span>| <span data-ttu-id="8541f-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8541f-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8541f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8541f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="8541f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8541f-120">Request headers</span></span>
| <span data-ttu-id="8541f-121">名称</span><span class="sxs-lookup"><span data-stu-id="8541f-121">Name</span></span>          | <span data-ttu-id="8541f-122">说明</span><span class="sxs-lookup"><span data-stu-id="8541f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8541f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8541f-123">Authorization</span></span> | <span data-ttu-id="8541f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8541f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8541f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8541f-126">Request body</span></span>
<span data-ttu-id="8541f-127">在请求正文中，提供打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="8541f-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="8541f-128">属性</span><span class="sxs-lookup"><span data-stu-id="8541f-128">Property</span></span>     | <span data-ttu-id="8541f-129">类型</span><span class="sxs-lookup"><span data-stu-id="8541f-129">Type</span></span>        | <span data-ttu-id="8541f-130">说明</span><span class="sxs-lookup"><span data-stu-id="8541f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8541f-131">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="8541f-131">destinationPrinterId</span></span>|<span data-ttu-id="8541f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="8541f-132">String</span></span>|<span data-ttu-id="8541f-133">打印作业应重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="8541f-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="8541f-134">configuration</span><span class="sxs-lookup"><span data-stu-id="8541f-134">configuration</span></span>|<span data-ttu-id="8541f-135">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="8541f-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="8541f-136">更新了打印作业的配置。</span><span class="sxs-lookup"><span data-stu-id="8541f-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="8541f-137">响应</span><span class="sxs-lookup"><span data-stu-id="8541f-137">Response</span></span>
<span data-ttu-id="8541f-138">如果成功，此方法将返回一个响应代码和一个排队等待目标打印机 `200 OK` 的 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8541f-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="8541f-139">示例</span><span class="sxs-lookup"><span data-stu-id="8541f-139">Example</span></span>
<span data-ttu-id="8541f-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8541f-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="8541f-141">请求</span><span class="sxs-lookup"><span data-stu-id="8541f-141">Request</span></span>
<span data-ttu-id="8541f-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8541f-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8541f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8541f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
}
```
# <a name="c"></a>[<span data-ttu-id="8541f-144">C#</span><span class="sxs-lookup"><span data-stu-id="8541f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8541f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8541f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8541f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8541f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8541f-147">Java</span><span class="sxs-lookup"><span data-stu-id="8541f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8541f-148">响应</span><span class="sxs-lookup"><span data-stu-id="8541f-148">Response</span></span>
<span data-ttu-id="8541f-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8541f-149">The following is an example of the response.</span></span> 
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
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed by the printer."
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


