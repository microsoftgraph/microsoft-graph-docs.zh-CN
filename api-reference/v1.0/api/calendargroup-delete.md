---
title: 删除 calendarGroup
description: 删除默认日历组以外的日历组。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ac4a2f1c9ff856737be9656a2e71180c90dc428b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369120"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="32dc9-103">删除 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="32dc9-103">Delete calendarGroup</span></span>

<span data-ttu-id="32dc9-104">删除默认日历组以外的日历组。</span><span class="sxs-lookup"><span data-stu-id="32dc9-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="32dc9-105">权限</span><span class="sxs-lookup"><span data-stu-id="32dc9-105">Permissions</span></span>

<span data-ttu-id="32dc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32dc9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="32dc9-108">Permission type</span></span>                        | <span data-ttu-id="32dc9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32dc9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="32dc9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32dc9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="32dc9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dc9-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="32dc9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32dc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32dc9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dc9-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="32dc9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="32dc9-114">Application</span></span>                            | <span data-ttu-id="32dc9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dc9-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32dc9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32dc9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32dc9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="32dc9-117">Request headers</span></span>

| <span data-ttu-id="32dc9-118">名称</span><span class="sxs-lookup"><span data-stu-id="32dc9-118">Name</span></span>          | <span data-ttu-id="32dc9-119">类型</span><span class="sxs-lookup"><span data-stu-id="32dc9-119">Type</span></span>   | <span data-ttu-id="32dc9-120">说明</span><span class="sxs-lookup"><span data-stu-id="32dc9-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="32dc9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32dc9-121">Authorization</span></span> | <span data-ttu-id="32dc9-122">string</span><span class="sxs-lookup"><span data-stu-id="32dc9-122">string</span></span> | <span data-ttu-id="32dc9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32dc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32dc9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="32dc9-125">Request body</span></span>

<span data-ttu-id="32dc9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32dc9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32dc9-127">响应</span><span class="sxs-lookup"><span data-stu-id="32dc9-127">Response</span></span>

<span data-ttu-id="32dc9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="32dc9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32dc9-130">示例</span><span class="sxs-lookup"><span data-stu-id="32dc9-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="32dc9-131">请求</span><span class="sxs-lookup"><span data-stu-id="32dc9-131">Request</span></span>

<span data-ttu-id="32dc9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32dc9-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32dc9-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="32dc9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32dc9-134">C#</span><span class="sxs-lookup"><span data-stu-id="32dc9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32dc9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32dc9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32dc9-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="32dc9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32dc9-137">Java</span><span class="sxs-lookup"><span data-stu-id="32dc9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32dc9-138">响应</span><span class="sxs-lookup"><span data-stu-id="32dc9-138">Response</span></span>

<span data-ttu-id="32dc9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32dc9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
