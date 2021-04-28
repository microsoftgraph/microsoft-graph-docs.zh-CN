---
title: 创建 workbookCommentReply
description: 使用此 API 创建新的 workbookCommentReply。
localization_priority: Normal
author: grangeryy
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e52a08fab6caad40cedf4fa72e0b16fc7aa5214b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053746"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="17a1a-103">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="17a1a-103">Create workbookCommentReply</span></span>

<span data-ttu-id="17a1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17a1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17a1a-105">创建新的 [workbookCommentReply](../resources/workbookcommentreply.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17a1a-105">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17a1a-106">权限</span><span class="sxs-lookup"><span data-stu-id="17a1a-106">Permissions</span></span>

<span data-ttu-id="17a1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17a1a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17a1a-109">Permission type</span></span>                        | <span data-ttu-id="17a1a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17a1a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="17a1a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17a1a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17a1a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17a1a-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="17a1a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17a1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17a1a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="17a1a-114">Not supported.</span></span> |
| <span data-ttu-id="17a1a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="17a1a-115">Application</span></span>                            | <span data-ttu-id="17a1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17a1a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17a1a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17a1a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{id}/workbook/comments/{id}/replies
POST /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="17a1a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="17a1a-118">Request headers</span></span>

| <span data-ttu-id="17a1a-119">名称</span><span class="sxs-lookup"><span data-stu-id="17a1a-119">Name</span></span>          | <span data-ttu-id="17a1a-120">说明</span><span class="sxs-lookup"><span data-stu-id="17a1a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="17a1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17a1a-121">Authorization</span></span> | <span data-ttu-id="17a1a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17a1a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17a1a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="17a1a-124">Request body</span></span>

<span data-ttu-id="17a1a-125">在请求正文中，提供 [workbookCommentReply](../resources/workbookcommentreply.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17a1a-125">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="17a1a-126">响应</span><span class="sxs-lookup"><span data-stu-id="17a1a-126">Response</span></span>

<span data-ttu-id="17a1a-127">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [workbookCommentReply](../resources/workbookcommentreply.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17a1a-127">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17a1a-128">示例</span><span class="sxs-lookup"><span data-stu-id="17a1a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17a1a-129">请求</span><span class="sxs-lookup"><span data-stu-id="17a1a-129">Request</span></span>

<span data-ttu-id="17a1a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17a1a-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17a1a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="17a1a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="c"></a>[<span data-ttu-id="17a1a-132">C#</span><span class="sxs-lookup"><span data-stu-id="17a1a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17a1a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17a1a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17a1a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17a1a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17a1a-135">Java</span><span class="sxs-lookup"><span data-stu-id="17a1a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17a1a-136">响应</span><span class="sxs-lookup"><span data-stu-id="17a1a-136">Response</span></span>

<span data-ttu-id="17a1a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17a1a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="17a1a-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="17a1a-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

