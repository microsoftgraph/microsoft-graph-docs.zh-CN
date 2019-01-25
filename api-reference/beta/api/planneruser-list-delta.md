---
title: 计划工具： 增量
description: 检索用户订阅对象更改。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 772a5d487f48b1552707da45729a84c7fdf7da2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525722"
---
# <a name="planner-delta"></a><span data-ttu-id="42f1c-103">计划工具： 增量</span><span class="sxs-lookup"><span data-stu-id="42f1c-103">Planner: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f1c-104">检索用户是[订阅](../resources/planner-overview.md#track-changes-using-delta-query)的对象更改。</span><span class="sxs-lookup"><span data-stu-id="42f1c-104">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="42f1c-105">此方法允许您的应用程序的用户可以访问从中计划程序随着时间的推移对象跟踪更改。</span><span class="sxs-lookup"><span data-stu-id="42f1c-105">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="42f1c-106">此方法的返回值可能包含 hetergenous 计划程序中的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="42f1c-106">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="42f1c-107">有关跟踪 Microsoft Graph 数据中的更改的详细信息，请参阅[使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="42f1c-107">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="42f1c-108">权限</span><span class="sxs-lookup"><span data-stu-id="42f1c-108">Permissions</span></span>

<span data-ttu-id="42f1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f1c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42f1c-111">Permission type</span></span>      | <span data-ttu-id="42f1c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42f1c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42f1c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42f1c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="42f1c-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f1c-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42f1c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42f1c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f1c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42f1c-116">Not supported.</span></span>    |
|<span data-ttu-id="42f1c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42f1c-117">Application</span></span> | <span data-ttu-id="42f1c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="42f1c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42f1c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42f1c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="42f1c-120">任何其他查询参数 (如`$select`， `$expand`，或`$filter`) 当前支持的增量查询的计划程序的实现。</span><span class="sxs-lookup"><span data-stu-id="42f1c-120">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42f1c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="42f1c-121">Request headers</span></span>

| <span data-ttu-id="42f1c-122">名称</span><span class="sxs-lookup"><span data-stu-id="42f1c-122">Name</span></span>           |<span data-ttu-id="42f1c-123">说明</span><span class="sxs-lookup"><span data-stu-id="42f1c-123">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="42f1c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f1c-124">Authorization</span></span>  | <span data-ttu-id="42f1c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42f1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f1c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42f1c-127">Request body</span></span>

<span data-ttu-id="42f1c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42f1c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42f1c-129">响应</span><span class="sxs-lookup"><span data-stu-id="42f1c-129">Response</span></span>

<span data-ttu-id="42f1c-130">如果成功，此方法返回`200 OK`响应代码和更改要应用于响应正文和要执行增量同步链接中的对象的集合。</span><span class="sxs-lookup"><span data-stu-id="42f1c-130">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="42f1c-131">如果`deltaLink`，呼叫者使用的格式不正确，此终结点将返回 HTTP 400。</span><span class="sxs-lookup"><span data-stu-id="42f1c-131">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="42f1c-132">如果`deltaLink`，呼叫者使用太旧，此终结点将返回 HTTP 410。</span><span class="sxs-lookup"><span data-stu-id="42f1c-132">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="42f1c-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="42f1c-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="42f1c-136">示例</span><span class="sxs-lookup"><span data-stu-id="42f1c-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="42f1c-137">请求</span><span class="sxs-lookup"><span data-stu-id="42f1c-137">Request</span></span>

<span data-ttu-id="42f1c-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42f1c-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="42f1c-139">响应</span><span class="sxs-lookup"><span data-stu-id="42f1c-139">Response</span></span>
<span data-ttu-id="42f1c-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="42f1c-140">Here is an example of the response.</span></span>

><span data-ttu-id="42f1c-141">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="42f1c-141">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="42f1c-142">从实际的呼叫，将返回所有已更改的属性。</span><span class="sxs-lookup"><span data-stu-id="42f1c-142">All the changed properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
