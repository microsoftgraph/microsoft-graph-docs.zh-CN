---
title: 列出 timesOff
description: 获取此计划中的 timesOff 列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 267ce0ef1fd3aae66cd39a715fa3c0df4e317ec7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336347"
---
# <a name="list-timesoff"></a><span data-ttu-id="1d535-103">列出 timesOff</span><span class="sxs-lookup"><span data-stu-id="1d535-103">List timesOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d535-104">按[计划](../resources/schedule.md)获取[timeOff](../resources/timeoff.md)实例的列表。</span><span class="sxs-lookup"><span data-stu-id="1d535-104">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d535-105">权限</span><span class="sxs-lookup"><span data-stu-id="1d535-105">Permissions</span></span>

<span data-ttu-id="1d535-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d535-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d535-108">Permission type</span></span>      | <span data-ttu-id="1d535-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d535-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d535-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d535-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d535-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d535-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d535-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d535-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d535-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d535-113">Not supported.</span></span>    |
|<span data-ttu-id="1d535-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d535-114">Application</span></span> | <span data-ttu-id="1d535-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d535-115">Not supported.</span></span> |

> <span data-ttu-id="1d535-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="1d535-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1d535-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="1d535-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d535-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d535-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d535-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d535-119">Optional query parameters</span></span>
<span data-ttu-id="1d535-120">此方法支持 $filter [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d535-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d535-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d535-121">Request headers</span></span>

| <span data-ttu-id="1d535-122">标头</span><span class="sxs-lookup"><span data-stu-id="1d535-122">Header</span></span>       | <span data-ttu-id="1d535-123">值</span><span class="sxs-lookup"><span data-stu-id="1d535-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d535-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d535-124">Authorization</span></span>  | <span data-ttu-id="1d535-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d535-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d535-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d535-127">Content-Type</span></span>  | <span data-ttu-id="1d535-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1d535-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d535-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d535-129">Request body</span></span>
<span data-ttu-id="1d535-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d535-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d535-131">响应</span><span class="sxs-lookup"><span data-stu-id="1d535-131">Response</span></span>

<span data-ttu-id="1d535-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d535-132">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d535-133">示例</span><span class="sxs-lookup"><span data-stu-id="1d535-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1d535-134">请求</span><span class="sxs-lookup"><span data-stu-id="1d535-134">Request</span></span>

<span data-ttu-id="1d535-135">下面是一个请求的示例, 该请求获取具有共享版本的所有**timeOff**对象和草稿版本的2019年3月18日之间的草稿。</span><span class="sxs-lookup"><span data-stu-id="1d535-135">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```

#### <a name="response"></a><span data-ttu-id="1d535-136">响应</span><span class="sxs-lookup"><span data-stu-id="1d535-136">Response</span></span>

<span data-ttu-id="1d535-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1d535-137">The following is an example of the response.</span></span> 

><span data-ttu-id="1d535-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1d535-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
