---
title: 列出 timeOffRequest
description: 检索团队中的 timeOffRequest 对象的列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: be4256b4de4f3ab8e42d5e6486decd191b5edae3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215820"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="e1401-103">列出 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="e1401-103">List timeOffRequest</span></span>

<span data-ttu-id="e1401-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1401-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1401-105">检索团队中的[timeOffRequest](../resources/timeoffrequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e1401-105">Retrieve a list of [timeOffRequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1401-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1401-106">Permissions</span></span>

<span data-ttu-id="e1401-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1401-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1401-109">Permission type</span></span>                        | <span data-ttu-id="e1401-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1401-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="e1401-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1401-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="e1401-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1401-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1401-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1401-114">Not supported.</span></span>    |
|<span data-ttu-id="e1401-115">Application</span><span class="sxs-lookup"><span data-stu-id="e1401-115">Application</span></span> | <span data-ttu-id="e1401-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="e1401-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e1401-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e1401-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e1401-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="e1401-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="e1401-119">目前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="e1401-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1401-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1401-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1401-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1401-121">Optional query parameters</span></span>

<span data-ttu-id="e1401-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e1401-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e1401-123">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e1401-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1401-124">请求头</span><span class="sxs-lookup"><span data-stu-id="e1401-124">Request headers</span></span>

| <span data-ttu-id="e1401-125">名称</span><span class="sxs-lookup"><span data-stu-id="e1401-125">Name</span></span>      |<span data-ttu-id="e1401-126">说明</span><span class="sxs-lookup"><span data-stu-id="e1401-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1401-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1401-127">Authorization</span></span> | <span data-ttu-id="e1401-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1401-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1401-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1401-130">Request body</span></span>

<span data-ttu-id="e1401-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1401-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1401-132">响应</span><span class="sxs-lookup"><span data-stu-id="e1401-132">Response</span></span>

<span data-ttu-id="e1401-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1401-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1401-134">示例</span><span class="sxs-lookup"><span data-stu-id="e1401-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1401-135">请求</span><span class="sxs-lookup"><span data-stu-id="e1401-135">Request</span></span>

<span data-ttu-id="e1401-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1401-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e1401-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1401-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="e1401-138">C#</span><span class="sxs-lookup"><span data-stu-id="e1401-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1401-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1401-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1401-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1401-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1401-141">Java</span><span class="sxs-lookup"><span data-stu-id="e1401-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="e1401-142">响应</span><span class="sxs-lookup"><span data-stu-id="e1401-142">Response</span></span>

<span data-ttu-id="e1401-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1401-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e1401-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1401-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "startDateTime": "datetime-value",
        "endDateTime": "datetime-value",
        "timeOffReasonId": "timeOffReasonId-value"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
