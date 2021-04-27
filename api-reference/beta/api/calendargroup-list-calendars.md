---
title: 列出日历
description: 检索属于日历组的日历列表。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1dc7c556f304b15935f2c1ec14c16d035dfdf64
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047705"
---
# <a name="list-calendars"></a><span data-ttu-id="53837-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="53837-103">List calendars</span></span>

<span data-ttu-id="53837-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53837-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53837-105">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="53837-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="53837-106">权限</span><span class="sxs-lookup"><span data-stu-id="53837-106">Permissions</span></span>

<span data-ttu-id="53837-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53837-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53837-109">Permission type</span></span>                        | <span data-ttu-id="53837-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53837-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="53837-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53837-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53837-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53837-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="53837-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53837-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53837-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53837-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="53837-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53837-115">Application</span></span>                            | <span data-ttu-id="53837-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="53837-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="53837-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53837-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="53837-118">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="53837-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="53837-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="53837-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53837-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53837-120">Optional query parameters</span></span>

<span data-ttu-id="53837-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53837-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53837-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="53837-122">Request headers</span></span>

| <span data-ttu-id="53837-123">名称</span><span class="sxs-lookup"><span data-stu-id="53837-123">Name</span></span>          | <span data-ttu-id="53837-124">类型</span><span class="sxs-lookup"><span data-stu-id="53837-124">Type</span></span>   | <span data-ttu-id="53837-125">说明</span><span class="sxs-lookup"><span data-stu-id="53837-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="53837-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="53837-126">Authorization</span></span> | <span data-ttu-id="53837-127">string</span><span class="sxs-lookup"><span data-stu-id="53837-127">string</span></span> | <span data-ttu-id="53837-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53837-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53837-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="53837-130">Request body</span></span>

<span data-ttu-id="53837-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53837-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53837-132">响应</span><span class="sxs-lookup"><span data-stu-id="53837-132">Response</span></span>

<span data-ttu-id="53837-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53837-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53837-134">示例</span><span class="sxs-lookup"><span data-stu-id="53837-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="53837-135">请求</span><span class="sxs-lookup"><span data-stu-id="53837-135">Request</span></span>

<span data-ttu-id="53837-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53837-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53837-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="53837-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="53837-138">C#</span><span class="sxs-lookup"><span data-stu-id="53837-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53837-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53837-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53837-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53837-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53837-141">Java</span><span class="sxs-lookup"><span data-stu-id="53837-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53837-142">响应</span><span class="sxs-lookup"><span data-stu-id="53837-142">Response</span></span>

<span data-ttu-id="53837-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53837-143">Here is an example of the response.</span></span> <span data-ttu-id="53837-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53837-144">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "calendarGroupId":"calendarGroupId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"      
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
