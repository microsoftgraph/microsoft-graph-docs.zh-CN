---
title: 列出日历
description: 检索属于日历组的日历列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5e1ca56fdeb2f1087a6c6902ee387220e6966602
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510062"
---
# <a name="list-calendars"></a><span data-ttu-id="75caf-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="75caf-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75caf-104">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="75caf-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="75caf-105">权限</span><span class="sxs-lookup"><span data-stu-id="75caf-105">Permissions</span></span>

<span data-ttu-id="75caf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75caf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="75caf-108">Permission type</span></span>                        | <span data-ttu-id="75caf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75caf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="75caf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75caf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="75caf-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75caf-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="75caf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75caf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75caf-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75caf-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="75caf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="75caf-114">Application</span></span>                            | <span data-ttu-id="75caf-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75caf-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="75caf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75caf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="75caf-117">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="75caf-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="75caf-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="75caf-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75caf-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75caf-119">Optional query parameters</span></span>

<span data-ttu-id="75caf-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75caf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75caf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="75caf-121">Request headers</span></span>

| <span data-ttu-id="75caf-122">名称</span><span class="sxs-lookup"><span data-stu-id="75caf-122">Name</span></span>          | <span data-ttu-id="75caf-123">类型</span><span class="sxs-lookup"><span data-stu-id="75caf-123">Type</span></span>   | <span data-ttu-id="75caf-124">说明</span><span class="sxs-lookup"><span data-stu-id="75caf-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="75caf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75caf-125">Authorization</span></span> | <span data-ttu-id="75caf-126">string</span><span class="sxs-lookup"><span data-stu-id="75caf-126">string</span></span> | <span data-ttu-id="75caf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75caf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75caf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="75caf-129">Request body</span></span>

<span data-ttu-id="75caf-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75caf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75caf-131">响应</span><span class="sxs-lookup"><span data-stu-id="75caf-131">Response</span></span>

<span data-ttu-id="75caf-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="75caf-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75caf-133">示例</span><span class="sxs-lookup"><span data-stu-id="75caf-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75caf-134">请求</span><span class="sxs-lookup"><span data-stu-id="75caf-134">Request</span></span>

<span data-ttu-id="75caf-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75caf-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="75caf-136">响应</span><span class="sxs-lookup"><span data-stu-id="75caf-136">Response</span></span>

<span data-ttu-id="75caf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75caf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/calendargroup-list-calendars.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
