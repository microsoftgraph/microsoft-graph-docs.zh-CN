---
title: 创建 timeOffReason
description: 创建新的 timeOffReason。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e4867fb06326b4a8f84cc711fd2d1a1e5219618
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051212"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="14d5c-103">创建 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="14d5c-103">Create timeOffReason</span></span>

<span data-ttu-id="14d5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d5c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14d5c-105">创建新的 [timeOffReason](../resources/timeoffreason.md)。</span><span class="sxs-lookup"><span data-stu-id="14d5c-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="14d5c-106">权限</span><span class="sxs-lookup"><span data-stu-id="14d5c-106">Permissions</span></span>

<span data-ttu-id="14d5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d5c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14d5c-109">Permission type</span></span>      | <span data-ttu-id="14d5c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14d5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14d5c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14d5c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14d5c-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="14d5c-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14d5c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14d5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d5c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14d5c-114">Not supported.</span></span>    |
|<span data-ttu-id="14d5c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14d5c-115">Application</span></span> | <span data-ttu-id="14d5c-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d5c-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="14d5c-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="14d5c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14d5c-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="14d5c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="14d5c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14d5c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="14d5c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14d5c-120">Request headers</span></span>

| <span data-ttu-id="14d5c-121">标头</span><span class="sxs-lookup"><span data-stu-id="14d5c-121">Header</span></span>       | <span data-ttu-id="14d5c-122">值</span><span class="sxs-lookup"><span data-stu-id="14d5c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14d5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14d5c-123">Authorization</span></span>  | <span data-ttu-id="14d5c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14d5c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="14d5c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14d5c-126">Content-Type</span></span>  | <span data-ttu-id="14d5c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="14d5c-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="14d5c-129">响应</span><span class="sxs-lookup"><span data-stu-id="14d5c-129">Response</span></span>

<span data-ttu-id="14d5c-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [timeOffReason](../resources/timeoffreason.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14d5c-130">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d5c-131">示例</span><span class="sxs-lookup"><span data-stu-id="14d5c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14d5c-132">请求</span><span class="sxs-lookup"><span data-stu-id="14d5c-132">Request</span></span>

<span data-ttu-id="14d5c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14d5c-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14d5c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="14d5c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="14d5c-135">C#</span><span class="sxs-lookup"><span data-stu-id="14d5c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14d5c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14d5c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14d5c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14d5c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14d5c-138">Java</span><span class="sxs-lookup"><span data-stu-id="14d5c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="14d5c-139">响应</span><span class="sxs-lookup"><span data-stu-id="14d5c-139">Response</span></span>

<span data-ttu-id="14d5c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14d5c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="14d5c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14d5c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
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
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

