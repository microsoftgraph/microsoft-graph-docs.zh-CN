---
title: 列出 swapShiftsChangeRequest
description: 检索团队中的 swapShiftsChangeRequest 对象列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e32092fbc0834768ec742f56ee02a812bf368a4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952627"
---
# <a name="list-swapshiftschangerequest"></a><span data-ttu-id="772ac-103">列出 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="772ac-103">List swapShiftsChangeRequest</span></span>

<span data-ttu-id="772ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="772ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="772ac-105">检索团队中的 [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="772ac-105">Retrieve a list of [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="772ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="772ac-106">Permissions</span></span>

<span data-ttu-id="772ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="772ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="772ac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="772ac-109">Permission type</span></span>                        | <span data-ttu-id="772ac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="772ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="772ac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="772ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="772ac-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="772ac-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="772ac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="772ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="772ac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="772ac-114">Not supported.</span></span>    |
|<span data-ttu-id="772ac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="772ac-115">Application</span></span> | <span data-ttu-id="772ac-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="772ac-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="772ac-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="772ac-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="772ac-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="772ac-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="772ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="772ac-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="772ac-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="772ac-120">Optional query parameters</span></span>

<span data-ttu-id="772ac-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="772ac-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="772ac-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="772ac-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="772ac-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="772ac-123">Request headers</span></span>

| <span data-ttu-id="772ac-124">名称</span><span class="sxs-lookup"><span data-stu-id="772ac-124">Name</span></span>      |<span data-ttu-id="772ac-125">说明</span><span class="sxs-lookup"><span data-stu-id="772ac-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="772ac-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="772ac-126">Authorization</span></span> | <span data-ttu-id="772ac-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="772ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="772ac-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="772ac-129">Request body</span></span>

<span data-ttu-id="772ac-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="772ac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="772ac-131">响应</span><span class="sxs-lookup"><span data-stu-id="772ac-131">Response</span></span>

<span data-ttu-id="772ac-132">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="772ac-132">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="772ac-133">示例</span><span class="sxs-lookup"><span data-stu-id="772ac-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="772ac-134">请求</span><span class="sxs-lookup"><span data-stu-id="772ac-134">Request</span></span>

<span data-ttu-id="772ac-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="772ac-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="772ac-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="772ac-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests
```
# <a name="c"></a>[<span data-ttu-id="772ac-137">C#</span><span class="sxs-lookup"><span data-stu-id="772ac-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="772ac-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="772ac-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="772ac-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="772ac-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="772ac-140">Java</span><span class="sxs-lookup"><span data-stu-id="772ac-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-swapshiftschangerequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="772ac-141">响应</span><span class="sxs-lookup"><span data-stu-id="772ac-141">Response</span></span>

<span data-ttu-id="772ac-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="772ac-142">The following is an example of the response.</span></span>

> <span data-ttu-id="772ac-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="772ac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
        "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
        "assignedTo": "manager",
        "state": "approved",
        "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
        "senderDateTime": "2019-05-01T10:00:00Z",
        "senderMessage": "I can't make my shift, any chance we can swap?",
        "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
        "recipientActionDateTime": "2019-05-01T11:00:00Z",
        "recipientActionMessage": "Sure!",
        "managerUserId": "fdcc8d43-7f83-438a-9ab1-098e8f2a95ff",
        "managerActionDateTime": "2019-05-01T12:00:00Z",
        "managerActionMessage": "Approved!"
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List swapShiftsChangeRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

