---
title: 列出 timeOffRequest
description: 检索团队中的 timeOffRequest 对象列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e04fb8dba357328247434fb0bfb63598a96fde9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963541"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="f3593-103">列出 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="f3593-103">List timeOffRequest</span></span>

<span data-ttu-id="f3593-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3593-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3593-105">检索团队中的 [timeOffRequest](../resources/timeoffrequest.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="f3593-105">Retrieve a list of [timeOffRequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3593-106">权限</span><span class="sxs-lookup"><span data-stu-id="f3593-106">Permissions</span></span>

<span data-ttu-id="f3593-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3593-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3593-109">Permission type</span></span>                        | <span data-ttu-id="f3593-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3593-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="f3593-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3593-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3593-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3593-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3593-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3593-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3593-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3593-114">Not supported.</span></span>    |
|<span data-ttu-id="f3593-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3593-115">Application</span></span> | <span data-ttu-id="f3593-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3593-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f3593-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="f3593-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f3593-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="f3593-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="f3593-119">目前仅在个人预览版中，不可用于公共用途。</span><span class="sxs-lookup"><span data-stu-id="f3593-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="f3593-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3593-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3593-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f3593-121">Optional query parameters</span></span>

<span data-ttu-id="f3593-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f3593-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f3593-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f3593-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3593-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3593-124">Request headers</span></span>

| <span data-ttu-id="f3593-125">名称</span><span class="sxs-lookup"><span data-stu-id="f3593-125">Name</span></span>      |<span data-ttu-id="f3593-126">说明</span><span class="sxs-lookup"><span data-stu-id="f3593-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3593-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3593-127">Authorization</span></span> | <span data-ttu-id="f3593-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f3593-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3593-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3593-130">Request body</span></span>

<span data-ttu-id="f3593-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3593-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3593-132">响应</span><span class="sxs-lookup"><span data-stu-id="f3593-132">Response</span></span>

<span data-ttu-id="f3593-133">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3593-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3593-134">示例</span><span class="sxs-lookup"><span data-stu-id="f3593-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3593-135">请求</span><span class="sxs-lookup"><span data-stu-id="f3593-135">Request</span></span>

<span data-ttu-id="f3593-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f3593-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f3593-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3593-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="f3593-138">C#</span><span class="sxs-lookup"><span data-stu-id="f3593-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3593-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3593-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3593-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3593-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3593-141">Java</span><span class="sxs-lookup"><span data-stu-id="f3593-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="f3593-142">响应</span><span class="sxs-lookup"><span data-stu-id="f3593-142">Response</span></span>

<span data-ttu-id="f3593-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f3593-143">The following is an example of the response.</span></span>

> <span data-ttu-id="f3593-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f3593-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

