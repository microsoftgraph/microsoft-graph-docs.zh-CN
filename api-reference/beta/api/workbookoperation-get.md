---
title: 获取 workbookOperation
description: 检索 workbookOperation 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bf5f7abd26368b233091ff4294e0f1707c4f01ab
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626186"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="9ac02-103">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="9ac02-103">Get workbookOperation</span></span>

<span data-ttu-id="9ac02-104">检索 [workbookOperation 对象](../resources/workbookoperation.md) 的状态。</span><span class="sxs-lookup"><span data-stu-id="9ac02-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ac02-105">权限</span><span class="sxs-lookup"><span data-stu-id="9ac02-105">Permissions</span></span>

<span data-ttu-id="9ac02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ac02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ac02-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ac02-108">Permission type</span></span>                        | <span data-ttu-id="9ac02-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ac02-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ac02-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ac02-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ac02-111">Files.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="9ac02-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="9ac02-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ac02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ac02-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ac02-113">Not supported.</span></span> |
| <span data-ttu-id="9ac02-114">Application</span><span class="sxs-lookup"><span data-stu-id="9ac02-114">Application</span></span>                            | <span data-ttu-id="9ac02-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ac02-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ac02-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ac02-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="9ac02-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ac02-117">Request headers</span></span>

| <span data-ttu-id="9ac02-118">名称</span><span class="sxs-lookup"><span data-stu-id="9ac02-118">Name</span></span>      |<span data-ttu-id="9ac02-119">说明</span><span class="sxs-lookup"><span data-stu-id="9ac02-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ac02-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ac02-120">Authorization</span></span> | <span data-ttu-id="9ac02-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ac02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ac02-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ac02-123">Request body</span></span>

<span data-ttu-id="9ac02-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ac02-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ac02-125">响应</span><span class="sxs-lookup"><span data-stu-id="9ac02-125">Response</span></span>

<span data-ttu-id="9ac02-126">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [workbookOperation](../resources/workbookoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ac02-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ac02-127">示例</span><span class="sxs-lookup"><span data-stu-id="9ac02-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ac02-128">请求</span><span class="sxs-lookup"><span data-stu-id="9ac02-128">Request</span></span>

<span data-ttu-id="9ac02-129">下面是长时间运行的操作请求的示例。</span><span class="sxs-lookup"><span data-stu-id="9ac02-129">The following is an example of a long-running operation request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ac02-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac02-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="9ac02-131">C#</span><span class="sxs-lookup"><span data-stu-id="9ac02-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ac02-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ac02-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ac02-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ac02-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ac02-134">Java</span><span class="sxs-lookup"><span data-stu-id="9ac02-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ac02-135">响应</span><span class="sxs-lookup"><span data-stu-id="9ac02-135">Response</span></span>

<span data-ttu-id="9ac02-136">下面是状态为"正在运行"的响应。</span><span class="sxs-lookup"><span data-stu-id="9ac02-136">The following is the response with the status of "running".</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "running"
}
```

<span data-ttu-id="9ac02-137">下面是状态为"已成功"的响应。</span><span class="sxs-lookup"><span data-stu-id="9ac02-137">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="9ac02-138">下面是状态为"failed"的响应。</span><span class="sxs-lookup"><span data-stu-id="9ac02-138">The following is the response with the status of "failed".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "failed",
  "error":
  {
      "code": "internalServerError",
      "message": "An internal server error occurred while processing the request.",
      "innerError": {
          "code": ""internalServerErrorUncategorized",
          "message": "An unspecified error has occurred.",
          "innerError": {
               "code": "GenericFileOpenError",
               "message": "The workbook cannot be opened."
          }
      }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


