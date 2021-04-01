---
title: Planner： delta
description: 检索用户订阅的对象更改。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7c730630f3fd655db29c93c699e8090d3046a4d4
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473491"
---
# <a name="planner-delta"></a><span data-ttu-id="b0d17-103">Planner： delta</span><span class="sxs-lookup"><span data-stu-id="b0d17-103">Planner: delta</span></span>

<span data-ttu-id="b0d17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d17-105">检索用户订阅的对象 [更改](../resources/planner-overview.md#track-changes-using-delta-query) 。</span><span class="sxs-lookup"><span data-stu-id="b0d17-105">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="b0d17-106">此方法允许应用程序跟踪用户随着时间的推移可以从 Planner 内访问的对象的更改。</span><span class="sxs-lookup"><span data-stu-id="b0d17-106">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="b0d17-107">此方法的返回值可能包含 Planner 中的对象的异种类型。</span><span class="sxs-lookup"><span data-stu-id="b0d17-107">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="b0d17-108">有关跟踪 Microsoft Graph 数据更改详细信息，请参阅使用 delta 查询跟踪 [Microsoft Graph 数据中的更改](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="b0d17-108">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0d17-109">权限</span><span class="sxs-lookup"><span data-stu-id="b0d17-109">Permissions</span></span>

<span data-ttu-id="b0d17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0d17-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0d17-112">Permission type</span></span>      | <span data-ttu-id="b0d17-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0d17-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0d17-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0d17-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b0d17-115">Tasks.Read、Tasks.ReadWrite、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0d17-115">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0d17-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0d17-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0d17-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0d17-117">Not supported.</span></span>    |
|<span data-ttu-id="b0d17-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0d17-118">Application</span></span> | <span data-ttu-id="b0d17-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0d17-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0d17-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0d17-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/{id}/planner/all/delta
```

<span data-ttu-id="b0d17-121">Planner 的增量 (上当前不支持其他查询参数) 如 、 或 `$select` `$expand` `$filter`) 。</span><span class="sxs-lookup"><span data-stu-id="b0d17-121">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0d17-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0d17-122">Request headers</span></span>

| <span data-ttu-id="b0d17-123">名称</span><span class="sxs-lookup"><span data-stu-id="b0d17-123">Name</span></span>           |<span data-ttu-id="b0d17-124">说明</span><span class="sxs-lookup"><span data-stu-id="b0d17-124">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="b0d17-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0d17-125">Authorization</span></span>  | <span data-ttu-id="b0d17-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0d17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0d17-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0d17-128">Request body</span></span>

<span data-ttu-id="b0d17-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0d17-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0d17-130">响应</span><span class="sxs-lookup"><span data-stu-id="b0d17-130">Response</span></span>

<span data-ttu-id="b0d17-131">如果成功，此方法返回 响应代码和要应用于响应正文中的对象的更改集合，以及要遵循的 `200 OK` Delta Sync 链接。</span><span class="sxs-lookup"><span data-stu-id="b0d17-131">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="b0d17-132">如果 `deltaLink` 调用方使用的 格式不正确，此终结点将返回 HTTP 400。</span><span class="sxs-lookup"><span data-stu-id="b0d17-132">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="b0d17-133">如果 `deltaLink` 调用方使用的 太旧，此终结点将返回 HTTP 410。</span><span class="sxs-lookup"><span data-stu-id="b0d17-133">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="b0d17-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b0d17-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b0d17-137">示例</span><span class="sxs-lookup"><span data-stu-id="b0d17-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0d17-138">请求</span><span class="sxs-lookup"><span data-stu-id="b0d17-138">Request</span></span>

<span data-ttu-id="b0d17-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0d17-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b0d17-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d17-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="c"></a>[<span data-ttu-id="b0d17-141">C#</span><span class="sxs-lookup"><span data-stu-id="b0d17-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0d17-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0d17-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0d17-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0d17-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0d17-144">Java</span><span class="sxs-lookup"><span data-stu-id="b0d17-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0d17-145">响应</span><span class="sxs-lookup"><span data-stu-id="b0d17-145">Response</span></span>
<span data-ttu-id="b0d17-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b0d17-146">Here is an example of the response.</span></span>

><span data-ttu-id="b0d17-147">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="b0d17-147">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="b0d17-148">所有更改的属性都将从实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="b0d17-148">All the changed properties will be returned from an actual call.</span></span>

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
  ]
}
-->


