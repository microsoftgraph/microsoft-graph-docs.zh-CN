---
title: 创建 openShift
description: 创建 openShift 对象的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 44f9918b5a7a91b2a16f32f6c8c3970b003a5583
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155080"
---
# <a name="create-openshift"></a><span data-ttu-id="d31e6-103">创建 openShift</span><span class="sxs-lookup"><span data-stu-id="d31e6-103">Create openShift</span></span>

<span data-ttu-id="d31e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d31e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d31e6-105">创建[openShift](../resources/openshift.md)对象的实例。</span><span class="sxs-lookup"><span data-stu-id="d31e6-105">Create an instance of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d31e6-106">权限</span><span class="sxs-lookup"><span data-stu-id="d31e6-106">Permissions</span></span>

<span data-ttu-id="d31e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d31e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d31e6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d31e6-109">Permission type</span></span>                        | <span data-ttu-id="d31e6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d31e6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d31e6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d31e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d31e6-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="d31e6-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d31e6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d31e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d31e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d31e6-114">Not supported.</span></span> |
| <span data-ttu-id="d31e6-115">Application</span><span class="sxs-lookup"><span data-stu-id="d31e6-115">Application</span></span>                            | <span data-ttu-id="d31e6-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d31e6-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="d31e6-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="d31e6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d31e6-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="d31e6-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d31e6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d31e6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShifts
```
  
## <a name="request-headers"></a><span data-ttu-id="d31e6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d31e6-120">Request headers</span></span>

| <span data-ttu-id="d31e6-121">名称</span><span class="sxs-lookup"><span data-stu-id="d31e6-121">Name</span></span>      |<span data-ttu-id="d31e6-122">说明</span><span class="sxs-lookup"><span data-stu-id="d31e6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d31e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d31e6-123">Authorization</span></span> | <span data-ttu-id="d31e6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d31e6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d31e6-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d31e6-126">Content-type</span></span> | <span data-ttu-id="d31e6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d31e6-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d31e6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d31e6-129">Request body</span></span>

<span data-ttu-id="d31e6-130">在此方法的请求正文中提供新的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d31e6-130">Provide the new [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d31e6-131">响应</span><span class="sxs-lookup"><span data-stu-id="d31e6-131">Response</span></span>

<span data-ttu-id="d31e6-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和创建的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d31e6-132">If successful, this method returns a `200 OK` response code and the created [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d31e6-133">示例</span><span class="sxs-lookup"><span data-stu-id="d31e6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d31e6-134">请求</span><span class="sxs-lookup"><span data-stu-id="d31e6-134">Request</span></span>

<span data-ttu-id="d31e6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d31e6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/openshifts
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
   "draftOpenShift":null,
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

### <a name="response"></a><span data-ttu-id="d31e6-136">响应</span><span class="sxs-lookup"><span data-stu-id="d31e6-136">Response</span></span>

<span data-ttu-id="d31e6-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d31e6-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d31e6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d31e6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "draftOpenShift": null,
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
