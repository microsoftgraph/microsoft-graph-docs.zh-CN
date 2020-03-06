---
title: 获取 workbookComment
description: 检索 workbookcomment 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7e0a59c3c8c6deceb28aadd6fbc58e18ace0e5b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508812"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="26255-103">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="26255-103">Get workbookComment</span></span>

<span data-ttu-id="26255-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26255-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26255-105">检索[workbookComment](../resources/workbookcomment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26255-105">Retrieve the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26255-106">权限</span><span class="sxs-lookup"><span data-stu-id="26255-106">Permissions</span></span>

<span data-ttu-id="26255-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26255-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26255-109">Permission type</span></span>                        | <span data-ttu-id="26255-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26255-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26255-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26255-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26255-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26255-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="26255-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26255-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26255-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26255-114">Not supported.</span></span> |
| <span data-ttu-id="26255-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26255-115">Application</span></span>                            | <span data-ttu-id="26255-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="26255-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26255-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26255-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26255-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26255-118">Request headers</span></span>

| <span data-ttu-id="26255-119">名称</span><span class="sxs-lookup"><span data-stu-id="26255-119">Name</span></span>      |<span data-ttu-id="26255-120">说明</span><span class="sxs-lookup"><span data-stu-id="26255-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26255-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26255-121">Authorization</span></span> | <span data-ttu-id="26255-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26255-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26255-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="26255-124">Request body</span></span>

<span data-ttu-id="26255-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26255-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26255-126">响应</span><span class="sxs-lookup"><span data-stu-id="26255-126">Response</span></span>

<span data-ttu-id="26255-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[workbookComment](../resources/workbookcomment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26255-127">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26255-128">示例</span><span class="sxs-lookup"><span data-stu-id="26255-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26255-129">请求</span><span class="sxs-lookup"><span data-stu-id="26255-129">Request</span></span>

<span data-ttu-id="26255-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26255-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26255-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="26255-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}
```
# <a name="c"></a>[<span data-ttu-id="26255-132">C#</span><span class="sxs-lookup"><span data-stu-id="26255-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26255-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26255-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26255-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26255-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26255-135">Java</span><span class="sxs-lookup"><span data-stu-id="26255-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26255-136">响应</span><span class="sxs-lookup"><span data-stu-id="26255-136">Response</span></span>

<span data-ttu-id="26255-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26255-137">The following is an example of the response.</span></span>

> <span data-ttu-id="26255-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26255-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is my comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookComment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
