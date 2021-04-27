---
title: 获取班次
description: 按 ID 获取班次。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e2f1542d18210b733ecd89b08972ed29d3b9e3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051863"
---
# <a name="get-shift"></a><span data-ttu-id="2ca1d-103">获取班次</span><span class="sxs-lookup"><span data-stu-id="2ca1d-103">Get shift</span></span>

<span data-ttu-id="2ca1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ca1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ca1d-105">按 ID 检索 [shift](../resources/shift.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ca1d-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ca1d-106">Permissions</span></span>

<span data-ttu-id="2ca1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca1d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ca1d-109">Permission type</span></span>      | <span data-ttu-id="2ca1d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ca1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ca1d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ca1d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ca1d-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca1d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ca1d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ca1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ca1d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-114">Not supported.</span></span>    |
|<span data-ttu-id="2ca1d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ca1d-115">Application</span></span> | <span data-ttu-id="2ca1d-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca1d-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ca1d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ca1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ca1d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ca1d-118">Optional query parameters</span></span>

<span data-ttu-id="2ca1d-119">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ca1d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ca1d-120">Request headers</span></span>

| <span data-ttu-id="2ca1d-121">标头</span><span class="sxs-lookup"><span data-stu-id="2ca1d-121">Header</span></span>       | <span data-ttu-id="2ca1d-122">值</span><span class="sxs-lookup"><span data-stu-id="2ca1d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ca1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ca1d-123">Authorization</span></span>  | <span data-ttu-id="2ca1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ca1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ca1d-126">Request body</span></span>
<span data-ttu-id="2ca1d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ca1d-128">响应</span><span class="sxs-lookup"><span data-stu-id="2ca1d-128">Response</span></span>

<span data-ttu-id="2ca1d-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [shift](../resources/shift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-129">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca1d-130">示例</span><span class="sxs-lookup"><span data-stu-id="2ca1d-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2ca1d-131">请求</span><span class="sxs-lookup"><span data-stu-id="2ca1d-131">Request</span></span>

<span data-ttu-id="2ca1d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ca1d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ca1d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="2ca1d-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ca1d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ca1d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ca1d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ca1d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ca1d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ca1d-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ca1d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ca1d-138">响应</span><span class="sxs-lookup"><span data-stu-id="2ca1d-138">Response</span></span>

<span data-ttu-id="2ca1d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-139">The following is an example of the response.</span></span>

><span data-ttu-id="2ca1d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ca1d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


