---
title: 列出班次
description: 获取日程安排中的班次列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b57e7f0a8cf2a13961d5825d7da42d3e376cfac8
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314634"
---
# <a name="list-shifts"></a><span data-ttu-id="503c9-103">列出班次</span><span class="sxs-lookup"><span data-stu-id="503c9-103">List shifts</span></span>

<span data-ttu-id="503c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="503c9-105">按[计划](../resources/schedule.md)获取[班次](../resources/shift.md)实例的列表。</span><span class="sxs-lookup"><span data-stu-id="503c9-105">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="503c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="503c9-106">Permissions</span></span>

<span data-ttu-id="503c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="503c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="503c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="503c9-109">Permission type</span></span>      | <span data-ttu-id="503c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="503c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="503c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="503c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="503c9-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="503c9-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="503c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="503c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="503c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="503c9-114">Not supported.</span></span>    |
|<span data-ttu-id="503c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="503c9-115">Application</span></span> | <span data-ttu-id="503c9-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="503c9-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="503c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="503c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="503c9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="503c9-118">Optional query parameters</span></span>
<span data-ttu-id="503c9-119">此方法支持 $filter [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="503c9-119">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="503c9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="503c9-120">Request headers</span></span>

| <span data-ttu-id="503c9-121">标头</span><span class="sxs-lookup"><span data-stu-id="503c9-121">Header</span></span>       | <span data-ttu-id="503c9-122">值</span><span class="sxs-lookup"><span data-stu-id="503c9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="503c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="503c9-123">Authorization</span></span>  | <span data-ttu-id="503c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="503c9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="503c9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="503c9-126">Request body</span></span>
<span data-ttu-id="503c9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="503c9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="503c9-128">响应</span><span class="sxs-lookup"><span data-stu-id="503c9-128">Response</span></span>

<span data-ttu-id="503c9-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [shift](../resources/shift.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="503c9-129">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="503c9-130">示例</span><span class="sxs-lookup"><span data-stu-id="503c9-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="503c9-131">请求</span><span class="sxs-lookup"><span data-stu-id="503c9-131">Request</span></span>

<span data-ttu-id="503c9-132">下面是一个请求的示例，该请求获取具有共享版本的所有 **shift** 对象和在2019年3月18日之间的草稿版本。</span><span class="sxs-lookup"><span data-stu-id="503c9-132">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

# <a name="http"></a>[<span data-ttu-id="503c9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="503c9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```
# <a name="c"></a>[<span data-ttu-id="503c9-134">C#</span><span class="sxs-lookup"><span data-stu-id="503c9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="503c9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="503c9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="503c9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="503c9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="503c9-137">响应</span><span class="sxs-lookup"><span data-stu-id="503c9-137">Response</span></span>

<span data-ttu-id="503c9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="503c9-138">The following is an example of the response.</span></span> 

><span data-ttu-id="503c9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="503c9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


