---
title: 列出日历
description: 检索属于日历组的日历列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d8d54b1dd3f8a1f75a3f4e4ab3449cb4fc8a8283
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322395"
---
# <a name="list-calendars"></a><span data-ttu-id="74f41-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="74f41-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74f41-104">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="74f41-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="74f41-105">权限</span><span class="sxs-lookup"><span data-stu-id="74f41-105">Permissions</span></span>

<span data-ttu-id="74f41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74f41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74f41-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="74f41-108">Permission type</span></span>                        | <span data-ttu-id="74f41-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74f41-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="74f41-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74f41-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="74f41-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74f41-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="74f41-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74f41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74f41-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74f41-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="74f41-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="74f41-114">Application</span></span>                            | <span data-ttu-id="74f41-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74f41-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="74f41-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74f41-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="74f41-117">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="74f41-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="74f41-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="74f41-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74f41-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74f41-119">Optional query parameters</span></span>

<span data-ttu-id="74f41-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="74f41-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74f41-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="74f41-121">Request headers</span></span>

| <span data-ttu-id="74f41-122">名称</span><span class="sxs-lookup"><span data-stu-id="74f41-122">Name</span></span>          | <span data-ttu-id="74f41-123">类型</span><span class="sxs-lookup"><span data-stu-id="74f41-123">Type</span></span>   | <span data-ttu-id="74f41-124">说明</span><span class="sxs-lookup"><span data-stu-id="74f41-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="74f41-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="74f41-125">Authorization</span></span> | <span data-ttu-id="74f41-126">string</span><span class="sxs-lookup"><span data-stu-id="74f41-126">string</span></span> | <span data-ttu-id="74f41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74f41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74f41-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="74f41-129">Request body</span></span>

<span data-ttu-id="74f41-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74f41-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74f41-131">响应</span><span class="sxs-lookup"><span data-stu-id="74f41-131">Response</span></span>

<span data-ttu-id="74f41-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="74f41-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f41-133">示例</span><span class="sxs-lookup"><span data-stu-id="74f41-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="74f41-134">请求</span><span class="sxs-lookup"><span data-stu-id="74f41-134">Request</span></span>

<span data-ttu-id="74f41-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74f41-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="74f41-136">响应</span><span class="sxs-lookup"><span data-stu-id="74f41-136">Response</span></span>

<span data-ttu-id="74f41-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74f41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
