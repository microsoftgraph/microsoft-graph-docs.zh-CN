---
title: 列出日历
description: 检索属于日历组的日历列表。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13b3899b1631230798a0324f29e573dc0e6ac829
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987573"
---
# <a name="list-calendars"></a><span data-ttu-id="eddae-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="eddae-103">List calendars</span></span>

<span data-ttu-id="eddae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eddae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eddae-105">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="eddae-105">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="eddae-106">权限</span><span class="sxs-lookup"><span data-stu-id="eddae-106">Permissions</span></span>

<span data-ttu-id="eddae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eddae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eddae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eddae-109">Permission type</span></span>                        | <span data-ttu-id="eddae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eddae-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="eddae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eddae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eddae-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eddae-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="eddae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eddae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eddae-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eddae-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="eddae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eddae-115">Application</span></span>                            | <span data-ttu-id="eddae-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eddae-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="eddae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eddae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="eddae-118">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="eddae-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="eddae-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="eddae-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eddae-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eddae-120">Optional query parameters</span></span>

<span data-ttu-id="eddae-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eddae-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eddae-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="eddae-122">Request headers</span></span>

| <span data-ttu-id="eddae-123">名称</span><span class="sxs-lookup"><span data-stu-id="eddae-123">Name</span></span>          | <span data-ttu-id="eddae-124">类型</span><span class="sxs-lookup"><span data-stu-id="eddae-124">Type</span></span>   | <span data-ttu-id="eddae-125">说明</span><span class="sxs-lookup"><span data-stu-id="eddae-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="eddae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="eddae-126">Authorization</span></span> | <span data-ttu-id="eddae-127">string</span><span class="sxs-lookup"><span data-stu-id="eddae-127">string</span></span> | <span data-ttu-id="eddae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eddae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eddae-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="eddae-130">Request body</span></span>

<span data-ttu-id="eddae-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eddae-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eddae-132">响应</span><span class="sxs-lookup"><span data-stu-id="eddae-132">Response</span></span>

<span data-ttu-id="eddae-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eddae-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eddae-134">示例</span><span class="sxs-lookup"><span data-stu-id="eddae-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eddae-135">请求</span><span class="sxs-lookup"><span data-stu-id="eddae-135">Request</span></span>

<span data-ttu-id="eddae-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eddae-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eddae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="eddae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="c"></a>[<span data-ttu-id="eddae-138">C#</span><span class="sxs-lookup"><span data-stu-id="eddae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eddae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eddae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eddae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eddae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eddae-141">响应</span><span class="sxs-lookup"><span data-stu-id="eddae-141">Response</span></span>

<span data-ttu-id="eddae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eddae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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


