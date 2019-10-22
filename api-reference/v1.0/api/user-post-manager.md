---
title: 分配管理器
description: 分配用户的经理。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36b24ef7b6e9fb7a35be3c87723b650581ec982c
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621446"
---
# <a name="assign-manager"></a><span data-ttu-id="c07cf-103">分配管理器</span><span class="sxs-lookup"><span data-stu-id="c07cf-103">Assign manager</span></span>

<span data-ttu-id="c07cf-104">分配用户的经理。</span><span class="sxs-lookup"><span data-stu-id="c07cf-104">Assign a user's manager.</span></span>
> [!NOTE]
> <span data-ttu-id="c07cf-105">您不能分配直接下属，也不能分配。而是使用此 API。</span><span class="sxs-lookup"><span data-stu-id="c07cf-105">You cannot assign direct reports; instead, use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c07cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="c07cf-106">Permissions</span></span>
<span data-ttu-id="c07cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c07cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c07cf-109">Permission type</span></span>      | <span data-ttu-id="c07cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c07cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c07cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c07cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c07cf-112">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c07cf-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c07cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c07cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c07cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c07cf-114">Not supported.</span></span>    |
|<span data-ttu-id="c07cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c07cf-115">Application</span></span> | <span data-ttu-id="c07cf-116">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07cf-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c07cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c07cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c07cf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c07cf-118">Request headers</span></span>
| <span data-ttu-id="c07cf-119">标头</span><span class="sxs-lookup"><span data-stu-id="c07cf-119">Header</span></span>       | <span data-ttu-id="c07cf-120">值</span><span class="sxs-lookup"><span data-stu-id="c07cf-120">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c07cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c07cf-121">Authorization</span></span>  | <span data-ttu-id="c07cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c07cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c07cf-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c07cf-124">Content-type</span></span>   | <span data-ttu-id="c07cf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c07cf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07cf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c07cf-127">Request body</span></span>
<span data-ttu-id="c07cf-128">在请求正文中，提供要添加的[directoryObject](../resources/directoryobject.md)、[用户](../resources/user.md)或[组织联系人](../resources/orgcontact.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c07cf-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c07cf-129">响应</span><span class="sxs-lookup"><span data-stu-id="c07cf-129">Response</span></span>

<span data-ttu-id="c07cf-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c07cf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c07cf-132">示例</span><span class="sxs-lookup"><span data-stu-id="c07cf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c07cf-133">请求</span><span class="sxs-lookup"><span data-stu-id="c07cf-133">Request</span></span>
<span data-ttu-id="c07cf-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c07cf-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c07cf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c07cf-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c07cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="c07cf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-manager-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c07cf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c07cf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-manager-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c07cf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c07cf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-manager-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c07cf-139">Java</span><span class="sxs-lookup"><span data-stu-id="c07cf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-manager-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c07cf-140">响应</span><span class="sxs-lookup"><span data-stu-id="c07cf-140">Response</span></span>
<span data-ttu-id="c07cf-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c07cf-141">The following is an example of the response.</span></span>
><span data-ttu-id="c07cf-142">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c07cf-142">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
