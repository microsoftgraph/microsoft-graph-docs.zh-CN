---
title: 获取 calendarGroup
description: 检索日历组对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 993de8179ffaaf4e4ea0ed08ea1c3cef755ca1db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922380"
---
# <a name="get-calendargroup"></a><span data-ttu-id="ca46b-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ca46b-103">Get calendarGroup</span></span>

> <span data-ttu-id="ca46b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca46b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca46b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca46b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca46b-106">检索日历组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca46b-106">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca46b-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca46b-107">Permissions</span></span>

<span data-ttu-id="ca46b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca46b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca46b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca46b-110">Permission type</span></span>                        | <span data-ttu-id="ca46b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca46b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ca46b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca46b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca46b-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca46b-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="ca46b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca46b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca46b-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca46b-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="ca46b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca46b-116">Application</span></span>                            | <span data-ttu-id="ca46b-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ca46b-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="ca46b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca46b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ca46b-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="ca46b-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca46b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca46b-120">Optional query parameters</span></span>

<span data-ttu-id="ca46b-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca46b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca46b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca46b-122">Request headers</span></span>

| <span data-ttu-id="ca46b-123">名称</span><span class="sxs-lookup"><span data-stu-id="ca46b-123">Name</span></span>          | <span data-ttu-id="ca46b-124">类型</span><span class="sxs-lookup"><span data-stu-id="ca46b-124">Type</span></span>   | <span data-ttu-id="ca46b-125">说明</span><span class="sxs-lookup"><span data-stu-id="ca46b-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="ca46b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca46b-126">Authorization</span></span> | <span data-ttu-id="ca46b-127">string</span><span class="sxs-lookup"><span data-stu-id="ca46b-127">string</span></span> | <span data-ttu-id="ca46b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca46b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca46b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca46b-130">Request body</span></span>

<span data-ttu-id="ca46b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca46b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca46b-132">响应</span><span class="sxs-lookup"><span data-stu-id="ca46b-132">Response</span></span>

<span data-ttu-id="ca46b-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca46b-133">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca46b-134">示例</span><span class="sxs-lookup"><span data-stu-id="ca46b-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca46b-135">请求</span><span class="sxs-lookup"><span data-stu-id="ca46b-135">Request</span></span>

<span data-ttu-id="ca46b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca46b-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="ca46b-137">响应</span><span class="sxs-lookup"><span data-stu-id="ca46b-137">Response</span></span>

<span data-ttu-id="ca46b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca46b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
