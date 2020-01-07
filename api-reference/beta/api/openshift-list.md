---
title: 列出 openShifts
description: 列出团队中的 openshift 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2eec0931a3c79587553bcba82758b96b398599dc
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952228"
---
# <a name="list-openshift"></a><span data-ttu-id="6e20a-103">列出 openShift</span><span class="sxs-lookup"><span data-stu-id="6e20a-103">List openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e20a-104">列出团队中的[openshift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e20a-104">List [openshift](../resources/openshift.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e20a-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e20a-105">Permissions</span></span>

<span data-ttu-id="6e20a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e20a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e20a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e20a-108">Permission type</span></span>                        | <span data-ttu-id="6e20a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e20a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e20a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e20a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e20a-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e20a-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6e20a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e20a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e20a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e20a-113">Not supported.</span></span> |
| <span data-ttu-id="6e20a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e20a-114">Application</span></span>                            | <span data-ttu-id="6e20a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e20a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e20a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e20a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e20a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e20a-117">Optional query parameters</span></span>

<span data-ttu-id="6e20a-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e20a-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6e20a-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6e20a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="6e20a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e20a-120">Request headers</span></span>

| <span data-ttu-id="6e20a-121">名称</span><span class="sxs-lookup"><span data-stu-id="6e20a-121">Name</span></span>      |<span data-ttu-id="6e20a-122">说明</span><span class="sxs-lookup"><span data-stu-id="6e20a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e20a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e20a-123">Authorization</span></span> | <span data-ttu-id="6e20a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e20a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e20a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e20a-126">Request body</span></span>

<span data-ttu-id="6e20a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e20a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e20a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6e20a-128">Response</span></span>

<span data-ttu-id="6e20a-129">如果成功，此方法在响应`200 OK`正文中返回团队中的响应代码和所有[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e20a-129">If successful, this method returns a `200 OK` response code and all [openShift](../resources/openshift.md) objects in the team in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e20a-130">示例</span><span class="sxs-lookup"><span data-stu-id="6e20a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e20a-131">请求</span><span class="sxs-lookup"><span data-stu-id="6e20a-131">Request</span></span>

<span data-ttu-id="6e20a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e20a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
```

### <a name="response"></a><span data-ttu-id="6e20a-133">响应</span><span class="sxs-lookup"><span data-stu-id="6e20a-133">Response</span></span>

<span data-ttu-id="6e20a-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e20a-134">The following is an example of the response.</span></span>

> <span data-ttu-id="6e20a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e20a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":2,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":3,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.332Z",
  "endDateTime": "2018-10-04T08:58:45.340Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T07:58:45.332Z",
  "code": "Break",
  "displayName": "Lunch"
  }
  ]
  },
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
