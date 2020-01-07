---
title: 创建 openShift
description: 创建 openshift 对象的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 635dd4c81e0b7f6cbe0cd2ceb26e391f2fb3bac5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952221"
---
# <a name="create-openshift"></a><span data-ttu-id="d83f5-103">创建 openShift</span><span class="sxs-lookup"><span data-stu-id="d83f5-103">Create openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d83f5-104">创建[openshift](../resources/openshift.md)对象的实例。</span><span class="sxs-lookup"><span data-stu-id="d83f5-104">Create an instance of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d83f5-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="d83f5-105">Permissions</span></span>

<span data-ttu-id="d83f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d83f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d83f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d83f5-108">Permission type</span></span>                        | <span data-ttu-id="d83f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d83f5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d83f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d83f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d83f5-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83f5-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d83f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d83f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d83f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d83f5-113">Not supported.</span></span> |
| <span data-ttu-id="d83f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d83f5-114">Application</span></span>                            | <span data-ttu-id="d83f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d83f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d83f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d83f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d83f5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d83f5-117">Optional query parameters</span></span>

<span data-ttu-id="d83f5-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d83f5-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d83f5-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d83f5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>
  
## <a name="request-headers"></a><span data-ttu-id="d83f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d83f5-120">Request headers</span></span>

| <span data-ttu-id="d83f5-121">名称</span><span class="sxs-lookup"><span data-stu-id="d83f5-121">Name</span></span>      |<span data-ttu-id="d83f5-122">说明</span><span class="sxs-lookup"><span data-stu-id="d83f5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d83f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d83f5-123">Authorization</span></span> | <span data-ttu-id="d83f5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d83f5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d83f5-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d83f5-126">Content-type</span></span> | <span data-ttu-id="d83f5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d83f5-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d83f5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d83f5-129">Request body</span></span>

<span data-ttu-id="d83f5-130">在此方法的请求正文中提供新的[openshift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d83f5-130">Provide the new [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d83f5-131">响应</span><span class="sxs-lookup"><span data-stu-id="d83f5-131">Response</span></span>

<span data-ttu-id="d83f5-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d83f5-132">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d83f5-133">示例</span><span class="sxs-lookup"><span data-stu-id="d83f5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d83f5-134">请求</span><span class="sxs-lookup"><span data-stu-id="d83f5-134">Request</span></span>

<span data-ttu-id="d83f5-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d83f5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
Authorization: Bearer {token}
Content-type: application/json
Content-length: 244

{
   "id":"OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
   "schedulingGroupId":"TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
   "sharedOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":2,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.340Z",
      "endDateTime":"2018-10-04T09: 50: 45.332Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T01: 58: 45.340Z",
            "code":"",
            "displayName":"Lunch"
         }
      ]
   },
   "draftOpenShift":{
      "notes":"InventoryManagement",
      "openSlotCount":3,
      "displayName":"Dayshift",
      "startDateTime":"2018-10-04T00: 58: 45.332Z",
      "endDateTime":"2018-10-04T08: 58: 45.340Z",
      "theme":"white",
      "activities":[
         {
            "isPaid":true,
            "startDateTime":"2018-10-04T00: 58: 45.340Z",
            "endDateTime":"2018-10-04T07: 58: 45.332Z",
            "code":"Break",
            "displayName":"Lunch"
         }
      ]
   },
   "createdDateTime":"2019-03-14T04: 32: 51.451Z",
   "lastModifiedDateTime":"2019-03-14T05: 32: 51.451Z",
   "lastModifiedBy":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
         "displayName":"JohnDoe"
      }
   }
}
```

### <a name="response"></a><span data-ttu-id="d83f5-136">响应</span><span class="sxs-lookup"><span data-stu-id="d83f5-136">Response</span></span>

<span data-ttu-id="d83f5-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d83f5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d83f5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d83f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
