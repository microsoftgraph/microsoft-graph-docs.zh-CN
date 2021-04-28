---
title: 替换班次
description: 替换现有班次。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 888932c4732bca7f15a5eb61327cda9bb554b762
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034894"
---
# <a name="replace-shift"></a><span data-ttu-id="d0f4d-103">替换班次</span><span class="sxs-lookup"><span data-stu-id="d0f4d-103">Replace shift</span></span>

<span data-ttu-id="d0f4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0f4d-105">替换现有的 [班次](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-105">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="d0f4d-106">如果指定的 [班次](../resources/shift.md) 不存在，此方法返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-106">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0f4d-107">权限</span><span class="sxs-lookup"><span data-stu-id="d0f4d-107">Permissions</span></span>

<span data-ttu-id="d0f4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f4d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0f4d-110">Permission type</span></span>      | <span data-ttu-id="d0f4d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0f4d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0f4d-113">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f4d-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0f4d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0f4d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-115">Not supported.</span></span>    |
|<span data-ttu-id="d0f4d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0f4d-116">Application</span></span> | <span data-ttu-id="d0f4d-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f4d-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0f4d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0f4d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="d0f4d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0f4d-119">Request headers</span></span>

| <span data-ttu-id="d0f4d-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0f4d-120">Header</span></span>       | <span data-ttu-id="d0f4d-121">值</span><span class="sxs-lookup"><span data-stu-id="d0f4d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0f4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0f4d-122">Authorization</span></span>  | <span data-ttu-id="d0f4d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0f4d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0f4d-125">Content-Type</span></span>  | <span data-ttu-id="d0f4d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0f4d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0f4d-128">Request body</span></span>

<span data-ttu-id="d0f4d-129">在请求正文中，提供 shift 对象的 JSON [表示](../resources/shift.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d0f4d-130">响应</span><span class="sxs-lookup"><span data-stu-id="d0f4d-130">Response</span></span>

<span data-ttu-id="d0f4d-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [shift](../resources/shift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f4d-132">示例</span><span class="sxs-lookup"><span data-stu-id="d0f4d-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d0f4d-133">请求</span><span class="sxs-lookup"><span data-stu-id="d0f4d-133">Request</span></span>

<span data-ttu-id="d0f4d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0f4d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f4d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d0f4d-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0f4d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0f4d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0f4d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0f4d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0f4d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0f4d-139">Java</span><span class="sxs-lookup"><span data-stu-id="d0f4d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="d0f4d-140">响应</span><span class="sxs-lookup"><span data-stu-id="d0f4d-140">Response</span></span>

<span data-ttu-id="d0f4d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d0f4d-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

