---
title: 获取 schedulingGroup
description: 按 ID 检索 [schedulingGroup](../resources/schedulinggroup.md) 的属性和关系。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b8784aa4e3f5b2c77b0da185e5c3e5eb30856fa3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975672"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="913e9-103">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="913e9-103">Get schedulingGroup</span></span>

<span data-ttu-id="913e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="913e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="913e9-105">按 ID 检索 [schedulingGroup](../resources/schedulinggroup.md) 的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="913e9-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="913e9-106">权限</span><span class="sxs-lookup"><span data-stu-id="913e9-106">Permissions</span></span>

<span data-ttu-id="913e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="913e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="913e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="913e9-109">Permission type</span></span>      | <span data-ttu-id="913e9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="913e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="913e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="913e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="913e9-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="913e9-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="913e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="913e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913e9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="913e9-114">Not supported.</span></span>    |
|<span data-ttu-id="913e9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="913e9-115">Application</span></span> | <span data-ttu-id="913e9-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="913e9-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="913e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="913e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="913e9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="913e9-118">Optional query parameters</span></span>

<span data-ttu-id="913e9-119">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="913e9-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="913e9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="913e9-120">Request headers</span></span>

| <span data-ttu-id="913e9-121">标头</span><span class="sxs-lookup"><span data-stu-id="913e9-121">Header</span></span>       | <span data-ttu-id="913e9-122">值</span><span class="sxs-lookup"><span data-stu-id="913e9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="913e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="913e9-123">Authorization</span></span>  | <span data-ttu-id="913e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="913e9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="913e9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="913e9-126">Request body</span></span>
<span data-ttu-id="913e9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="913e9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="913e9-128">响应</span><span class="sxs-lookup"><span data-stu-id="913e9-128">Response</span></span>

<span data-ttu-id="913e9-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="913e9-129">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="913e9-130">示例</span><span class="sxs-lookup"><span data-stu-id="913e9-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="913e9-131">请求</span><span class="sxs-lookup"><span data-stu-id="913e9-131">Request</span></span>

<span data-ttu-id="913e9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="913e9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="913e9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="913e9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="913e9-134">C#</span><span class="sxs-lookup"><span data-stu-id="913e9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="913e9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="913e9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="913e9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="913e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="913e9-137">Java</span><span class="sxs-lookup"><span data-stu-id="913e9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="913e9-138">响应</span><span class="sxs-lookup"><span data-stu-id="913e9-138">Response</span></span>

<span data-ttu-id="913e9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="913e9-139">The following is an example of the response.</span></span> 

><span data-ttu-id="913e9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="913e9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


