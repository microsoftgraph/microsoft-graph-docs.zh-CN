---
title: 创建附件
description: 使用此 API 可将附件添加到 outlookTask。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 66512eca0fffb72f5f014efe8b06533dc2a294f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450609"
---
# <a name="create-attachment"></a><span data-ttu-id="24fd1-103">创建附件</span><span class="sxs-lookup"><span data-stu-id="24fd1-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24fd1-104">使用此 API 可将[附件](../resources/attachment.md)添加到[outlookTask](../resources/outlooktask.md)。</span><span class="sxs-lookup"><span data-stu-id="24fd1-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24fd1-105">权限</span><span class="sxs-lookup"><span data-stu-id="24fd1-105">Permissions</span></span>

<span data-ttu-id="24fd1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24fd1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="24fd1-108">Permission type</span></span>      | <span data-ttu-id="24fd1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24fd1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24fd1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24fd1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24fd1-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24fd1-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="24fd1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24fd1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24fd1-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24fd1-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="24fd1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="24fd1-114">Application</span></span> | <span data-ttu-id="24fd1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24fd1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24fd1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24fd1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="24fd1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="24fd1-117">Request headers</span></span>

| <span data-ttu-id="24fd1-118">名称</span><span class="sxs-lookup"><span data-stu-id="24fd1-118">Name</span></span>       | <span data-ttu-id="24fd1-119">说明</span><span class="sxs-lookup"><span data-stu-id="24fd1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24fd1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="24fd1-120">Authorization</span></span>  | <span data-ttu-id="24fd1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24fd1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24fd1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24fd1-123">Content-Type</span></span> | <span data-ttu-id="24fd1-124">一个字符串, 表示实体的正文中的数据类型。</span><span class="sxs-lookup"><span data-stu-id="24fd1-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="24fd1-125">必需。</span><span class="sxs-lookup"><span data-stu-id="24fd1-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24fd1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24fd1-126">Request body</span></span>

<span data-ttu-id="24fd1-127">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24fd1-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="24fd1-128">响应</span><span class="sxs-lookup"><span data-stu-id="24fd1-128">Response</span></span>

<span data-ttu-id="24fd1-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24fd1-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fd1-130">示例</span><span class="sxs-lookup"><span data-stu-id="24fd1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="24fd1-131">请求</span><span class="sxs-lookup"><span data-stu-id="24fd1-131">Request</span></span>

<span data-ttu-id="24fd1-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24fd1-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24fd1-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="24fd1-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="24fd1-134">C#</span><span class="sxs-lookup"><span data-stu-id="24fd1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-attachment-from-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24fd1-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="24fd1-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-attachment-from-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24fd1-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="24fd1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-attachment-from-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24fd1-137">响应</span><span class="sxs-lookup"><span data-stu-id="24fd1-137">Response</span></span>

<span data-ttu-id="24fd1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24fd1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
