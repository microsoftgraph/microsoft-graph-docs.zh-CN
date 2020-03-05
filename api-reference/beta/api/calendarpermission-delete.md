---
title: 删除 calendarPermission
description: 删除 calendarPermission。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 662efaae4fade948b88d716af664ce157705fef6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440911"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="b0ee1-103">删除 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b0ee1-103">Delete calendarPermission</span></span>

<span data-ttu-id="b0ee1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b0ee1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0ee1-105">删除 calendarPermission。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-105">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0ee1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0ee1-106">Permissions</span></span>

<span data-ttu-id="b0ee1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0ee1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0ee1-109">Permission type</span></span>      | <span data-ttu-id="b0ee1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0ee1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ee1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0ee1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ee1-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ee1-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b0ee1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0ee1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ee1-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ee1-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b0ee1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0ee1-115">Application</span></span> | <span data-ttu-id="b0ee1-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ee1-116">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="b0ee1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0ee1-117">HTTP request</span></span>

<span data-ttu-id="b0ee1-118">删除用户的主日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b0ee1-118">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b0ee1-119">删除组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b0ee1-119">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b0ee1-120">删除包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="b0ee1-120">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0ee1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0ee1-121">Request headers</span></span>

| <span data-ttu-id="b0ee1-122">名称</span><span class="sxs-lookup"><span data-stu-id="b0ee1-122">Name</span></span>          | <span data-ttu-id="b0ee1-123">说明</span><span class="sxs-lookup"><span data-stu-id="b0ee1-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b0ee1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0ee1-124">Authorization</span></span> | <span data-ttu-id="b0ee1-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b0ee1-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0ee1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0ee1-126">Request body</span></span>

<span data-ttu-id="b0ee1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0ee1-128">响应</span><span class="sxs-lookup"><span data-stu-id="b0ee1-128">Response</span></span>

<span data-ttu-id="b0ee1-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0ee1-131">示例</span><span class="sxs-lookup"><span data-stu-id="b0ee1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0ee1-132">请求</span><span class="sxs-lookup"><span data-stu-id="b0ee1-132">Request</span></span>

<span data-ttu-id="b0ee1-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0ee1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0ee1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b0ee1-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0ee1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0ee1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0ee1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0ee1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0ee1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0ee1-138">响应</span><span class="sxs-lookup"><span data-stu-id="b0ee1-138">Response</span></span>

<span data-ttu-id="b0ee1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b0ee1-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
