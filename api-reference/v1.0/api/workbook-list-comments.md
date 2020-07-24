---
title: 列出 workbookComments
description: 检索 workbookComment 对象的列表。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: feab40fe5e56249ca0653d82084c8636f35e74f2
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408013"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="3dece-103">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="3dece-103">List workbookComments</span></span>

<span data-ttu-id="3dece-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dece-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dece-105">检索[workbookComment](../resources/workbookcomment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3dece-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dece-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dece-106">Permissions</span></span>

<span data-ttu-id="3dece-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dece-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dece-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dece-109">Permission type</span></span>                        | <span data-ttu-id="3dece-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dece-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3dece-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dece-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dece-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3dece-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="3dece-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dece-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dece-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dece-114">Not supported.</span></span> |
| <span data-ttu-id="3dece-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dece-115">Application</span></span>                            | <span data-ttu-id="3dece-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dece-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dece-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dece-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="3dece-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dece-118">Request headers</span></span>

| <span data-ttu-id="3dece-119">名称</span><span class="sxs-lookup"><span data-stu-id="3dece-119">Name</span></span>      |<span data-ttu-id="3dece-120">说明</span><span class="sxs-lookup"><span data-stu-id="3dece-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3dece-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dece-121">Authorization</span></span> | <span data-ttu-id="3dece-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dece-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dece-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dece-124">Request body</span></span>

<span data-ttu-id="3dece-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3dece-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dece-126">响应</span><span class="sxs-lookup"><span data-stu-id="3dece-126">Response</span></span>

<span data-ttu-id="3dece-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[workbookComment](../resources/workbookcomment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3dece-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3dece-128">示例</span><span class="sxs-lookup"><span data-stu-id="3dece-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3dece-129">请求</span><span class="sxs-lookup"><span data-stu-id="3dece-129">Request</span></span>

<span data-ttu-id="3dece-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dece-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dece-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dece-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="3dece-132">C#</span><span class="sxs-lookup"><span data-stu-id="3dece-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dece-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dece-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dece-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dece-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dece-135">Java</span><span class="sxs-lookup"><span data-stu-id="3dece-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3dece-136">响应</span><span class="sxs-lookup"><span data-stu-id="3dece-136">Response</span></span>

<span data-ttu-id="3dece-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3dece-137">The following is an example of the response.</span></span>

> <span data-ttu-id="3dece-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3dece-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is text of comment.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List comments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
