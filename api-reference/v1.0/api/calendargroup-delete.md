---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 88d8c4d82eb5dfc71eaf2fbc189b514d8d097e0f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052507"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="16432-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="16432-103">Delete calendarGroup</span></span>

<span data-ttu-id="16432-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16432-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16432-105">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="16432-105">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="16432-106">权限</span><span class="sxs-lookup"><span data-stu-id="16432-106">Permissions</span></span>

<span data-ttu-id="16432-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16432-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16432-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16432-109">Permission type</span></span>                        | <span data-ttu-id="16432-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16432-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="16432-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16432-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16432-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16432-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="16432-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16432-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16432-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16432-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="16432-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="16432-115">Application</span></span>                            | <span data-ttu-id="16432-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16432-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="16432-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16432-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16432-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="16432-118">Request headers</span></span>

| <span data-ttu-id="16432-119">名称</span><span class="sxs-lookup"><span data-stu-id="16432-119">Name</span></span>          | <span data-ttu-id="16432-120">类型</span><span class="sxs-lookup"><span data-stu-id="16432-120">Type</span></span>   | <span data-ttu-id="16432-121">说明</span><span class="sxs-lookup"><span data-stu-id="16432-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="16432-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16432-122">Authorization</span></span> | <span data-ttu-id="16432-123">string</span><span class="sxs-lookup"><span data-stu-id="16432-123">string</span></span> | <span data-ttu-id="16432-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16432-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16432-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16432-126">Request body</span></span>

<span data-ttu-id="16432-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16432-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16432-128">响应</span><span class="sxs-lookup"><span data-stu-id="16432-128">Response</span></span>

<span data-ttu-id="16432-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="16432-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16432-131">示例</span><span class="sxs-lookup"><span data-stu-id="16432-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16432-132">请求</span><span class="sxs-lookup"><span data-stu-id="16432-132">Request</span></span>

<span data-ttu-id="16432-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16432-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16432-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="16432-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="16432-135">C#</span><span class="sxs-lookup"><span data-stu-id="16432-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16432-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16432-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16432-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16432-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16432-138">Java</span><span class="sxs-lookup"><span data-stu-id="16432-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="16432-139">响应</span><span class="sxs-lookup"><span data-stu-id="16432-139">Response</span></span>

<span data-ttu-id="16432-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16432-140">Here is an example of the response.</span></span> <span data-ttu-id="16432-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16432-141">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

