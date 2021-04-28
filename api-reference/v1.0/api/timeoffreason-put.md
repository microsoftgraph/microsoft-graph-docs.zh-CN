---
title: 替换 timeOffReason
description: 替换现有的 timeOffReason。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee87ff78baa7ae9b1fd5cf4428b99a167c960fc5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050232"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="3c054-103">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="3c054-103">Replace timeOffReason</span></span>

<span data-ttu-id="3c054-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c054-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c054-105">替换现有的 [timeOffReason](../resources/timeoffreason.md)。</span><span class="sxs-lookup"><span data-stu-id="3c054-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="3c054-106">如果指定的 [timeOffReason](../resources/timeoffreason.md) 不存在，此方法将返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="3c054-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c054-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c054-107">Permissions</span></span>

<span data-ttu-id="3c054-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c054-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c054-110">Permission type</span></span>      | <span data-ttu-id="3c054-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c054-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c054-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c054-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c054-113">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c054-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c054-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c054-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c054-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c054-115">Not supported.</span></span>    |
|<span data-ttu-id="3c054-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c054-116">Application</span></span> | <span data-ttu-id="3c054-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c054-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="3c054-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="3c054-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3c054-119">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="3c054-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c054-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c054-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="3c054-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c054-121">Request headers</span></span>

| <span data-ttu-id="3c054-122">标头</span><span class="sxs-lookup"><span data-stu-id="3c054-122">Header</span></span>       | <span data-ttu-id="3c054-123">值</span><span class="sxs-lookup"><span data-stu-id="3c054-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c054-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c054-124">Authorization</span></span>  | <span data-ttu-id="3c054-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c054-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c054-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c054-127">Content-Type</span></span>  | <span data-ttu-id="3c054-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3c054-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c054-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c054-130">Request body</span></span>

<span data-ttu-id="3c054-131">在请求正文中，提供 [timeOffReason](../resources/timeoffreason.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c054-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c054-132">响应</span><span class="sxs-lookup"><span data-stu-id="3c054-132">Response</span></span>

<span data-ttu-id="3c054-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [timeOffReason](../resources/timeoffreason.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c054-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c054-134">示例</span><span class="sxs-lookup"><span data-stu-id="3c054-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c054-135">请求</span><span class="sxs-lookup"><span data-stu-id="3c054-135">Request</span></span>

<span data-ttu-id="3c054-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c054-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c054-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c054-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="3c054-138">C#</span><span class="sxs-lookup"><span data-stu-id="3c054-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c054-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c054-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c054-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c054-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c054-141">Java</span><span class="sxs-lookup"><span data-stu-id="3c054-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="3c054-142">响应</span><span class="sxs-lookup"><span data-stu-id="3c054-142">Response</span></span>

<span data-ttu-id="3c054-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c054-143">The following is an example of the response.</span></span> 

><span data-ttu-id="3c054-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c054-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
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
      "displayName": "Alex Wilbur"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

