---
title: 获取 calendarGroup
description: 检索日历组对象的属性和关系。
author: angelgolfer-ms
ms.openlocfilehash: fce49730733537b14eff145a6f6acd9fe4d82485
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358315"
---
# <a name="get-calendargroup"></a><span data-ttu-id="09ddb-103">获取 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="09ddb-103">Get calendarGroup</span></span>

<span data-ttu-id="09ddb-104">检索日历组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09ddb-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ddb-105">权限</span><span class="sxs-lookup"><span data-stu-id="09ddb-105">Permissions</span></span>

<span data-ttu-id="09ddb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09ddb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="09ddb-108">Permission type</span></span>                        | <span data-ttu-id="09ddb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09ddb-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="09ddb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09ddb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09ddb-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09ddb-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="09ddb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09ddb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ddb-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09ddb-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="09ddb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="09ddb-114">Application</span></span>                            | <span data-ttu-id="09ddb-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="09ddb-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="09ddb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09ddb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="09ddb-117">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="09ddb-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09ddb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09ddb-118">Optional query parameters</span></span>

<span data-ttu-id="09ddb-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09ddb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09ddb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="09ddb-120">Request headers</span></span>

| <span data-ttu-id="09ddb-121">Name</span><span class="sxs-lookup"><span data-stu-id="09ddb-121">Name</span></span>          | <span data-ttu-id="09ddb-122">类型</span><span class="sxs-lookup"><span data-stu-id="09ddb-122">Type</span></span>   | <span data-ttu-id="09ddb-123">说明</span><span class="sxs-lookup"><span data-stu-id="09ddb-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="09ddb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ddb-124">Authorization</span></span> | <span data-ttu-id="09ddb-125">string</span><span class="sxs-lookup"><span data-stu-id="09ddb-125">string</span></span> | <span data-ttu-id="09ddb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09ddb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ddb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="09ddb-128">Request body</span></span>

<span data-ttu-id="09ddb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09ddb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ddb-130">响应</span><span class="sxs-lookup"><span data-stu-id="09ddb-130">Response</span></span>

<span data-ttu-id="09ddb-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09ddb-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ddb-132">示例</span><span class="sxs-lookup"><span data-stu-id="09ddb-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="09ddb-133">请求</span><span class="sxs-lookup"><span data-stu-id="09ddb-133">Request</span></span>

<span data-ttu-id="09ddb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09ddb-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="09ddb-135">响应</span><span class="sxs-lookup"><span data-stu-id="09ddb-135">Response</span></span>

<span data-ttu-id="09ddb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09ddb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
