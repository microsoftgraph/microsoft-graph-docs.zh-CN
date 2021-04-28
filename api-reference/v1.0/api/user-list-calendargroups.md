---
title: List calendarGroups
description: 获取用户的日历组。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 908406b612b97bc554815ad79928a00af7a59af9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049392"
---
# <a name="list-calendargroups"></a><span data-ttu-id="b8ae0-103">List calendarGroups</span><span class="sxs-lookup"><span data-stu-id="b8ae0-103">List calendarGroups</span></span>

<span data-ttu-id="b8ae0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8ae0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8ae0-105">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-105">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8ae0-106">权限</span><span class="sxs-lookup"><span data-stu-id="b8ae0-106">Permissions</span></span>
<span data-ttu-id="b8ae0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8ae0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8ae0-109">Permission type</span></span>      | <span data-ttu-id="b8ae0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8ae0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8ae0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ae0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b8ae0-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ae0-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b8ae0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ae0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8ae0-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ae0-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b8ae0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8ae0-115">Application</span></span> | <span data-ttu-id="b8ae0-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ae0-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8ae0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8ae0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8ae0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b8ae0-118">Optional query parameters</span></span>
<span data-ttu-id="b8ae0-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b8ae0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8ae0-120">Request headers</span></span>
| <span data-ttu-id="b8ae0-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8ae0-121">Header</span></span>       | <span data-ttu-id="b8ae0-122">值</span><span class="sxs-lookup"><span data-stu-id="b8ae0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8ae0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8ae0-123">Authorization</span></span>  | <span data-ttu-id="b8ae0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8ae0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8ae0-126">Content-Type</span></span>  | <span data-ttu-id="b8ae0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b8ae0-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8ae0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8ae0-128">Request body</span></span>
<span data-ttu-id="b8ae0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8ae0-130">响应</span><span class="sxs-lookup"><span data-stu-id="b8ae0-130">Response</span></span>

<span data-ttu-id="b8ae0-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-131">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8ae0-132">示例</span><span class="sxs-lookup"><span data-stu-id="b8ae0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8ae0-133">请求</span><span class="sxs-lookup"><span data-stu-id="b8ae0-133">Request</span></span>
<span data-ttu-id="b8ae0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8ae0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8ae0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
# <a name="c"></a>[<span data-ttu-id="b8ae0-136">C#</span><span class="sxs-lookup"><span data-stu-id="b8ae0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8ae0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8ae0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8ae0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8ae0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8ae0-139">Java</span><span class="sxs-lookup"><span data-stu-id="b8ae0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8ae0-140">响应</span><span class="sxs-lookup"><span data-stu-id="b8ae0-140">Response</span></span>
<span data-ttu-id="b8ae0-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-141">Here is an example of the response.</span></span> <span data-ttu-id="b8ae0-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8ae0-142">Note: The response object shown here might be shortened for readability.</span></span>
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
      "name": "My Calendars",
      "classId": "0006f0b7-0000-0000-c000-000000000046",
      "changeKey": "NreqLYgxdE2DpHBBId74XwAAAAAGZw==",
      "id": "AQMkADIxYjJiYgEzLTFmN_F8AAAIBBgAA_F8AAAJjIQAAAA=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
