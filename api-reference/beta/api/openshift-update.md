---
title: 更新 openShift
description: 更新 openShift 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c17e56fb6fe0f6eb963d30beb35dc867955cea3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976882"
---
# <a name="update-openshift"></a><span data-ttu-id="ee14e-103">更新 openShift</span><span class="sxs-lookup"><span data-stu-id="ee14e-103">Update openShift</span></span>

<span data-ttu-id="ee14e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee14e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee14e-105">更新 [openShift](../resources/openshift.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ee14e-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee14e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee14e-106">Permissions</span></span>

<span data-ttu-id="ee14e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee14e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee14e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee14e-109">Permission type</span></span>                        | <span data-ttu-id="ee14e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee14e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ee14e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee14e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee14e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee14e-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ee14e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee14e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee14e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee14e-114">Not supported.</span></span> |
| <span data-ttu-id="ee14e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee14e-115">Application</span></span>                            | <span data-ttu-id="ee14e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee14e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee14e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee14e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="ee14e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee14e-118">Request headers</span></span>

| <span data-ttu-id="ee14e-119">名称</span><span class="sxs-lookup"><span data-stu-id="ee14e-119">Name</span></span>       | <span data-ttu-id="ee14e-120">说明</span><span class="sxs-lookup"><span data-stu-id="ee14e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ee14e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee14e-121">Authorization</span></span> | <span data-ttu-id="ee14e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee14e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee14e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ee14e-124">Content-type</span></span> | <span data-ttu-id="ee14e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ee14e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee14e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee14e-127">Request body</span></span>

<span data-ttu-id="ee14e-128">在此方法的请求正文中提供修改的 [openshift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee14e-128">Provide the modified [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="ee14e-129">属性</span><span class="sxs-lookup"><span data-stu-id="ee14e-129">Property</span></span>     | <span data-ttu-id="ee14e-130">类型</span><span class="sxs-lookup"><span data-stu-id="ee14e-130">Type</span></span>        | <span data-ttu-id="ee14e-131">说明</span><span class="sxs-lookup"><span data-stu-id="ee14e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee14e-132">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="ee14e-132">draftOpenShift</span></span>|<span data-ttu-id="ee14e-133">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ee14e-133">openShiftItem</span></span>|<span data-ttu-id="ee14e-134">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ee14e-134">An unpublished open shift.</span></span>|
|<span data-ttu-id="ee14e-135">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="ee14e-135">schedulingGroupId</span></span>|<span data-ttu-id="ee14e-136">String</span><span class="sxs-lookup"><span data-stu-id="ee14e-136">String</span></span>| <span data-ttu-id="ee14e-137">计划组 id。</span><span class="sxs-lookup"><span data-stu-id="ee14e-137">Scheduling group id.</span></span> |
|<span data-ttu-id="ee14e-138">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="ee14e-138">sharedOpenShift</span></span>|<span data-ttu-id="ee14e-139">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="ee14e-139">openShiftItem</span></span>|<span data-ttu-id="ee14e-140">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="ee14e-140">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="ee14e-141">响应</span><span class="sxs-lookup"><span data-stu-id="ee14e-141">Response</span></span>

<span data-ttu-id="ee14e-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee14e-142">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee14e-143">示例</span><span class="sxs-lookup"><span data-stu-id="ee14e-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee14e-144">请求</span><span class="sxs-lookup"><span data-stu-id="ee14e-144">Request</span></span>

<span data-ttu-id="ee14e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee14e-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee14e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee14e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
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
# <a name="c"></a>[<span data-ttu-id="ee14e-147">C#</span><span class="sxs-lookup"><span data-stu-id="ee14e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee14e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee14e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee14e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee14e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee14e-150">Java</span><span class="sxs-lookup"><span data-stu-id="ee14e-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee14e-151">响应</span><span class="sxs-lookup"><span data-stu-id="ee14e-151">Response</span></span>

<span data-ttu-id="ee14e-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee14e-152">The following is an example of the response.</span></span>

> <span data-ttu-id="ee14e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ee14e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


