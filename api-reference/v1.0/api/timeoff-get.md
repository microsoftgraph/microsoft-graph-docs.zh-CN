---
title: 获取 timeOff
description: 按 ID 获取 timeOff。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 562b4699d96ade55880b45fd2c4d7ced77f0d7e4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051219"
---
# <a name="get-timeoff"></a><span data-ttu-id="c5043-103">获取 timeOff</span><span class="sxs-lookup"><span data-stu-id="c5043-103">Get timeOff</span></span>

<span data-ttu-id="c5043-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5043-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5043-105">按 ID 检索 [timeOff 对象](../resources/timeoff.md) 的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5043-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5043-106">权限</span><span class="sxs-lookup"><span data-stu-id="c5043-106">Permissions</span></span>

<span data-ttu-id="c5043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5043-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5043-109">Permission type</span></span>      | <span data-ttu-id="c5043-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5043-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5043-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5043-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5043-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5043-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5043-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5043-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5043-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5043-114">Not supported.</span></span>    |
|<span data-ttu-id="c5043-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5043-115">Application</span></span> | <span data-ttu-id="c5043-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5043-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="c5043-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="c5043-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c5043-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="c5043-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5043-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5043-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5043-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5043-120">Optional query parameters</span></span>

<span data-ttu-id="c5043-121">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5043-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5043-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5043-122">Request headers</span></span>

| <span data-ttu-id="c5043-123">标头</span><span class="sxs-lookup"><span data-stu-id="c5043-123">Header</span></span>       | <span data-ttu-id="c5043-124">值</span><span class="sxs-lookup"><span data-stu-id="c5043-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5043-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5043-125">Authorization</span></span>  | <span data-ttu-id="c5043-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5043-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5043-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5043-128">Request body</span></span>
<span data-ttu-id="c5043-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5043-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5043-130">响应</span><span class="sxs-lookup"><span data-stu-id="c5043-130">Response</span></span>

<span data-ttu-id="c5043-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [timeOff](../resources/timeoff.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5043-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5043-132">示例</span><span class="sxs-lookup"><span data-stu-id="c5043-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c5043-133">请求</span><span class="sxs-lookup"><span data-stu-id="c5043-133">Request</span></span>

<span data-ttu-id="c5043-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5043-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5043-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5043-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="c5043-136">C#</span><span class="sxs-lookup"><span data-stu-id="c5043-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5043-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5043-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5043-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5043-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5043-139">Java</span><span class="sxs-lookup"><span data-stu-id="c5043-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="c5043-140">响应</span><span class="sxs-lookup"><span data-stu-id="c5043-140">Response</span></span>

<span data-ttu-id="c5043-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5043-141">The following is an example of the response.</span></span> 

><span data-ttu-id="c5043-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c5043-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

