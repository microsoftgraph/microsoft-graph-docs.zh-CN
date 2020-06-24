---
title: 获取 shift
description: 按 ID 获取 shift。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 329d89d8a06182d5de7f9b3d149e348c7f7df4e7
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845692"
---
# <a name="get-shift"></a><span data-ttu-id="132a2-103">获取 shift</span><span class="sxs-lookup"><span data-stu-id="132a2-103">Get shift</span></span>

<span data-ttu-id="132a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="132a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="132a2-105">按 ID 检索[shift](../resources/shift.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="132a2-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="132a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="132a2-106">Permissions</span></span>

<span data-ttu-id="132a2-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="132a2-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="132a2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="132a2-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="132a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="132a2-109">Permission type</span></span>                        | <span data-ttu-id="132a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="132a2-110">Permissions (from least to most privileged)</span></span>                                    |
|:---------------------------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="132a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="132a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="132a2-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="132a2-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="132a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="132a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="132a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="132a2-114">Not supported.</span></span>                                                                 |
| <span data-ttu-id="132a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="132a2-115">Application</span></span>                            | <span data-ttu-id="132a2-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="132a2-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span>                                      |

> <span data-ttu-id="132a2-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="132a2-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="132a2-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="132a2-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="132a2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="132a2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="132a2-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="132a2-120">Optional query parameters</span></span>

<span data-ttu-id="132a2-121">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="132a2-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="132a2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="132a2-122">Request headers</span></span>

| <span data-ttu-id="132a2-123">标头</span><span class="sxs-lookup"><span data-stu-id="132a2-123">Header</span></span>       | <span data-ttu-id="132a2-124">值</span><span class="sxs-lookup"><span data-stu-id="132a2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="132a2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="132a2-125">Authorization</span></span>  | <span data-ttu-id="132a2-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="132a2-126">Bearer {token}.</span></span> <span data-ttu-id="132a2-127">Required.</span><span class="sxs-lookup"><span data-stu-id="132a2-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="132a2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="132a2-128">Request body</span></span>
<span data-ttu-id="132a2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="132a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="132a2-130">响应</span><span class="sxs-lookup"><span data-stu-id="132a2-130">Response</span></span>

<span data-ttu-id="132a2-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="132a2-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="132a2-132">示例</span><span class="sxs-lookup"><span data-stu-id="132a2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="132a2-133">请求</span><span class="sxs-lookup"><span data-stu-id="132a2-133">Request</span></span>

<span data-ttu-id="132a2-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="132a2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="132a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="132a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="132a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="132a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="132a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="132a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="132a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="132a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="132a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="132a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="132a2-140">响应</span><span class="sxs-lookup"><span data-stu-id="132a2-140">Response</span></span>

<span data-ttu-id="132a2-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="132a2-141">The following is an example of the response.</span></span>

><span data-ttu-id="132a2-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="132a2-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="132a2-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="132a2-143">All the properties will be returned from an actual call.</span></span>
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
