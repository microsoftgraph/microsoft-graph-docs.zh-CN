---
title: 替换 timeOff
description: 替换现有的 timeOff 对象。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b05916566f366793e683e413b3dd44076f2f76a5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051212"
---
# <a name="replace-timeoff"></a><span data-ttu-id="febf4-103">替换 timeOff</span><span class="sxs-lookup"><span data-stu-id="febf4-103">Replace timeOff</span></span>

<span data-ttu-id="febf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="febf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="febf4-105">替换现有的 [timeOff](../resources/timeoff.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="febf4-105">Replace an existing [timeOff](../resources/timeoff.md) object.</span></span>

<span data-ttu-id="febf4-106">如果指定的 [timeOff](../resources/timeoff.md) 对象不存在，此方法将返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="febf4-106">If the specified [timeOff](../resources/timeoff.md) object doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="febf4-107">权限</span><span class="sxs-lookup"><span data-stu-id="febf4-107">Permissions</span></span>

<span data-ttu-id="febf4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="febf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="febf4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="febf4-110">Permission type</span></span>      | <span data-ttu-id="febf4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="febf4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="febf4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="febf4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="febf4-113">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="febf4-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="febf4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="febf4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="febf4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="febf4-115">Not supported.</span></span>    |
|<span data-ttu-id="febf4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="febf4-116">Application</span></span> | <span data-ttu-id="febf4-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="febf4-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="febf4-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="febf4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="febf4-119">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="febf4-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="febf4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="febf4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="febf4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="febf4-121">Request headers</span></span>

| <span data-ttu-id="febf4-122">标头</span><span class="sxs-lookup"><span data-stu-id="febf4-122">Header</span></span>       | <span data-ttu-id="febf4-123">值</span><span class="sxs-lookup"><span data-stu-id="febf4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="febf4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="febf4-124">Authorization</span></span>  | <span data-ttu-id="febf4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="febf4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="febf4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="febf4-127">Content-Type</span></span>  | <span data-ttu-id="febf4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="febf4-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="febf4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="febf4-130">Request body</span></span>

<span data-ttu-id="febf4-131">在请求正文中，提供 [timeOff](../resources/timeoff.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="febf4-131">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="febf4-132">响应</span><span class="sxs-lookup"><span data-stu-id="febf4-132">Response</span></span>

<span data-ttu-id="febf4-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [timeOff](../resources/timeoff.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="febf4-133">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="febf4-134">示例</span><span class="sxs-lookup"><span data-stu-id="febf4-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="febf4-135">请求</span><span class="sxs-lookup"><span data-stu-id="febf4-135">Request</span></span>

<span data-ttu-id="febf4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="febf4-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="febf4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="febf4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="febf4-138">C#</span><span class="sxs-lookup"><span data-stu-id="febf4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="febf4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="febf4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="febf4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="febf4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="febf4-141">Java</span><span class="sxs-lookup"><span data-stu-id="febf4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="febf4-142">响应</span><span class="sxs-lookup"><span data-stu-id="febf4-142">Response</span></span>

<span data-ttu-id="febf4-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="febf4-143">The following is an example of the response.</span></span> 

><span data-ttu-id="febf4-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="febf4-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "@odata.type":"microsoft.graph.identitySet",
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

