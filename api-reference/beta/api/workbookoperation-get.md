---
title: 获取 workbookOperation
description: 检索 workbookOperation 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c5ead367116603a286574a30551134f9176d1477
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566169"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="4bd42-103">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="4bd42-103">Get workbookOperation</span></span>

<span data-ttu-id="4bd42-104">检索[workbookOperation](../resources/workbookoperation.md)对象的状态。</span><span class="sxs-lookup"><span data-stu-id="4bd42-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bd42-105">权限</span><span class="sxs-lookup"><span data-stu-id="4bd42-105">Permissions</span></span>

<span data-ttu-id="4bd42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bd42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bd42-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bd42-108">Permission type</span></span>                        | <span data-ttu-id="4bd42-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bd42-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4bd42-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd42-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bd42-111">文件读写。</span><span class="sxs-lookup"><span data-stu-id="4bd42-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="4bd42-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bd42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd42-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bd42-113">Not supported.</span></span> |
| <span data-ttu-id="4bd42-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bd42-114">Application</span></span>                            | <span data-ttu-id="4bd42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bd42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd42-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bd42-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="4bd42-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bd42-117">Request headers</span></span>

| <span data-ttu-id="4bd42-118">名称</span><span class="sxs-lookup"><span data-stu-id="4bd42-118">Name</span></span>      |<span data-ttu-id="4bd42-119">说明</span><span class="sxs-lookup"><span data-stu-id="4bd42-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4bd42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd42-120">Authorization</span></span> | <span data-ttu-id="4bd42-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bd42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bd42-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bd42-123">Request body</span></span>

<span data-ttu-id="4bd42-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4bd42-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bd42-125">响应</span><span class="sxs-lookup"><span data-stu-id="4bd42-125">Response</span></span>

<span data-ttu-id="4bd42-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[workbookOperation](../resources/workbookoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bd42-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bd42-127">示例</span><span class="sxs-lookup"><span data-stu-id="4bd42-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4bd42-128">请求</span><span class="sxs-lookup"><span data-stu-id="4bd42-128">Request</span></span>

<span data-ttu-id="4bd42-129">以下是长时间运行的操作请求的示例。</span><span class="sxs-lookup"><span data-stu-id="4bd42-129">The following is an example of a long-running operation request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bd42-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd42-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="4bd42-131">C#</span><span class="sxs-lookup"><span data-stu-id="4bd42-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bd42-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bd42-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bd42-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bd42-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4bd42-134">响应</span><span class="sxs-lookup"><span data-stu-id="4bd42-134">Response</span></span>

<span data-ttu-id="4bd42-135">以下是状态为 "正在运行" 的响应。</span><span class="sxs-lookup"><span data-stu-id="4bd42-135">The following is the response with the status of "running".</span></span>


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

<span data-ttu-id="4bd42-136">以下是状态为 "已成功" 的响应。</span><span class="sxs-lookup"><span data-stu-id="4bd42-136">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="4bd42-137">以下是状态为 "失败" 的响应。</span><span class="sxs-lookup"><span data-stu-id="4bd42-137">The following is the response with the status of "failed".</span></span>

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
