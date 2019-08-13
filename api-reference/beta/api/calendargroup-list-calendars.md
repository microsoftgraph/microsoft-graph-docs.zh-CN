---
title: 列出日历
description: 检索属于日历组的日历列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fcb30ab9c563197635be04995b92f540d0f8a514
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317826"
---
# <a name="list-calendars"></a><span data-ttu-id="f55bc-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="f55bc-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f55bc-104">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="f55bc-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f55bc-105">权限</span><span class="sxs-lookup"><span data-stu-id="f55bc-105">Permissions</span></span>

<span data-ttu-id="f55bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f55bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f55bc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f55bc-108">Permission type</span></span>                        | <span data-ttu-id="f55bc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f55bc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f55bc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f55bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f55bc-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f55bc-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="f55bc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f55bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f55bc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f55bc-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="f55bc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f55bc-114">Application</span></span>                            | <span data-ttu-id="f55bc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f55bc-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f55bc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f55bc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f55bc-117">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="f55bc-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="f55bc-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="f55bc-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f55bc-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f55bc-119">Optional query parameters</span></span>

<span data-ttu-id="f55bc-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f55bc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f55bc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f55bc-121">Request headers</span></span>

| <span data-ttu-id="f55bc-122">名称</span><span class="sxs-lookup"><span data-stu-id="f55bc-122">Name</span></span>          | <span data-ttu-id="f55bc-123">类型</span><span class="sxs-lookup"><span data-stu-id="f55bc-123">Type</span></span>   | <span data-ttu-id="f55bc-124">说明</span><span class="sxs-lookup"><span data-stu-id="f55bc-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f55bc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f55bc-125">Authorization</span></span> | <span data-ttu-id="f55bc-126">string</span><span class="sxs-lookup"><span data-stu-id="f55bc-126">string</span></span> | <span data-ttu-id="f55bc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f55bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f55bc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f55bc-129">Request body</span></span>

<span data-ttu-id="f55bc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f55bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f55bc-131">响应</span><span class="sxs-lookup"><span data-stu-id="f55bc-131">Response</span></span>

<span data-ttu-id="f55bc-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f55bc-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f55bc-133">示例</span><span class="sxs-lookup"><span data-stu-id="f55bc-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f55bc-134">请求</span><span class="sxs-lookup"><span data-stu-id="f55bc-134">Request</span></span>

<span data-ttu-id="f55bc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f55bc-135">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f55bc-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f55bc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendargroup_get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f55bc-137">C#</span><span class="sxs-lookup"><span data-stu-id="f55bc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendargroup-get-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f55bc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f55bc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendargroup-get-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f55bc-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="f55bc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendargroup-get-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f55bc-140">Java</span><span class="sxs-lookup"><span data-stu-id="f55bc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendargroup-get-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f55bc-141">响应</span><span class="sxs-lookup"><span data-stu-id="f55bc-141">Response</span></span>

<span data-ttu-id="f55bc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f55bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
