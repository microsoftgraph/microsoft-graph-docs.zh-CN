---
title: 列出 openShifts
description: 列出团队中的 openshift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7fb5c0eb493af6c1d70102f8206999d1004fc0e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057127"
---
# <a name="list-openshifts"></a><span data-ttu-id="d475c-103">列出 openShifts</span><span class="sxs-lookup"><span data-stu-id="d475c-103">List openShifts</span></span>

<span data-ttu-id="d475c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d475c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d475c-105">列出团队中的 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d475c-105">List [openShift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d475c-106">权限</span><span class="sxs-lookup"><span data-stu-id="d475c-106">Permissions</span></span>

<span data-ttu-id="d475c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d475c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d475c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d475c-109">Permission type</span></span>                        | <span data-ttu-id="d475c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d475c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d475c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d475c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d475c-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="d475c-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d475c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d475c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d475c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d475c-114">Not supported.</span></span> |
| <span data-ttu-id="d475c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d475c-115">Application</span></span>                            | <span data-ttu-id="d475c-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="d475c-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="d475c-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="d475c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d475c-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="d475c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d475c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d475c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d475c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d475c-120">Optional query parameters</span></span>

<span data-ttu-id="d475c-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d475c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d475c-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d475c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="d475c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d475c-123">Request headers</span></span>

| <span data-ttu-id="d475c-124">名称</span><span class="sxs-lookup"><span data-stu-id="d475c-124">Name</span></span>      |<span data-ttu-id="d475c-125">说明</span><span class="sxs-lookup"><span data-stu-id="d475c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d475c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d475c-126">Authorization</span></span> | <span data-ttu-id="d475c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d475c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d475c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d475c-129">Request body</span></span>

<span data-ttu-id="d475c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d475c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d475c-131">响应</span><span class="sxs-lookup"><span data-stu-id="d475c-131">Response</span></span>

<span data-ttu-id="d475c-132">如果成功，此方法在 `200 OK` 响应正文中返回团队中的响应代码和所有 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d475c-132">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d475c-133">示例</span><span class="sxs-lookup"><span data-stu-id="d475c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d475c-134">请求</span><span class="sxs-lookup"><span data-stu-id="d475c-134">Request</span></span>

<span data-ttu-id="d475c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d475c-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d475c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d475c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="d475c-137">C#</span><span class="sxs-lookup"><span data-stu-id="d475c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d475c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d475c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d475c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d475c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d475c-140">Java</span><span class="sxs-lookup"><span data-stu-id="d475c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d475c-141">响应</span><span class="sxs-lookup"><span data-stu-id="d475c-141">Response</span></span>

<span data-ttu-id="d475c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d475c-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d475c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d475c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

