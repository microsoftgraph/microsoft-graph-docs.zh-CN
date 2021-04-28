---
title: 列出 timeOffReasons
description: 获取计划中的 timeOffReasons 列表。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 840b41dbdbd5054c1b3512cfbe1084451a3d6a0c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053872"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="904ca-103">列出 timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="904ca-103">List timeOffReasons</span></span>

<span data-ttu-id="904ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="904ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="904ca-105">获取计划中的 [timeOffReasons](../resources/timeoffreason.md) [列表](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="904ca-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="904ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="904ca-106">Permissions</span></span>

<span data-ttu-id="904ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="904ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="904ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="904ca-109">Permission type</span></span>      | <span data-ttu-id="904ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="904ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="904ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="904ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="904ca-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904ca-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="904ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="904ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="904ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="904ca-114">Not supported.</span></span>    |
|<span data-ttu-id="904ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="904ca-115">Application</span></span> | <span data-ttu-id="904ca-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904ca-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="904ca-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="904ca-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="904ca-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="904ca-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="904ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="904ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="904ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="904ca-120">Request headers</span></span>

| <span data-ttu-id="904ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="904ca-121">Header</span></span>       | <span data-ttu-id="904ca-122">值</span><span class="sxs-lookup"><span data-stu-id="904ca-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="904ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="904ca-123">Authorization</span></span>  | <span data-ttu-id="904ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="904ca-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="904ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="904ca-126">Request body</span></span>
<span data-ttu-id="904ca-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="904ca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="904ca-128">响应</span><span class="sxs-lookup"><span data-stu-id="904ca-128">Response</span></span>

<span data-ttu-id="904ca-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [timeOffReason](../resources/timeoffreason.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="904ca-129">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="904ca-130">示例</span><span class="sxs-lookup"><span data-stu-id="904ca-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="904ca-131">请求</span><span class="sxs-lookup"><span data-stu-id="904ca-131">Request</span></span>

<span data-ttu-id="904ca-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="904ca-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="904ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="904ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
```
# <a name="c"></a>[<span data-ttu-id="904ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="904ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="904ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="904ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="904ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="904ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="904ca-137">Java</span><span class="sxs-lookup"><span data-stu-id="904ca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="904ca-138">响应</span><span class="sxs-lookup"><span data-stu-id="904ca-138">Response</span></span>

<span data-ttu-id="904ca-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="904ca-139">The following is an example of the response.</span></span> 

><span data-ttu-id="904ca-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="904ca-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

