---
title: 列出 calendarGroups
description: 获取用户的日历组。
ms.openlocfilehash: 560dd09d42b59e68b6282d7dec4305f7b10ea9f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049375"
---
# <a name="list-calendargroups"></a><span data-ttu-id="f8fe3-103">列出 calendarGroups</span><span class="sxs-lookup"><span data-stu-id="f8fe3-103">List calendarGroups</span></span>

> <span data-ttu-id="f8fe3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8fe3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8fe3-106">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-106">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8fe3-107">权限</span><span class="sxs-lookup"><span data-stu-id="f8fe3-107">Permissions</span></span>
<span data-ttu-id="f8fe3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8fe3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8fe3-110">Permission type</span></span>      | <span data-ttu-id="f8fe3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8fe3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8fe3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8fe3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f8fe3-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8fe3-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8fe3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8fe3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8fe3-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8fe3-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8fe3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8fe3-116">Application</span></span> | <span data-ttu-id="f8fe3-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8fe3-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8fe3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8fe3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8fe3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8fe3-119">Optional query parameters</span></span>
<span data-ttu-id="f8fe3-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8fe3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8fe3-121">Request headers</span></span>
| <span data-ttu-id="f8fe3-122">标头</span><span class="sxs-lookup"><span data-stu-id="f8fe3-122">Header</span></span>       | <span data-ttu-id="f8fe3-123">值</span><span class="sxs-lookup"><span data-stu-id="f8fe3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8fe3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8fe3-124">Authorization</span></span>  | <span data-ttu-id="f8fe3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f8fe3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8fe3-127">Content-Type</span></span>  | <span data-ttu-id="f8fe3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f8fe3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8fe3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8fe3-129">Request body</span></span>
<span data-ttu-id="f8fe3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8fe3-131">响应</span><span class="sxs-lookup"><span data-stu-id="f8fe3-131">Response</span></span>

<span data-ttu-id="f8fe3-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [CalendarGroup](../resources/calendargroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-132">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8fe3-133">示例</span><span class="sxs-lookup"><span data-stu-id="f8fe3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8fe3-134">请求</span><span class="sxs-lookup"><span data-stu-id="f8fe3-134">Request</span></span>
<span data-ttu-id="f8fe3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="f8fe3-136">响应</span><span class="sxs-lookup"><span data-stu-id="f8fe3-136">Response</span></span>
<span data-ttu-id="f8fe3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8fe3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
