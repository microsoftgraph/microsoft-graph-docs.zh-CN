---
title: 创建附件
description: 使用此 API 可将附件添加到 outlookTask。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1eefcc0ddb25d3ac3195687b9c220a94000621e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349894"
---
# <a name="create-attachment"></a><span data-ttu-id="9ed58-103">创建附件</span><span class="sxs-lookup"><span data-stu-id="9ed58-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed58-104">使用此 API 可将[附件](../resources/attachment.md)添加到[outlookTask](../resources/outlooktask.md)。</span><span class="sxs-lookup"><span data-stu-id="9ed58-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed58-105">权限</span><span class="sxs-lookup"><span data-stu-id="9ed58-105">Permissions</span></span>

<span data-ttu-id="9ed58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ed58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed58-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ed58-108">Permission type</span></span>      | <span data-ttu-id="9ed58-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ed58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed58-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed58-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed58-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9ed58-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed58-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed58-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9ed58-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ed58-114">Application</span></span> | <span data-ttu-id="9ed58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ed58-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed58-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ed58-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="9ed58-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ed58-117">Request headers</span></span>

| <span data-ttu-id="9ed58-118">名称</span><span class="sxs-lookup"><span data-stu-id="9ed58-118">Name</span></span>       | <span data-ttu-id="9ed58-119">说明</span><span class="sxs-lookup"><span data-stu-id="9ed58-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ed58-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed58-120">Authorization</span></span>  | <span data-ttu-id="9ed58-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ed58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ed58-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ed58-123">Content-Type</span></span> | <span data-ttu-id="9ed58-124">一个字符串, 表示实体的正文中的数据类型。</span><span class="sxs-lookup"><span data-stu-id="9ed58-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="9ed58-125">必需。</span><span class="sxs-lookup"><span data-stu-id="9ed58-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed58-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ed58-126">Request body</span></span>

<span data-ttu-id="9ed58-127">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ed58-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9ed58-128">响应</span><span class="sxs-lookup"><span data-stu-id="9ed58-128">Response</span></span>

<span data-ttu-id="9ed58-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ed58-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ed58-130">示例</span><span class="sxs-lookup"><span data-stu-id="9ed58-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ed58-131">请求</span><span class="sxs-lookup"><span data-stu-id="9ed58-131">Request</span></span>

<span data-ttu-id="9ed58-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ed58-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ed58-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9ed58-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ed58-134">C#</span><span class="sxs-lookup"><span data-stu-id="9ed58-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-attachment-from-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ed58-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed58-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-attachment-from-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ed58-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="9ed58-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-attachment-from-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ed58-137">Java</span><span class="sxs-lookup"><span data-stu-id="9ed58-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-attachment-from-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ed58-138">响应</span><span class="sxs-lookup"><span data-stu-id="9ed58-138">Response</span></span>

<span data-ttu-id="9ed58-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ed58-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
