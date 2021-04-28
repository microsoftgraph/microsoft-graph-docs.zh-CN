---
title: 创建 offerShiftRequest
description: 创建 offerShiftRequest 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d6cc8615d35190376a409af5efbd794a1b55f2d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049490"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="7021b-103">创建 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="7021b-103">Create offerShiftRequest</span></span>

<span data-ttu-id="7021b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7021b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7021b-105">创建 [offerShiftRequest 的实例](../resources/offershiftrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="7021b-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7021b-106">权限</span><span class="sxs-lookup"><span data-stu-id="7021b-106">Permissions</span></span>

<span data-ttu-id="7021b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7021b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7021b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7021b-109">Permission type</span></span>                        | <span data-ttu-id="7021b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7021b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7021b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7021b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7021b-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7021b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7021b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7021b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7021b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7021b-114">Not supported.</span></span> |
| <span data-ttu-id="7021b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7021b-115">Application</span></span>                            | <span data-ttu-id="7021b-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7021b-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7021b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7021b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="7021b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7021b-118">Request headers</span></span>

| <span data-ttu-id="7021b-119">名称</span><span class="sxs-lookup"><span data-stu-id="7021b-119">Name</span></span>      |<span data-ttu-id="7021b-120">说明</span><span class="sxs-lookup"><span data-stu-id="7021b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7021b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7021b-121">Authorization</span></span> | <span data-ttu-id="7021b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7021b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7021b-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="7021b-124">Content-type</span></span> | <span data-ttu-id="7021b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7021b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7021b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7021b-127">Request body</span></span>
<span data-ttu-id="7021b-128">在此方法的请求正文中提供新的 [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7021b-128">Provide the new [offerShiftRequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7021b-129">响应</span><span class="sxs-lookup"><span data-stu-id="7021b-129">Response</span></span>

<span data-ttu-id="7021b-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7021b-130">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7021b-131">示例</span><span class="sxs-lookup"><span data-stu-id="7021b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7021b-132">请求</span><span class="sxs-lookup"><span data-stu-id="7021b-132">Request</span></span>

<span data-ttu-id="7021b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7021b-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7021b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7021b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_3"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```
# <a name="c"></a>[<span data-ttu-id="7021b-135">C#</span><span class="sxs-lookup"><span data-stu-id="7021b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7021b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7021b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7021b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7021b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7021b-138">Java</span><span class="sxs-lookup"><span data-stu-id="7021b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="7021b-139">响应</span><span class="sxs-lookup"><span data-stu-id="7021b-139">Response</span></span>

<span data-ttu-id="7021b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7021b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7021b-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7021b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

