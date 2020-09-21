---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bee626f15477984771295d3e3c51d2b1fc9b4877
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070275"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="2d8f8-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2d8f8-103">Delete calendarGroup</span></span>

<span data-ttu-id="2d8f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d8f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d8f8-105">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-105">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d8f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d8f8-106">Permissions</span></span>

<span data-ttu-id="2d8f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d8f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d8f8-109">Permission type</span></span>                        | <span data-ttu-id="2d8f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d8f8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2d8f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d8f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d8f8-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8f8-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2d8f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d8f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d8f8-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8f8-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2d8f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d8f8-115">Application</span></span>                            | <span data-ttu-id="2d8f8-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8f8-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2d8f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d8f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2d8f8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d8f8-118">Request headers</span></span>

| <span data-ttu-id="2d8f8-119">名称</span><span class="sxs-lookup"><span data-stu-id="2d8f8-119">Name</span></span>          | <span data-ttu-id="2d8f8-120">类型</span><span class="sxs-lookup"><span data-stu-id="2d8f8-120">Type</span></span>   | <span data-ttu-id="2d8f8-121">说明</span><span class="sxs-lookup"><span data-stu-id="2d8f8-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2d8f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d8f8-122">Authorization</span></span> | <span data-ttu-id="2d8f8-123">string</span><span class="sxs-lookup"><span data-stu-id="2d8f8-123">string</span></span> | <span data-ttu-id="2d8f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d8f8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d8f8-126">Request body</span></span>

<span data-ttu-id="2d8f8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d8f8-128">响应</span><span class="sxs-lookup"><span data-stu-id="2d8f8-128">Response</span></span>

<span data-ttu-id="2d8f8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d8f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="2d8f8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2d8f8-132">请求</span><span class="sxs-lookup"><span data-stu-id="2d8f8-132">Request</span></span>

<span data-ttu-id="2d8f8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d8f8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d8f8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="2d8f8-135">C#</span><span class="sxs-lookup"><span data-stu-id="2d8f8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d8f8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d8f8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d8f8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d8f8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d8f8-138">Java</span><span class="sxs-lookup"><span data-stu-id="2d8f8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d8f8-139">响应</span><span class="sxs-lookup"><span data-stu-id="2d8f8-139">Response</span></span>

<span data-ttu-id="2d8f8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d8f8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

