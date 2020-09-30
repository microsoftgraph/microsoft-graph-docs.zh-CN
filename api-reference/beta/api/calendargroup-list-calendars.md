---
title: 列出日历
description: 检索属于日历组的日历列表。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 998dcfca1930ecea3525b4867cc77ff821d20574
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313105"
---
# <a name="list-calendars"></a><span data-ttu-id="5136a-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="5136a-103">List calendars</span></span>

<span data-ttu-id="5136a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5136a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5136a-105">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="5136a-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="5136a-106">权限</span><span class="sxs-lookup"><span data-stu-id="5136a-106">Permissions</span></span>

<span data-ttu-id="5136a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5136a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5136a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5136a-109">Permission type</span></span>                        | <span data-ttu-id="5136a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5136a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5136a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5136a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5136a-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5136a-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="5136a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5136a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5136a-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5136a-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="5136a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5136a-115">Application</span></span>                            | <span data-ttu-id="5136a-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5136a-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="5136a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5136a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5136a-118">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="5136a-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="5136a-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="5136a-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5136a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5136a-120">Optional query parameters</span></span>

<span data-ttu-id="5136a-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5136a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5136a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5136a-122">Request headers</span></span>

| <span data-ttu-id="5136a-123">名称</span><span class="sxs-lookup"><span data-stu-id="5136a-123">Name</span></span>          | <span data-ttu-id="5136a-124">类型</span><span class="sxs-lookup"><span data-stu-id="5136a-124">Type</span></span>   | <span data-ttu-id="5136a-125">说明</span><span class="sxs-lookup"><span data-stu-id="5136a-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="5136a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5136a-126">Authorization</span></span> | <span data-ttu-id="5136a-127">string</span><span class="sxs-lookup"><span data-stu-id="5136a-127">string</span></span> | <span data-ttu-id="5136a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5136a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5136a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5136a-130">Request body</span></span>

<span data-ttu-id="5136a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5136a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5136a-132">响应</span><span class="sxs-lookup"><span data-stu-id="5136a-132">Response</span></span>

<span data-ttu-id="5136a-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5136a-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5136a-134">示例</span><span class="sxs-lookup"><span data-stu-id="5136a-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5136a-135">请求</span><span class="sxs-lookup"><span data-stu-id="5136a-135">Request</span></span>

<span data-ttu-id="5136a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5136a-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5136a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5136a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="5136a-138">C#</span><span class="sxs-lookup"><span data-stu-id="5136a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5136a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5136a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5136a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5136a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5136a-141">响应</span><span class="sxs-lookup"><span data-stu-id="5136a-141">Response</span></span>

<span data-ttu-id="5136a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5136a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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