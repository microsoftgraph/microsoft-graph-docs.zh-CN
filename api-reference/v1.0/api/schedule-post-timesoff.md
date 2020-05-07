---
title: 创建 timeOff
description: 创建新的 timeOff。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8fd943cca84ac894b87da3499356cc4581fe951e
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154487"
---
# <a name="create-timeoff"></a><span data-ttu-id="816e3-103">创建 timeOff</span><span class="sxs-lookup"><span data-stu-id="816e3-103">Create timeOff</span></span>

<span data-ttu-id="816e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="816e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="816e3-105">在[计划](../resources/schedule.md)中创建新的[timeOff](../resources/timeoff.md)实例。</span><span class="sxs-lookup"><span data-stu-id="816e3-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="816e3-106">权限</span><span class="sxs-lookup"><span data-stu-id="816e3-106">Permissions</span></span>

<span data-ttu-id="816e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="816e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816e3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="816e3-109">Permission type</span></span>      | <span data-ttu-id="816e3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="816e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="816e3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="816e3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="816e3-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="816e3-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="816e3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="816e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="816e3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="816e3-114">Not supported.</span></span>    |
|<span data-ttu-id="816e3-115">Application</span><span class="sxs-lookup"><span data-stu-id="816e3-115">Application</span></span> | <span data-ttu-id="816e3-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="816e3-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="816e3-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="816e3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="816e3-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="816e3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="816e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="816e3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="816e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="816e3-120">Request headers</span></span>

| <span data-ttu-id="816e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="816e3-121">Header</span></span>       | <span data-ttu-id="816e3-122">值</span><span class="sxs-lookup"><span data-stu-id="816e3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="816e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="816e3-123">Authorization</span></span>  | <span data-ttu-id="816e3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="816e3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="816e3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="816e3-126">Content-Type</span></span>  | <span data-ttu-id="816e3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="816e3-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="816e3-129">响应</span><span class="sxs-lookup"><span data-stu-id="816e3-129">Response</span></span>

<span data-ttu-id="816e3-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和[timeOff](../resources/timeoff.md)对象。</span><span class="sxs-lookup"><span data-stu-id="816e3-130">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="816e3-131">示例</span><span class="sxs-lookup"><span data-stu-id="816e3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="816e3-132">请求</span><span class="sxs-lookup"><span data-stu-id="816e3-132">Request</span></span>

<span data-ttu-id="816e3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="816e3-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff
Content-type: application/json

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

---

### <a name="response"></a><span data-ttu-id="816e3-134">响应</span><span class="sxs-lookup"><span data-stu-id="816e3-134">Response</span></span>

<span data-ttu-id="816e3-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="816e3-135">The following is an example of the response.</span></span> 

><span data-ttu-id="816e3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="816e3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type":"microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
