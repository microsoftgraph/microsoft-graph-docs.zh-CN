---
title: 获取 printerShare
description: 检索打印机共享的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c34a3a0c0e425035d71108c98aed7c2aa75c3333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035510"
---
# <a name="get-printershare"></a><span data-ttu-id="779ad-103">获取 printerShare</span><span class="sxs-lookup"><span data-stu-id="779ad-103">Get printerShare</span></span>

<span data-ttu-id="779ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="779ad-105">检索打印机共享的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="779ad-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="779ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="779ad-106">Permissions</span></span>
<span data-ttu-id="779ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="779ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="779ad-109">除了以下权限之外，用户或应用程序的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="779ad-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="779ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="779ad-110">Permission type</span></span> | <span data-ttu-id="779ad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="779ad-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="779ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="779ad-112">Delegated (work or school account)</span></span>| <span data-ttu-id="779ad-113">PrinterShare、PrinterShare 和所有</span><span class="sxs-lookup"><span data-stu-id="779ad-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="779ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="779ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="779ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="779ad-115">Not Supported.</span></span>|
|<span data-ttu-id="779ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="779ad-116">Application</span></span>|<span data-ttu-id="779ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="779ad-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="779ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="779ad-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="779ad-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="779ad-119">Optional query parameters</span></span>
<span data-ttu-id="779ad-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="779ad-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="779ad-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="779ad-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="779ad-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="779ad-122">Exceptions</span></span>
* <span data-ttu-id="779ad-123">`$count`运算符不受支持。</span><span class="sxs-lookup"><span data-stu-id="779ad-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="779ad-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="779ad-124">Request headers</span></span>
| <span data-ttu-id="779ad-125">名称</span><span class="sxs-lookup"><span data-stu-id="779ad-125">Name</span></span>      |<span data-ttu-id="779ad-126">说明</span><span class="sxs-lookup"><span data-stu-id="779ad-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="779ad-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="779ad-127">Authorization</span></span> | <span data-ttu-id="779ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="779ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="779ad-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="779ad-130">Request body</span></span>
<span data-ttu-id="779ad-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="779ad-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="779ad-132">响应</span><span class="sxs-lookup"><span data-stu-id="779ad-132">Response</span></span>
<span data-ttu-id="779ad-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="779ad-133">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="779ad-134">示例</span><span class="sxs-lookup"><span data-stu-id="779ad-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="779ad-135">请求</span><span class="sxs-lookup"><span data-stu-id="779ad-135">Request</span></span>
<span data-ttu-id="779ad-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="779ad-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="779ad-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="779ad-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="779ad-138">C#</span><span class="sxs-lookup"><span data-stu-id="779ad-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="779ad-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="779ad-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="779ad-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="779ad-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="779ad-141">响应</span><span class="sxs-lookup"><span data-stu-id="779ad-141">Response</span></span>
<span data-ttu-id="779ad-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="779ad-142">The following is an example of the response.</span></span>
><span data-ttu-id="779ad-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="779ad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


