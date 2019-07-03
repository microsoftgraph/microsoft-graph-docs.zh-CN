---
title: 指定经理
description: 使用此 API 指定用户的经理。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 033940016bc1e94fe8fe20c7cfd8a70476c859df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460110"
---
# <a name="assign-a-manager"></a><span data-ttu-id="70706-103">指定经理</span><span class="sxs-lookup"><span data-stu-id="70706-103">Assign a manager</span></span>

<span data-ttu-id="70706-104">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="70706-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="70706-105">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="70706-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="70706-106">权限</span><span class="sxs-lookup"><span data-stu-id="70706-106">Permissions</span></span>
<span data-ttu-id="70706-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70706-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70706-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70706-109">Permission type</span></span>      | <span data-ttu-id="70706-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70706-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70706-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70706-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70706-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70706-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70706-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70706-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70706-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70706-114">Not supported.</span></span>    |
|<span data-ttu-id="70706-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70706-115">Application</span></span> | <span data-ttu-id="70706-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70706-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70706-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70706-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="70706-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70706-118">Request headers</span></span>
| <span data-ttu-id="70706-119">名称</span><span class="sxs-lookup"><span data-stu-id="70706-119">Name</span></span>       | <span data-ttu-id="70706-120">类型</span><span class="sxs-lookup"><span data-stu-id="70706-120">Type</span></span> | <span data-ttu-id="70706-121">说明</span><span class="sxs-lookup"><span data-stu-id="70706-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70706-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70706-122">Authorization</span></span>  | <span data-ttu-id="70706-123">string</span><span class="sxs-lookup"><span data-stu-id="70706-123">string</span></span>  | <span data-ttu-id="70706-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70706-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70706-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70706-126">Request body</span></span>
<span data-ttu-id="70706-127">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70706-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="70706-128">响应</span><span class="sxs-lookup"><span data-stu-id="70706-128">Response</span></span>

<span data-ttu-id="70706-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="70706-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70706-131">示例</span><span class="sxs-lookup"><span data-stu-id="70706-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70706-132">请求</span><span class="sxs-lookup"><span data-stu-id="70706-132">Request</span></span>
<span data-ttu-id="70706-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70706-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70706-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="70706-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70706-135">C#</span><span class="sxs-lookup"><span data-stu-id="70706-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70706-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="70706-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70706-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="70706-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="70706-138">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70706-138">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="70706-139">响应</span><span class="sxs-lookup"><span data-stu-id="70706-139">Response</span></span>
<span data-ttu-id="70706-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70706-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
