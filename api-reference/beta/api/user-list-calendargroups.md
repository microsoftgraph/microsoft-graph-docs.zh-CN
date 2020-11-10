---
title: List calendarGroups
description: 获取用户的日历组。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2fd3a38fe2bcc0fef706f3d7d2f428fda7d8a992
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979410"
---
# <a name="list-calendargroups"></a><span data-ttu-id="6b5da-103">List calendarGroups</span><span class="sxs-lookup"><span data-stu-id="6b5da-103">List calendarGroups</span></span>

<span data-ttu-id="6b5da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b5da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b5da-105">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="6b5da-105">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b5da-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b5da-106">Permissions</span></span>
<span data-ttu-id="6b5da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b5da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b5da-109">Permission type</span></span>      | <span data-ttu-id="6b5da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b5da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b5da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b5da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b5da-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b5da-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6b5da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b5da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b5da-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b5da-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6b5da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b5da-115">Application</span></span> | <span data-ttu-id="6b5da-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b5da-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b5da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b5da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b5da-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6b5da-118">Optional query parameters</span></span>
<span data-ttu-id="6b5da-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b5da-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6b5da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b5da-120">Request headers</span></span>
| <span data-ttu-id="6b5da-121">标头</span><span class="sxs-lookup"><span data-stu-id="6b5da-121">Header</span></span>       | <span data-ttu-id="6b5da-122">值</span><span class="sxs-lookup"><span data-stu-id="6b5da-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b5da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b5da-123">Authorization</span></span>  | <span data-ttu-id="6b5da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b5da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b5da-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b5da-126">Content-Type</span></span>  | <span data-ttu-id="6b5da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6b5da-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b5da-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b5da-128">Request body</span></span>
<span data-ttu-id="6b5da-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b5da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b5da-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b5da-130">Response</span></span>

<span data-ttu-id="6b5da-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6b5da-131">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b5da-132">示例</span><span class="sxs-lookup"><span data-stu-id="6b5da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b5da-133">请求</span><span class="sxs-lookup"><span data-stu-id="6b5da-133">Request</span></span>
<span data-ttu-id="6b5da-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b5da-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b5da-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5da-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups
```
# <a name="c"></a>[<span data-ttu-id="6b5da-136">C#</span><span class="sxs-lookup"><span data-stu-id="6b5da-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b5da-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b5da-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b5da-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b5da-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b5da-139">Java</span><span class="sxs-lookup"><span data-stu-id="6b5da-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b5da-140">响应</span><span class="sxs-lookup"><span data-stu-id="6b5da-140">Response</span></span>
<span data-ttu-id="6b5da-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b5da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
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
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
