---
title: 计划工具： 增量
description: 检索用户订阅对象更改。
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 4fe4ed9164c5baf9aea8819ba4f3140c23ec87d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838638"
---
# <a name="planner-delta"></a><span data-ttu-id="7795c-103">计划工具： 增量</span><span class="sxs-lookup"><span data-stu-id="7795c-103">Planner: delta</span></span>

> <span data-ttu-id="7795c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7795c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7795c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7795c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7795c-106">检索用户是[订阅](../resources/planner-overview.md#track-changes-using-delta-query)的对象更改。</span><span class="sxs-lookup"><span data-stu-id="7795c-106">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="7795c-107">此方法允许您的应用程序的用户可以访问从中计划程序随着时间的推移对象跟踪更改。</span><span class="sxs-lookup"><span data-stu-id="7795c-107">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="7795c-108">此方法的返回值可能包含 hetergenous 计划程序中的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="7795c-108">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="7795c-109">有关跟踪 Microsoft Graph 数据中的更改的详细信息，请参阅[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="7795c-109">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="7795c-110">权限</span><span class="sxs-lookup"><span data-stu-id="7795c-110">Permissions</span></span>

<span data-ttu-id="7795c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7795c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7795c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7795c-113">Permission type</span></span>      | <span data-ttu-id="7795c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7795c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7795c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7795c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7795c-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7795c-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7795c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7795c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7795c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7795c-118">Not supported.</span></span>    |
|<span data-ttu-id="7795c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7795c-119">Application</span></span> | <span data-ttu-id="7795c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7795c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7795c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7795c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="7795c-122">任何其他查询参数 (如`$select`， `$expand`，或`$filter`) 当前支持的增量查询的计划程序的实现。</span><span class="sxs-lookup"><span data-stu-id="7795c-122">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7795c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7795c-123">Request headers</span></span>

| <span data-ttu-id="7795c-124">名称</span><span class="sxs-lookup"><span data-stu-id="7795c-124">Name</span></span>           |<span data-ttu-id="7795c-125">说明</span><span class="sxs-lookup"><span data-stu-id="7795c-125">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="7795c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7795c-126">Authorization</span></span>  | <span data-ttu-id="7795c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7795c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7795c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7795c-129">Request body</span></span>

<span data-ttu-id="7795c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7795c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7795c-131">响应</span><span class="sxs-lookup"><span data-stu-id="7795c-131">Response</span></span>

<span data-ttu-id="7795c-132">如果成功，此方法返回`200 OK`响应代码和更改要应用于响应正文和要执行增量同步链接中的对象的集合。</span><span class="sxs-lookup"><span data-stu-id="7795c-132">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="7795c-133">如果`deltaLink`，呼叫者使用的格式不正确，此终结点将返回 HTTP 400。</span><span class="sxs-lookup"><span data-stu-id="7795c-133">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="7795c-134">如果`deltaLink`，呼叫者使用太旧，此终结点将返回 HTTP 410。</span><span class="sxs-lookup"><span data-stu-id="7795c-134">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="7795c-p104">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="7795c-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7795c-138">示例</span><span class="sxs-lookup"><span data-stu-id="7795c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7795c-139">请求</span><span class="sxs-lookup"><span data-stu-id="7795c-139">Request</span></span>

<span data-ttu-id="7795c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7795c-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="7795c-141">响应</span><span class="sxs-lookup"><span data-stu-id="7795c-141">Response</span></span>
<span data-ttu-id="7795c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7795c-142">Here is an example of the response.</span></span>

><span data-ttu-id="7795c-143">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="7795c-143">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="7795c-144">从实际的呼叫，将返回所有已更改的属性。</span><span class="sxs-lookup"><span data-stu-id="7795c-144">All the changed properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_delta",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.entity)",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
cache-control: private
client-request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
preference-applied: odata.track-changes, odata.track-changes

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerDelta)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/planner/all/delta?$deltatoken=jVztGMFnm7qLEQ69FaXzWF5sPEJZU2YxZa32QEvnZTZ4q4C10ThM5uL7bEPm9ysqrxOY0QQIb4Uqmc9DH3rn7pczamvtCipDVJ4FivXh398.J9pSVKpytlutvx03-iBmO4ZM_3qPztOq2T9VIjHoRR0",
    "value": [
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBASCc=\"",
            "percentComplete": 100,
            "completedDateTime": "2018-03-13T21:31:25.778Z",
            "completedBy": {
                "user": {
                    "id": "8414b634-316f-41ba-b6a6-646a2949e3a5"
                }
            },
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBATCc=\"",
            "percentComplete": 0,
            "completedDateTime": null,
            "completedBy": null,
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAUCc=\"",
            "title": "Title change",
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
