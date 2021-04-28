---
title: 获取 calendarGroup
description: 检索 calendargroup 对象的属性和关系。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d486f1c03bf0d0aa86ab97d2c694a1313098a9dd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039963"
---
# <a name="get-calendargroup"></a><span data-ttu-id="55938-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="55938-103">Get calendarGroup</span></span>

<span data-ttu-id="55938-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55938-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55938-105">检索 calendargroup 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55938-105">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55938-106">权限</span><span class="sxs-lookup"><span data-stu-id="55938-106">Permissions</span></span>

<span data-ttu-id="55938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55938-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55938-109">Permission type</span></span>                        | <span data-ttu-id="55938-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55938-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="55938-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55938-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55938-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55938-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="55938-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55938-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55938-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55938-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="55938-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="55938-115">Application</span></span>                            | <span data-ttu-id="55938-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55938-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="55938-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55938-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="55938-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="55938-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55938-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="55938-119">Optional query parameters</span></span>

<span data-ttu-id="55938-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="55938-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55938-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="55938-121">Request headers</span></span>

| <span data-ttu-id="55938-122">名称</span><span class="sxs-lookup"><span data-stu-id="55938-122">Name</span></span>          | <span data-ttu-id="55938-123">类型</span><span class="sxs-lookup"><span data-stu-id="55938-123">Type</span></span>   | <span data-ttu-id="55938-124">说明</span><span class="sxs-lookup"><span data-stu-id="55938-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="55938-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="55938-125">Authorization</span></span> | <span data-ttu-id="55938-126">string</span><span class="sxs-lookup"><span data-stu-id="55938-126">string</span></span> | <span data-ttu-id="55938-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55938-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55938-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="55938-129">Request body</span></span>

<span data-ttu-id="55938-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55938-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55938-131">响应</span><span class="sxs-lookup"><span data-stu-id="55938-131">Response</span></span>

<span data-ttu-id="55938-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55938-132">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55938-133">示例</span><span class="sxs-lookup"><span data-stu-id="55938-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="55938-134">请求</span><span class="sxs-lookup"><span data-stu-id="55938-134">Request</span></span>

<span data-ttu-id="55938-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55938-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55938-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="55938-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="55938-137">C#</span><span class="sxs-lookup"><span data-stu-id="55938-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55938-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55938-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55938-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55938-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55938-140">Java</span><span class="sxs-lookup"><span data-stu-id="55938-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55938-141">响应</span><span class="sxs-lookup"><span data-stu-id="55938-141">Response</span></span>

<span data-ttu-id="55938-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55938-142">Here is an example of the response.</span></span> <span data-ttu-id="55938-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55938-143">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
