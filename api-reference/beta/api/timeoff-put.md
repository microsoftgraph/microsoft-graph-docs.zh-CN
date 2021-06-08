---
title: 替换 timeOff
description: 替换现有的 timeOff。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 535feee59c1f3992d9d78eea1380b50bd841987c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787350"
---
# <a name="replace-timeoff"></a><span data-ttu-id="400de-103">替换 timeOff</span><span class="sxs-lookup"><span data-stu-id="400de-103">Replace timeOff</span></span>

<span data-ttu-id="400de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="400de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="400de-105">替换现有的 [timeOff](../resources/timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="400de-105">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="400de-106">如果指定的 [timeOff](../resources/timeoff.md) 不存在，此方法将返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="400de-106">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="400de-107">权限</span><span class="sxs-lookup"><span data-stu-id="400de-107">Permissions</span></span>

<span data-ttu-id="400de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="400de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="400de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="400de-110">Permission type</span></span>      | <span data-ttu-id="400de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="400de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="400de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="400de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="400de-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="400de-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="400de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="400de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="400de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="400de-115">Not supported.</span></span>    |
|<span data-ttu-id="400de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="400de-116">Application</span></span> | <span data-ttu-id="400de-117">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="400de-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="400de-118">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="400de-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="400de-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="400de-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="400de-120">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="400de-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="400de-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="400de-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="400de-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="400de-122">Request headers</span></span>

| <span data-ttu-id="400de-123">标头</span><span class="sxs-lookup"><span data-stu-id="400de-123">Header</span></span>       | <span data-ttu-id="400de-124">值</span><span class="sxs-lookup"><span data-stu-id="400de-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="400de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="400de-125">Authorization</span></span>  | <span data-ttu-id="400de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="400de-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="400de-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="400de-128">Content-Type</span></span>  | <span data-ttu-id="400de-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="400de-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="400de-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="400de-131">Request body</span></span>

<span data-ttu-id="400de-132">在请求正文中，提供 [timeOff](../resources/timeoff.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="400de-132">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="400de-133">响应</span><span class="sxs-lookup"><span data-stu-id="400de-133">Response</span></span>

<span data-ttu-id="400de-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [timeOff](../resources/timeoff.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="400de-134">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="400de-135">示例</span><span class="sxs-lookup"><span data-stu-id="400de-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="400de-136">请求</span><span class="sxs-lookup"><span data-stu-id="400de-136">Request</span></span>

<span data-ttu-id="400de-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="400de-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="400de-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="400de-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
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
# <a name="c"></a>[<span data-ttu-id="400de-139">C#</span><span class="sxs-lookup"><span data-stu-id="400de-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="400de-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="400de-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="400de-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="400de-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="400de-142">Java</span><span class="sxs-lookup"><span data-stu-id="400de-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="400de-143">响应</span><span class="sxs-lookup"><span data-stu-id="400de-143">Response</span></span>

<span data-ttu-id="400de-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="400de-144">The following is an example of the response.</span></span> 

><span data-ttu-id="400de-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="400de-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


