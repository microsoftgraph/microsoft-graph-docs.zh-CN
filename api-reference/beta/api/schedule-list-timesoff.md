---
title: 列出 timesOff
description: 获取此计划中的 timesOff 列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1f3ad2ca2ad07e6285337513dfa7cf5ee151a13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453840"
---
# <a name="list-timesoff"></a><span data-ttu-id="b84bb-103">列出 timesOff</span><span class="sxs-lookup"><span data-stu-id="b84bb-103">List timesOff</span></span>

<span data-ttu-id="b84bb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b84bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b84bb-105">按[计划](../resources/schedule.md)获取[timeOff](../resources/timeoff.md)实例的列表。</span><span class="sxs-lookup"><span data-stu-id="b84bb-105">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b84bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="b84bb-106">Permissions</span></span>

<span data-ttu-id="b84bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b84bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b84bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b84bb-109">Permission type</span></span>      | <span data-ttu-id="b84bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b84bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b84bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b84bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b84bb-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b84bb-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b84bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b84bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b84bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b84bb-114">Not supported.</span></span>    |
|<span data-ttu-id="b84bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b84bb-115">Application</span></span> | <span data-ttu-id="b84bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b84bb-116">Not supported.</span></span> |

> <span data-ttu-id="b84bb-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b84bb-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b84bb-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b84bb-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b84bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b84bb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b84bb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b84bb-120">Optional query parameters</span></span>
<span data-ttu-id="b84bb-121">此方法支持 $filter [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b84bb-121">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b84bb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b84bb-122">Request headers</span></span>

| <span data-ttu-id="b84bb-123">标头</span><span class="sxs-lookup"><span data-stu-id="b84bb-123">Header</span></span>       | <span data-ttu-id="b84bb-124">值</span><span class="sxs-lookup"><span data-stu-id="b84bb-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b84bb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84bb-125">Authorization</span></span>  | <span data-ttu-id="b84bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b84bb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b84bb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b84bb-128">Content-Type</span></span>  | <span data-ttu-id="b84bb-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b84bb-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b84bb-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b84bb-130">Request body</span></span>
<span data-ttu-id="b84bb-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b84bb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b84bb-132">响应</span><span class="sxs-lookup"><span data-stu-id="b84bb-132">Response</span></span>

<span data-ttu-id="b84bb-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b84bb-133">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84bb-134">示例</span><span class="sxs-lookup"><span data-stu-id="b84bb-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b84bb-135">请求</span><span class="sxs-lookup"><span data-stu-id="b84bb-135">Request</span></span>

<span data-ttu-id="b84bb-136">下面是一个请求的示例，该请求获取具有共享版本的所有**timeOff**对象和草稿版本的2019年3月18日之间的草稿。</span><span class="sxs-lookup"><span data-stu-id="b84bb-136">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="b84bb-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b84bb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="b84bb-138">C#</span><span class="sxs-lookup"><span data-stu-id="b84bb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timesoff-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b84bb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b84bb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timesoff-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b84bb-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b84bb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timesoff-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b84bb-141">响应</span><span class="sxs-lookup"><span data-stu-id="b84bb-141">Response</span></span>

<span data-ttu-id="b84bb-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b84bb-142">The following is an example of the response.</span></span> 

><span data-ttu-id="b84bb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b84bb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timesOff in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
