---
title: 分配管理器
description: 分配用户的经理。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cc9b4547e3b2e62a59f8827a88ba1e58a693aa10
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108296"
---
# <a name="assign-manager"></a><span data-ttu-id="2d04b-103">分配管理器</span><span class="sxs-lookup"><span data-stu-id="2d04b-103">Assign manager</span></span>

<span data-ttu-id="2d04b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d04b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d04b-105">分配用户的经理。</span><span class="sxs-lookup"><span data-stu-id="2d04b-105">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="2d04b-106">您不能分配直接下属，也不能分配。而是使用此 API。</span><span class="sxs-lookup"><span data-stu-id="2d04b-106">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d04b-107">权限</span><span class="sxs-lookup"><span data-stu-id="2d04b-107">Permissions</span></span>
<span data-ttu-id="2d04b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d04b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d04b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d04b-110">Permission type</span></span>      | <span data-ttu-id="2d04b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d04b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d04b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d04b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d04b-113">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d04b-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d04b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d04b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d04b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d04b-115">Not supported.</span></span>    |
|<span data-ttu-id="2d04b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d04b-116">Application</span></span> | <span data-ttu-id="2d04b-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d04b-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d04b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d04b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2d04b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d04b-119">Request headers</span></span>
| <span data-ttu-id="2d04b-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d04b-120">Header</span></span>       | <span data-ttu-id="2d04b-121">值</span><span class="sxs-lookup"><span data-stu-id="2d04b-121">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2d04b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d04b-122">Authorization</span></span>  | <span data-ttu-id="2d04b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d04b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d04b-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="2d04b-125">Content-type</span></span>   | <span data-ttu-id="2d04b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2d04b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d04b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d04b-128">Request body</span></span>
<span data-ttu-id="2d04b-129">在请求正文中，提供要添加的[directoryObject](../resources/directoryobject.md)、[用户](../resources/user.md)或[组织联系人](../resources/orgcontact.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d04b-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="2d04b-130">响应</span><span class="sxs-lookup"><span data-stu-id="2d04b-130">Response</span></span>

<span data-ttu-id="2d04b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d04b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d04b-133">示例</span><span class="sxs-lookup"><span data-stu-id="2d04b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d04b-134">请求</span><span class="sxs-lookup"><span data-stu-id="2d04b-134">Request</span></span>
<span data-ttu-id="2d04b-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d04b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d04b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d04b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_manager_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="2d04b-137">C#</span><span class="sxs-lookup"><span data-stu-id="2d04b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d04b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d04b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d04b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d04b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d04b-140">Java</span><span class="sxs-lookup"><span data-stu-id="2d04b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d04b-141">响应</span><span class="sxs-lookup"><span data-stu-id="2d04b-141">Response</span></span>
<span data-ttu-id="2d04b-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d04b-142">The following is an example of the response.</span></span>
><span data-ttu-id="2d04b-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2d04b-143">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
