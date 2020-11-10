---
title: 删除班次
description: 删除日程中的班次轮换。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a6a905b8bc27508cb69a0c8b5c71388b0df3044
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969197"
---
# <a name="delete-shift"></a><span data-ttu-id="ce647-103">删除班次</span><span class="sxs-lookup"><span data-stu-id="ce647-103">Delete shift</span></span>

<span data-ttu-id="ce647-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce647-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce647-105">删除日程中的 [班次轮换](../resources/shift.md) 。</span><span class="sxs-lookup"><span data-stu-id="ce647-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce647-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce647-106">Permissions</span></span>

<span data-ttu-id="ce647-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce647-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce647-109">Permission type</span></span>      | <span data-ttu-id="ce647-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce647-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce647-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce647-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce647-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="ce647-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce647-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce647-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce647-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce647-114">Not supported.</span></span>    |
|<span data-ttu-id="ce647-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce647-115">Application</span></span> | <span data-ttu-id="ce647-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="ce647-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce647-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce647-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="ce647-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce647-118">Request headers</span></span>

| <span data-ttu-id="ce647-119">标头</span><span class="sxs-lookup"><span data-stu-id="ce647-119">Header</span></span>       | <span data-ttu-id="ce647-120">值</span><span class="sxs-lookup"><span data-stu-id="ce647-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce647-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce647-121">Authorization</span></span>  | <span data-ttu-id="ce647-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce647-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce647-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce647-124">Request body</span></span>
<span data-ttu-id="ce647-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce647-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce647-126">响应</span><span class="sxs-lookup"><span data-stu-id="ce647-126">Response</span></span>

<span data-ttu-id="ce647-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ce647-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce647-129">示例</span><span class="sxs-lookup"><span data-stu-id="ce647-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ce647-130">请求</span><span class="sxs-lookup"><span data-stu-id="ce647-130">Request</span></span>

<span data-ttu-id="ce647-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce647-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce647-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce647-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="ce647-133">C#</span><span class="sxs-lookup"><span data-stu-id="ce647-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce647-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce647-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce647-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce647-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce647-136">Java</span><span class="sxs-lookup"><span data-stu-id="ce647-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce647-137">响应</span><span class="sxs-lookup"><span data-stu-id="ce647-137">Response</span></span>

<span data-ttu-id="ce647-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce647-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ce647-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ce647-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


