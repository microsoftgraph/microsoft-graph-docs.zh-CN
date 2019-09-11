---
title: 创建 workbookCommentReply
description: 创建新的 workbookCommentReply。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2b53390a83172d3ab1c6c144302cf7c76fd219f3
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838917"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="bd3b9-103">创建 workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="bd3b9-103">Create workbookCommentReply</span></span>

<span data-ttu-id="bd3b9-104">创建新的[workbookCommentReply](../resources/workbookcommentreply.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-104">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd3b9-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd3b9-105">Permissions</span></span>

<span data-ttu-id="bd3b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd3b9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd3b9-108">Permission type</span></span>                        | <span data-ttu-id="bd3b9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd3b9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd3b9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd3b9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd3b9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd3b9-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="bd3b9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd3b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd3b9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-113">Not supported.</span></span> |
| <span data-ttu-id="bd3b9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd3b9-114">Application</span></span>                            | <span data-ttu-id="bd3b9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd3b9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd3b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="bd3b9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd3b9-117">Request headers</span></span>

| <span data-ttu-id="bd3b9-118">名称</span><span class="sxs-lookup"><span data-stu-id="bd3b9-118">Name</span></span>          | <span data-ttu-id="bd3b9-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd3b9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd3b9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd3b9-120">Authorization</span></span> | <span data-ttu-id="bd3b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd3b9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd3b9-123">Request body</span></span>

<span data-ttu-id="bd3b9-124">在请求正文中，提供[workbookCommentReply](../resources/workbookcommentreply.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-124">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bd3b9-125">响应</span><span class="sxs-lookup"><span data-stu-id="bd3b9-125">Response</span></span>

<span data-ttu-id="bd3b9-126">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workbookCommentReply](../resources/workbookcommentreply.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-126">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd3b9-127">示例</span><span class="sxs-lookup"><span data-stu-id="bd3b9-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd3b9-128">请求</span><span class="sxs-lookup"><span data-stu-id="bd3b9-128">Request</span></span>

<span data-ttu-id="bd3b9-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd3b9-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bd3b9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/beta/drive/root/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd3b9-131">C#</span><span class="sxs-lookup"><span data-stu-id="bd3b9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd3b9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd3b9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd3b9-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="bd3b9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd3b9-134">响应</span><span class="sxs-lookup"><span data-stu-id="bd3b9-134">Response</span></span>

<span data-ttu-id="bd3b9-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-135">The following is an example of the response.</span></span>

> <span data-ttu-id="bd3b9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd3b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
