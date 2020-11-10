---
title: printJob：重定向
description: 将打印作业重定向到其他打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a047641696f0882e83a3b84aa215084083d245b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968287"
---
# <a name="printjob-redirect"></a><span data-ttu-id="474a5-103">printJob：重定向</span><span class="sxs-lookup"><span data-stu-id="474a5-103">printJob: redirect</span></span>

<span data-ttu-id="474a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="474a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="474a5-105">将 [打印作业](../resources/printjob.md) 重定向到其他 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="474a5-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="474a5-106">有关如何使用此 API 将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持请求打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="474a5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="474a5-107">将删除在2天内未重定向的已暂停打印作业。</span><span class="sxs-lookup"><span data-stu-id="474a5-107">Paused print jobs that are not redirected within 2 days will be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="474a5-108">权限</span><span class="sxs-lookup"><span data-stu-id="474a5-108">Permissions</span></span>
<span data-ttu-id="474a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="474a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="474a5-111">若要使用通用打印服务，用户或应用程序的租户必须具有活动的通用打印订阅、授予 " [获取打印机](printer-get.md) 访问" 权限的权限以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="474a5-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="474a5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="474a5-112">Permission type</span></span> | <span data-ttu-id="474a5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="474a5-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="474a5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="474a5-114">Delegated (work or school account)</span></span>| <span data-ttu-id="474a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="474a5-115">Not supported.</span></span> |
|<span data-ttu-id="474a5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="474a5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474a5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="474a5-117">Not Supported.</span></span>|
|<span data-ttu-id="474a5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="474a5-118">Application</span></span>| <span data-ttu-id="474a5-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="474a5-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="474a5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="474a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="474a5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="474a5-121">Request headers</span></span>
| <span data-ttu-id="474a5-122">名称</span><span class="sxs-lookup"><span data-stu-id="474a5-122">Name</span></span>          | <span data-ttu-id="474a5-123">说明</span><span class="sxs-lookup"><span data-stu-id="474a5-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="474a5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="474a5-124">Authorization</span></span> | <span data-ttu-id="474a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="474a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="474a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="474a5-127">Request body</span></span>
<span data-ttu-id="474a5-128">在请求正文中，提供应将打印作业重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="474a5-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="474a5-129">属性</span><span class="sxs-lookup"><span data-stu-id="474a5-129">Property</span></span>     | <span data-ttu-id="474a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="474a5-130">Type</span></span>        | <span data-ttu-id="474a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="474a5-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="474a5-132">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="474a5-132">destinationPrinterId</span></span>|<span data-ttu-id="474a5-133">String</span><span class="sxs-lookup"><span data-stu-id="474a5-133">String</span></span>|<span data-ttu-id="474a5-134">应将打印作业重定向到的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="474a5-134">The ID of the printer the print job should be redirected to.</span></span>|

## <a name="response"></a><span data-ttu-id="474a5-135">响应</span><span class="sxs-lookup"><span data-stu-id="474a5-135">Response</span></span>
<span data-ttu-id="474a5-136">如果成功，此方法将返回 `200 OK` 排队等候目标打印机的响应代码和 [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="474a5-136">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="474a5-137">示例</span><span class="sxs-lookup"><span data-stu-id="474a5-137">Example</span></span>
<span data-ttu-id="474a5-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="474a5-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="474a5-139">请求</span><span class="sxs-lookup"><span data-stu-id="474a5-139">Request</span></span>
<span data-ttu-id="474a5-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="474a5-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="474a5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="474a5-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="474a5-142">C#</span><span class="sxs-lookup"><span data-stu-id="474a5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="474a5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="474a5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="474a5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="474a5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="474a5-145">Java</span><span class="sxs-lookup"><span data-stu-id="474a5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="474a5-146">响应</span><span class="sxs-lookup"><span data-stu-id="474a5-146">Response</span></span>
<span data-ttu-id="474a5-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="474a5-147">The following is an example of the response.</span></span> 
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


