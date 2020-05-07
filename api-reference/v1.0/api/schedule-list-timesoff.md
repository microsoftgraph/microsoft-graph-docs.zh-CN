---
title: 列出 timesOff
description: 获取此计划中的 timesOff 列表。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 59791d2959b6ebed13d5d176cff6444df60b5227
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154524"
---
# <a name="list-timesoff"></a><span data-ttu-id="f5d4f-103">列出 timesOff</span><span class="sxs-lookup"><span data-stu-id="f5d4f-103">List timesOff</span></span>

<span data-ttu-id="f5d4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5d4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5d4f-105">按[计划](../resources/schedule.md)获取[timeOff](../resources/timeoff.md)实例的列表。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-105">Get the list of [timeOff](../resources/timeoff.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d4f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5d4f-106">Permissions</span></span>

<span data-ttu-id="f5d4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d4f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5d4f-109">Permission type</span></span>      | <span data-ttu-id="f5d4f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5d4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5d4f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5d4f-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="f5d4f-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5d4f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5d4f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-114">Not supported.</span></span>    |
|<span data-ttu-id="f5d4f-115">Application</span><span class="sxs-lookup"><span data-stu-id="f5d4f-115">Application</span></span> | <span data-ttu-id="f5d4f-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="f5d4f-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f5d4f-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f5d4f-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f5d4f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5d4f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5d4f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f5d4f-120">Optional query parameters</span></span>
<span data-ttu-id="f5d4f-121">此方法支持`$filter` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-121">This method supports the `$filter` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5d4f-122">请求头</span><span class="sxs-lookup"><span data-stu-id="f5d4f-122">Request headers</span></span>

| <span data-ttu-id="f5d4f-123">标头</span><span class="sxs-lookup"><span data-stu-id="f5d4f-123">Header</span></span>       | <span data-ttu-id="f5d4f-124">值</span><span class="sxs-lookup"><span data-stu-id="f5d4f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5d4f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5d4f-125">Authorization</span></span>  | <span data-ttu-id="f5d4f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5d4f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5d4f-128">Request body</span></span>
<span data-ttu-id="f5d4f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5d4f-130">响应</span><span class="sxs-lookup"><span data-stu-id="f5d4f-130">Response</span></span>

<span data-ttu-id="f5d4f-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-131">If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5d4f-132">示例</span><span class="sxs-lookup"><span data-stu-id="f5d4f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5d4f-133">请求</span><span class="sxs-lookup"><span data-stu-id="f5d4f-133">Request</span></span>

<span data-ttu-id="f5d4f-134">下面是一个请求的示例，该请求获取具有共享版本的所有**timeOff**对象和草稿版本的2019年3月18日之间的草稿。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-134">The following is an example of a request that gets all **timeOff** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-list-timesoff"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff?$filter=sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z
```
---


### <a name="response"></a><span data-ttu-id="f5d4f-135">响应</span><span class="sxs-lookup"><span data-stu-id="f5d4f-135">Response</span></span>

<span data-ttu-id="f5d4f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-136">The following is an example of the response.</span></span> 

><span data-ttu-id="f5d4f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f5d4f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
