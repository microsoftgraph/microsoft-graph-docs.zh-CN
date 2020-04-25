---
title: 删除 calendarPermission
description: 删除 calendarPermission。
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9dd829cf780af8d4720bae487296cd547c6852e9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806616"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="7c997-103">删除 calendarPermission</span><span class="sxs-lookup"><span data-stu-id="7c997-103">Delete calendarPermission</span></span>

<span data-ttu-id="7c997-104">删除 calendarPermission。</span><span class="sxs-lookup"><span data-stu-id="7c997-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c997-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="7c997-105">Permissions</span></span>

<span data-ttu-id="7c997-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c997-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c997-108">Permission type</span></span>      | <span data-ttu-id="7c997-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c997-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c997-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c997-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c997-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c997-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7c997-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c997-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c997-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c997-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7c997-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c997-114">Application</span></span> | <span data-ttu-id="7c997-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c997-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="7c997-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c997-116">HTTP request</span></span>

<span data-ttu-id="7c997-117">删除用户的主日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="7c997-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="7c997-118">删除组日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="7c997-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="7c997-119">删除包含已标识事件的用户日历的指定权限：</span><span class="sxs-lookup"><span data-stu-id="7c997-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c997-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c997-120">Request headers</span></span>

| <span data-ttu-id="7c997-121">名称</span><span class="sxs-lookup"><span data-stu-id="7c997-121">Name</span></span>          | <span data-ttu-id="7c997-122">说明</span><span class="sxs-lookup"><span data-stu-id="7c997-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7c997-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c997-123">Authorization</span></span> | <span data-ttu-id="7c997-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7c997-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c997-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c997-125">Request body</span></span>

<span data-ttu-id="7c997-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c997-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c997-127">响应</span><span class="sxs-lookup"><span data-stu-id="7c997-127">Response</span></span>

<span data-ttu-id="7c997-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c997-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c997-130">示例</span><span class="sxs-lookup"><span data-stu-id="7c997-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c997-131">请求</span><span class="sxs-lookup"><span data-stu-id="7c997-131">Request</span></span>

<span data-ttu-id="7c997-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c997-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7c997-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c997-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="7c997-134">C#</span><span class="sxs-lookup"><span data-stu-id="7c997-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c997-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c997-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c997-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c997-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c997-137">Java</span><span class="sxs-lookup"><span data-stu-id="7c997-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c997-138">响应</span><span class="sxs-lookup"><span data-stu-id="7c997-138">Response</span></span>

<span data-ttu-id="7c997-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c997-139">The following is an example of the response.</span></span>

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
