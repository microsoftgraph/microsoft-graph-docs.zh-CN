---
title: 获取 openShift
description: 检索 openshift 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ef3b1681ed6a155cf59bc3276cc041969b2d580
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153518"
---
# <a name="get-openshift"></a><span data-ttu-id="bd36f-103">获取 openShift</span><span class="sxs-lookup"><span data-stu-id="bd36f-103">Get openShift</span></span>

<span data-ttu-id="bd36f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd36f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd36f-105">检索[openshift](../resources/openshift.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd36f-105">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd36f-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd36f-106">Permissions</span></span>

<span data-ttu-id="bd36f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd36f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd36f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd36f-109">Permission type</span></span>                        | <span data-ttu-id="bd36f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd36f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd36f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd36f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd36f-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd36f-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bd36f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd36f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd36f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd36f-114">Not supported.</span></span> |
| <span data-ttu-id="bd36f-115">Application</span><span class="sxs-lookup"><span data-stu-id="bd36f-115">Application</span></span>                            | <span data-ttu-id="bd36f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd36f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd36f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd36f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd36f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bd36f-118">Optional query parameters</span></span>

<span data-ttu-id="bd36f-119">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd36f-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd36f-120">请求头</span><span class="sxs-lookup"><span data-stu-id="bd36f-120">Request headers</span></span>

| <span data-ttu-id="bd36f-121">名称</span><span class="sxs-lookup"><span data-stu-id="bd36f-121">Name</span></span>      |<span data-ttu-id="bd36f-122">说明</span><span class="sxs-lookup"><span data-stu-id="bd36f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd36f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd36f-123">Authorization</span></span> | <span data-ttu-id="bd36f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd36f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd36f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd36f-126">Request body</span></span>

<span data-ttu-id="bd36f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd36f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd36f-128">响应</span><span class="sxs-lookup"><span data-stu-id="bd36f-128">Response</span></span>

<span data-ttu-id="bd36f-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd36f-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd36f-130">示例</span><span class="sxs-lookup"><span data-stu-id="bd36f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd36f-131">请求</span><span class="sxs-lookup"><span data-stu-id="bd36f-131">Request</span></span>

<span data-ttu-id="bd36f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd36f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd36f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd36f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="bd36f-134">C#</span><span class="sxs-lookup"><span data-stu-id="bd36f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd36f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd36f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd36f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd36f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd36f-137">响应</span><span class="sxs-lookup"><span data-stu-id="bd36f-137">Response</span></span>

<span data-ttu-id="bd36f-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd36f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="bd36f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd36f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
