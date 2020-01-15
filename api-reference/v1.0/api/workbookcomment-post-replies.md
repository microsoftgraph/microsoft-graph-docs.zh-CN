---
title: 创建 workbookCommentReply
description: 使用此 API 创建新的 workbookCommentReply。
localization_priority: Normal
author: grangeryy
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e75299e8eaf35b4c25b9da244422116f8227e088
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119768"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="9668d-103">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9668d-103">Create workbookCommentReply</span></span>

<span data-ttu-id="9668d-104">创建新的[workbookCommentReply](../resources/workbookcommentreply.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9668d-104">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9668d-105">权限</span><span class="sxs-lookup"><span data-stu-id="9668d-105">Permissions</span></span>

<span data-ttu-id="9668d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9668d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9668d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9668d-108">Permission type</span></span>                        | <span data-ttu-id="9668d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9668d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9668d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9668d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9668d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9668d-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="9668d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9668d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9668d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9668d-113">Not supported.</span></span> |
| <span data-ttu-id="9668d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9668d-114">Application</span></span>                            | <span data-ttu-id="9668d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9668d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9668d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9668d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="9668d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9668d-117">Request headers</span></span>

| <span data-ttu-id="9668d-118">名称</span><span class="sxs-lookup"><span data-stu-id="9668d-118">Name</span></span>          | <span data-ttu-id="9668d-119">说明</span><span class="sxs-lookup"><span data-stu-id="9668d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9668d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9668d-120">Authorization</span></span> | <span data-ttu-id="9668d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9668d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9668d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9668d-123">Request body</span></span>

<span data-ttu-id="9668d-124">在请求正文中，提供[workbookCommentReply](../resources/workbookcommentreply.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9668d-124">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9668d-125">响应</span><span class="sxs-lookup"><span data-stu-id="9668d-125">Response</span></span>

<span data-ttu-id="9668d-126">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workbookCommentReply](../resources/workbookcommentreply.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9668d-126">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9668d-127">示例</span><span class="sxs-lookup"><span data-stu-id="9668d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9668d-128">请求</span><span class="sxs-lookup"><span data-stu-id="9668d-128">Request</span></span>

<span data-ttu-id="9668d-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9668d-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9668d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9668d-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9668d-131">C#</span><span class="sxs-lookup"><span data-stu-id="9668d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9668d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9668d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9668d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9668d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9668d-134">Java</span><span class="sxs-lookup"><span data-stu-id="9668d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9668d-135">响应</span><span class="sxs-lookup"><span data-stu-id="9668d-135">Response</span></span>

<span data-ttu-id="9668d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9668d-136">The following is an example of the response.</span></span>

> <span data-ttu-id="9668d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9668d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
