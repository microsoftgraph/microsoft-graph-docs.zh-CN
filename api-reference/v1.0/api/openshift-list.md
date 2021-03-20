---
title: 列出 openShifts
description: 列出团队中的 openshift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5717a77c06c18e5ce36594eefcfd4130dbb8ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953481"
---
# <a name="list-openshifts"></a><span data-ttu-id="e701d-103">列出 openShifts</span><span class="sxs-lookup"><span data-stu-id="e701d-103">List openShifts</span></span>

<span data-ttu-id="e701d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e701d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e701d-105">列出 [团队中的 openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e701d-105">List [openShift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="e701d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e701d-106">Permissions</span></span>

<span data-ttu-id="e701d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e701d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e701d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e701d-109">Permission type</span></span>                        | <span data-ttu-id="e701d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e701d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e701d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e701d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e701d-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e701d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e701d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e701d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e701d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e701d-114">Not supported.</span></span> |
| <span data-ttu-id="e701d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e701d-115">Application</span></span>                            | <span data-ttu-id="e701d-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e701d-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e701d-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e701d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e701d-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="e701d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e701d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e701d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e701d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e701d-120">Optional query parameters</span></span>

<span data-ttu-id="e701d-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e701d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e701d-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e701d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="e701d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e701d-123">Request headers</span></span>

| <span data-ttu-id="e701d-124">名称</span><span class="sxs-lookup"><span data-stu-id="e701d-124">Name</span></span>      |<span data-ttu-id="e701d-125">说明</span><span class="sxs-lookup"><span data-stu-id="e701d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e701d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e701d-126">Authorization</span></span> | <span data-ttu-id="e701d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e701d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e701d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e701d-129">Request body</span></span>

<span data-ttu-id="e701d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e701d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e701d-131">响应</span><span class="sxs-lookup"><span data-stu-id="e701d-131">Response</span></span>

<span data-ttu-id="e701d-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和团队中所有 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e701d-132">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e701d-133">示例</span><span class="sxs-lookup"><span data-stu-id="e701d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e701d-134">请求</span><span class="sxs-lookup"><span data-stu-id="e701d-134">Request</span></span>

<span data-ttu-id="e701d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e701d-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e701d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e701d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="e701d-137">C#</span><span class="sxs-lookup"><span data-stu-id="e701d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e701d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e701d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e701d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e701d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e701d-140">Java</span><span class="sxs-lookup"><span data-stu-id="e701d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="e701d-141">响应</span><span class="sxs-lookup"><span data-stu-id="e701d-141">Response</span></span>

<span data-ttu-id="e701d-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e701d-142">The following is an example of the response.</span></span>

> <span data-ttu-id="e701d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e701d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
  "application": null,
  "device": null,
  "conversation": null,
  "user": {
  "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
  "displayName": "John Doe"
  }
  }
  }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

