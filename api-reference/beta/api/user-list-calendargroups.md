---
title: List calendarGroups
description: 获取用户的日历组。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 706bb810b0dcd9615443c477437350a020166be5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544276"
---
# <a name="list-calendargroups"></a><span data-ttu-id="236aa-103">List calendarGroups</span><span class="sxs-lookup"><span data-stu-id="236aa-103">List calendarGroups</span></span>

<span data-ttu-id="236aa-104">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="236aa-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="236aa-105">权限</span><span class="sxs-lookup"><span data-stu-id="236aa-105">Permissions</span></span>
<span data-ttu-id="236aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="236aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="236aa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="236aa-108">Permission type</span></span>      | <span data-ttu-id="236aa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="236aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="236aa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="236aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="236aa-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="236aa-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="236aa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="236aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="236aa-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="236aa-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="236aa-114">Application</span><span class="sxs-lookup"><span data-stu-id="236aa-114">Application</span></span> | <span data-ttu-id="236aa-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="236aa-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="236aa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="236aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="236aa-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="236aa-117">Optional query parameters</span></span>
<span data-ttu-id="236aa-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="236aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="236aa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="236aa-119">Request headers</span></span>
| <span data-ttu-id="236aa-120">标头</span><span class="sxs-lookup"><span data-stu-id="236aa-120">Header</span></span>       | <span data-ttu-id="236aa-121">值</span><span class="sxs-lookup"><span data-stu-id="236aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="236aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="236aa-122">Authorization</span></span>  | <span data-ttu-id="236aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="236aa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="236aa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="236aa-125">Content-Type</span></span>  | <span data-ttu-id="236aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="236aa-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="236aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="236aa-127">Request body</span></span>
<span data-ttu-id="236aa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="236aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="236aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="236aa-129">Response</span></span>

<span data-ttu-id="236aa-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="236aa-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="236aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="236aa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="236aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="236aa-132">Request</span></span>
<span data-ttu-id="236aa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="236aa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="236aa-134">响应</span><span class="sxs-lookup"><span data-stu-id="236aa-134">Response</span></span>
<span data-ttu-id="236aa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="236aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
