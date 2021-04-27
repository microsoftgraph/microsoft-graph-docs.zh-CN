---
title: 指定经理
description: 使用此 API 指定用户的经理。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 05d3f30e3061a39e3104293691448e0f4534790b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049609"
---
# <a name="assign-a-manager"></a><span data-ttu-id="4edd8-103">指定经理</span><span class="sxs-lookup"><span data-stu-id="4edd8-103">Assign a manager</span></span>

<span data-ttu-id="4edd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4edd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4edd8-105">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="4edd8-105">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="4edd8-106">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="4edd8-106">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="4edd8-107">权限</span><span class="sxs-lookup"><span data-stu-id="4edd8-107">Permissions</span></span>
<span data-ttu-id="4edd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4edd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4edd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4edd8-110">Permission type</span></span>      | <span data-ttu-id="4edd8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4edd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4edd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4edd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4edd8-113">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4edd8-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4edd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4edd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4edd8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4edd8-115">Not supported.</span></span>    |
|<span data-ttu-id="4edd8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4edd8-116">Application</span></span> | <span data-ttu-id="4edd8-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4edd8-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4edd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4edd8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4edd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4edd8-119">Request headers</span></span>
| <span data-ttu-id="4edd8-120">名称</span><span class="sxs-lookup"><span data-stu-id="4edd8-120">Name</span></span>       | <span data-ttu-id="4edd8-121">类型</span><span class="sxs-lookup"><span data-stu-id="4edd8-121">Type</span></span> | <span data-ttu-id="4edd8-122">说明</span><span class="sxs-lookup"><span data-stu-id="4edd8-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4edd8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4edd8-123">Authorization</span></span>  | <span data-ttu-id="4edd8-124">string</span><span class="sxs-lookup"><span data-stu-id="4edd8-124">string</span></span>  | <span data-ttu-id="4edd8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4edd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4edd8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4edd8-127">Request body</span></span>
<span data-ttu-id="4edd8-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4edd8-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="4edd8-129">响应</span><span class="sxs-lookup"><span data-stu-id="4edd8-129">Response</span></span>

<span data-ttu-id="4edd8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4edd8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4edd8-132">示例</span><span class="sxs-lookup"><span data-stu-id="4edd8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4edd8-133">请求</span><span class="sxs-lookup"><span data-stu-id="4edd8-133">Request</span></span>
<span data-ttu-id="4edd8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4edd8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4edd8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4edd8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_for_user"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="4edd8-136">C#</span><span class="sxs-lookup"><span data-stu-id="4edd8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-for-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4edd8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4edd8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-for-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4edd8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4edd8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-for-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4edd8-139">Java</span><span class="sxs-lookup"><span data-stu-id="4edd8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-for-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4edd8-140">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4edd8-140">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="4edd8-141">响应</span><span class="sxs-lookup"><span data-stu-id="4edd8-141">Response</span></span>
<span data-ttu-id="4edd8-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4edd8-142">Here is an example of the response.</span></span> <span data-ttu-id="4edd8-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4edd8-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


