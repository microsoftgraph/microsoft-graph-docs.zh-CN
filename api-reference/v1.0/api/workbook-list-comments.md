---
title: 列出 workbookComments
description: 检索 workbookComment 对象的列表。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 11ec3c796207e216734fb9e858b7fb0fd9ef0007
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031497"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="b2afd-103">列出 workbookComments</span><span class="sxs-lookup"><span data-stu-id="b2afd-103">List workbookComments</span></span>

<span data-ttu-id="b2afd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2afd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2afd-105">检索  [workbookComment 对象](../resources/workbookcomment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="b2afd-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2afd-106">权限</span><span class="sxs-lookup"><span data-stu-id="b2afd-106">Permissions</span></span>

<span data-ttu-id="b2afd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2afd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2afd-109">Permission type</span></span>                        | <span data-ttu-id="b2afd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2afd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2afd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2afd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2afd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2afd-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="b2afd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2afd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2afd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2afd-114">Not supported.</span></span> |
| <span data-ttu-id="b2afd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2afd-115">Application</span></span>                            | <span data-ttu-id="b2afd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2afd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2afd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2afd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="b2afd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2afd-118">Request headers</span></span>

| <span data-ttu-id="b2afd-119">名称</span><span class="sxs-lookup"><span data-stu-id="b2afd-119">Name</span></span>      |<span data-ttu-id="b2afd-120">说明</span><span class="sxs-lookup"><span data-stu-id="b2afd-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2afd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2afd-121">Authorization</span></span> | <span data-ttu-id="b2afd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2afd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2afd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2afd-124">Request body</span></span>

<span data-ttu-id="b2afd-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2afd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2afd-126">响应</span><span class="sxs-lookup"><span data-stu-id="b2afd-126">Response</span></span>

<span data-ttu-id="b2afd-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [workbookComment](../resources/workbookcomment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2afd-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2afd-128">示例</span><span class="sxs-lookup"><span data-stu-id="b2afd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2afd-129">请求</span><span class="sxs-lookup"><span data-stu-id="b2afd-129">Request</span></span>

<span data-ttu-id="b2afd-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2afd-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2afd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2afd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="b2afd-132">C#</span><span class="sxs-lookup"><span data-stu-id="b2afd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2afd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2afd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2afd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2afd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2afd-135">Java</span><span class="sxs-lookup"><span data-stu-id="b2afd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2afd-136">响应</span><span class="sxs-lookup"><span data-stu-id="b2afd-136">Response</span></span>

<span data-ttu-id="b2afd-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2afd-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b2afd-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2afd-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

