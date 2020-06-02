---
title: 列出 openShifts
description: 列出团队中的 openshift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bc65d419addf58bbf7b0a715c61538491777a5ec
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "42456416"
---
# <a name="list-openshift"></a><span data-ttu-id="6fd46-103">列出 openShift</span><span class="sxs-lookup"><span data-stu-id="6fd46-103">List openShift</span></span>

<span data-ttu-id="6fd46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd46-105">列出团队中的[openshift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fd46-105">List [openshift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fd46-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fd46-106">Permissions</span></span>

<span data-ttu-id="6fd46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fd46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fd46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fd46-109">Permission type</span></span>                        | <span data-ttu-id="6fd46-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fd46-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6fd46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fd46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fd46-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fd46-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6fd46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fd46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fd46-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fd46-114">Not supported.</span></span> |
| <span data-ttu-id="6fd46-115">Application</span><span class="sxs-lookup"><span data-stu-id="6fd46-115">Application</span></span>                            | <span data-ttu-id="6fd46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fd46-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fd46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fd46-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fd46-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6fd46-118">Optional query parameters</span></span>

<span data-ttu-id="6fd46-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6fd46-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6fd46-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6fd46-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="6fd46-121">请求头</span><span class="sxs-lookup"><span data-stu-id="6fd46-121">Request headers</span></span>

| <span data-ttu-id="6fd46-122">名称</span><span class="sxs-lookup"><span data-stu-id="6fd46-122">Name</span></span>      |<span data-ttu-id="6fd46-123">说明</span><span class="sxs-lookup"><span data-stu-id="6fd46-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6fd46-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fd46-124">Authorization</span></span> | <span data-ttu-id="6fd46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fd46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fd46-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fd46-127">Request body</span></span>

<span data-ttu-id="6fd46-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fd46-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fd46-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fd46-129">Response</span></span>

<span data-ttu-id="6fd46-130">如果成功，此方法在 `200 OK` 响应正文中返回团队中的响应代码和所有[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fd46-130">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fd46-131">示例</span><span class="sxs-lookup"><span data-stu-id="6fd46-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fd46-132">请求</span><span class="sxs-lookup"><span data-stu-id="6fd46-132">Request</span></span>

<span data-ttu-id="6fd46-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6fd46-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fd46-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd46-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
```
# <a name="c"></a>[<span data-ttu-id="6fd46-135">C#</span><span class="sxs-lookup"><span data-stu-id="6fd46-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fd46-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fd46-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fd46-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fd46-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fd46-138">响应</span><span class="sxs-lookup"><span data-stu-id="6fd46-138">Response</span></span>

<span data-ttu-id="6fd46-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6fd46-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6fd46-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6fd46-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
