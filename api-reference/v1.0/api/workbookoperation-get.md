---
title: 获取 workbookOperation
description: 检索 workbookOperation 对象的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0d790d7bfc243cb5cfbc32a12d6a00db32c46cd9
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408143"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="02574-103">获取 workbookOperation</span><span class="sxs-lookup"><span data-stu-id="02574-103">Get workbookOperation</span></span>

<span data-ttu-id="02574-104">检索[workbookOperation](../resources/workbookoperation.md)对象的状态。</span><span class="sxs-lookup"><span data-stu-id="02574-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02574-105">权限</span><span class="sxs-lookup"><span data-stu-id="02574-105">Permissions</span></span>

<span data-ttu-id="02574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02574-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="02574-108">Permission type</span></span>                        | <span data-ttu-id="02574-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02574-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02574-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02574-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02574-111">文件读写。</span><span class="sxs-lookup"><span data-stu-id="02574-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="02574-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02574-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="02574-113">Not supported.</span></span> |
| <span data-ttu-id="02574-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="02574-114">Application</span></span>                            | <span data-ttu-id="02574-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="02574-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02574-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02574-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="02574-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="02574-117">Request headers</span></span>

| <span data-ttu-id="02574-118">名称</span><span class="sxs-lookup"><span data-stu-id="02574-118">Name</span></span>      |<span data-ttu-id="02574-119">说明</span><span class="sxs-lookup"><span data-stu-id="02574-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02574-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02574-120">Authorization</span></span> | <span data-ttu-id="02574-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02574-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02574-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="02574-123">Request body</span></span>

<span data-ttu-id="02574-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02574-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02574-125">响应</span><span class="sxs-lookup"><span data-stu-id="02574-125">Response</span></span>

<span data-ttu-id="02574-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[workbookOperation](../resources/workbookoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="02574-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02574-127">示例</span><span class="sxs-lookup"><span data-stu-id="02574-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02574-128">请求</span><span class="sxs-lookup"><span data-stu-id="02574-128">Request</span></span>

<span data-ttu-id="02574-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02574-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```

### <a name="response"></a><span data-ttu-id="02574-130">响应</span><span class="sxs-lookup"><span data-stu-id="02574-130">Response</span></span>

<span data-ttu-id="02574-131">以下是状态为 "正在运行" 的响应。</span><span class="sxs-lookup"><span data-stu-id="02574-131">The following is the response with the status of "running".</span></span>


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

<span data-ttu-id="02574-132">以下是状态为 "已成功" 的响应。</span><span class="sxs-lookup"><span data-stu-id="02574-132">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="02574-133">以下是状态为 "失败" 的响应。</span><span class="sxs-lookup"><span data-stu-id="02574-133">The following is the response with the status of "failed".</span></span>

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
