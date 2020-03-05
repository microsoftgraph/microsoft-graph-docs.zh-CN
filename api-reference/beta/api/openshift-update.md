---
title: 更新 openShift
description: 更新 openShift 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0b9c38e5be9e4f55d8d1b71460cf6735c73d5478
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456407"
---
# <a name="update-openshift"></a><span data-ttu-id="529c3-103">更新 openShift</span><span class="sxs-lookup"><span data-stu-id="529c3-103">Update openShift</span></span>

<span data-ttu-id="529c3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="529c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="529c3-105">更新[openShift](../resources/openshift.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="529c3-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="529c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="529c3-106">Permissions</span></span>

<span data-ttu-id="529c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="529c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="529c3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="529c3-109">Permission type</span></span>                        | <span data-ttu-id="529c3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="529c3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="529c3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="529c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="529c3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529c3-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="529c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="529c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="529c3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="529c3-114">Not supported.</span></span> |
| <span data-ttu-id="529c3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="529c3-115">Application</span></span>                            | <span data-ttu-id="529c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="529c3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="529c3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="529c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="529c3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="529c3-118">Request headers</span></span>

| <span data-ttu-id="529c3-119">名称</span><span class="sxs-lookup"><span data-stu-id="529c3-119">Name</span></span>       | <span data-ttu-id="529c3-120">说明</span><span class="sxs-lookup"><span data-stu-id="529c3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="529c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="529c3-121">Authorization</span></span> | <span data-ttu-id="529c3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="529c3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="529c3-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="529c3-124">Content-type</span></span> | <span data-ttu-id="529c3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="529c3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="529c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="529c3-127">Request body</span></span>

<span data-ttu-id="529c3-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="529c3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="529c3-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="529c3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="529c3-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="529c3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="529c3-131">属性</span><span class="sxs-lookup"><span data-stu-id="529c3-131">Property</span></span>     | <span data-ttu-id="529c3-132">类型</span><span class="sxs-lookup"><span data-stu-id="529c3-132">Type</span></span>        | <span data-ttu-id="529c3-133">说明</span><span class="sxs-lookup"><span data-stu-id="529c3-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="529c3-134">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="529c3-134">draftOpenShift</span></span>|<span data-ttu-id="529c3-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="529c3-135">openShiftItem</span></span>|<span data-ttu-id="529c3-136">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="529c3-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="529c3-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="529c3-137">schedulingGroupId</span></span>|<span data-ttu-id="529c3-138">String</span><span class="sxs-lookup"><span data-stu-id="529c3-138">String</span></span>| <span data-ttu-id="529c3-139">计划组 id。</span><span class="sxs-lookup"><span data-stu-id="529c3-139">Scheduling group id.</span></span> |
|<span data-ttu-id="529c3-140">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="529c3-140">sharedOpenShift</span></span>|<span data-ttu-id="529c3-141">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="529c3-141">openShiftItem</span></span>|<span data-ttu-id="529c3-142">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="529c3-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="529c3-143">响应</span><span class="sxs-lookup"><span data-stu-id="529c3-143">Response</span></span>

<span data-ttu-id="529c3-144">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="529c3-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="529c3-145">示例</span><span class="sxs-lookup"><span data-stu-id="529c3-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="529c3-146">请求</span><span class="sxs-lookup"><span data-stu-id="529c3-146">Request</span></span>

<span data-ttu-id="529c3-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="529c3-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="529c3-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="529c3-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
Content-type: application/json

{
"schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
"sharedOpenShift": {
"notes": "Inventory Management",
"openSlotCount":5,
"displayName": "Field shift",
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
"draftOpenShift": null
}
```
# <a name="c"></a>[<span data-ttu-id="529c3-149">C#</span><span class="sxs-lookup"><span data-stu-id="529c3-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="529c3-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="529c3-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="529c3-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="529c3-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="529c3-152">响应</span><span class="sxs-lookup"><span data-stu-id="529c3-152">Response</span></span>

<span data-ttu-id="529c3-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="529c3-153">The following is an example of the response.</span></span>

> <span data-ttu-id="529c3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="529c3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "openSlotCount":5,
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
  "description": "Update openshift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
