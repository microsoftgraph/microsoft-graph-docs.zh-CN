---
title: 获取班次
description: 按 ID 获取班次。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b0a105d8002a3b257322a7841bae8927bcaee0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960699"
---
# <a name="get-shift"></a><span data-ttu-id="1f812-103">获取班次</span><span class="sxs-lookup"><span data-stu-id="1f812-103">Get shift</span></span>

<span data-ttu-id="1f812-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f812-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f812-105">按 ID 检索 [shift](../resources/shift.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1f812-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f812-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f812-106">Permissions</span></span>

<span data-ttu-id="1f812-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f812-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f812-109">Permission type</span></span>      | <span data-ttu-id="1f812-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f812-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f812-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f812-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f812-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f812-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f812-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f812-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f812-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f812-114">Not supported.</span></span>    |
|<span data-ttu-id="1f812-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f812-115">Application</span></span> | <span data-ttu-id="1f812-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f812-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f812-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f812-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f812-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1f812-118">Optional query parameters</span></span>

<span data-ttu-id="1f812-119">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1f812-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f812-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f812-120">Request headers</span></span>

| <span data-ttu-id="1f812-121">标头</span><span class="sxs-lookup"><span data-stu-id="1f812-121">Header</span></span>       | <span data-ttu-id="1f812-122">值</span><span class="sxs-lookup"><span data-stu-id="1f812-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f812-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f812-123">Authorization</span></span>  | <span data-ttu-id="1f812-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f812-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f812-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f812-126">Request body</span></span>
<span data-ttu-id="1f812-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f812-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f812-128">响应</span><span class="sxs-lookup"><span data-stu-id="1f812-128">Response</span></span>

<span data-ttu-id="1f812-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [shift](../resources/shift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f812-129">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f812-130">示例</span><span class="sxs-lookup"><span data-stu-id="1f812-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1f812-131">请求</span><span class="sxs-lookup"><span data-stu-id="1f812-131">Request</span></span>

<span data-ttu-id="1f812-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1f812-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f812-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f812-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="1f812-134">C#</span><span class="sxs-lookup"><span data-stu-id="1f812-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f812-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f812-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f812-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f812-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f812-137">Java</span><span class="sxs-lookup"><span data-stu-id="1f812-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f812-138">响应</span><span class="sxs-lookup"><span data-stu-id="1f812-138">Response</span></span>

<span data-ttu-id="1f812-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1f812-139">The following is an example of the response.</span></span>

><span data-ttu-id="1f812-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1f812-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHFT_ca485cdd-a42c-4b93-9e6a-6fa54fd45fe1",
    "createdDateTime": "2019-06-06T20:15:38.9Z",
    "lastModifiedDateTime": "2019-11-18T01:12:08.318Z",
    "schedulingGroupId": "TAG_d18fd675-3ac8-41b2-8038-d17fdac8b0d3",
    "userId": "a7b0c8c4-3f5c-492f-ab13-40f0e0f0ffa8",
    "draftShift": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "1c717a55-febd-4850-b5f6-101f3a29972c",
            "displayName": "Sumanth Lingom"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


