---
title: 更新 openShift
description: 更新 openShift 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 71b6dc24bb4eb6426e5b15ca7c4147ae77ff1457
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032934"
---
# <a name="update-openshift"></a><span data-ttu-id="d9294-103">更新 openShift</span><span class="sxs-lookup"><span data-stu-id="d9294-103">Update openShift</span></span>

<span data-ttu-id="d9294-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9294-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9294-105">更新 [openShift](../resources/openshift.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9294-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9294-106">权限</span><span class="sxs-lookup"><span data-stu-id="d9294-106">Permissions</span></span>

<span data-ttu-id="d9294-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9294-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9294-109">Permission type</span></span>                        | <span data-ttu-id="d9294-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9294-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9294-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9294-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9294-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="d9294-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d9294-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9294-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9294-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9294-114">Not supported.</span></span> |
| <span data-ttu-id="d9294-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9294-115">Application</span></span>                            | <span data-ttu-id="d9294-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9294-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="d9294-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="d9294-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d9294-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="d9294-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9294-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9294-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="d9294-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9294-120">Request headers</span></span>

| <span data-ttu-id="d9294-121">名称</span><span class="sxs-lookup"><span data-stu-id="d9294-121">Name</span></span>       | <span data-ttu-id="d9294-122">说明</span><span class="sxs-lookup"><span data-stu-id="d9294-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d9294-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9294-123">Authorization</span></span> | <span data-ttu-id="d9294-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9294-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9294-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d9294-126">Content-type</span></span> | <span data-ttu-id="d9294-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d9294-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9294-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9294-129">Request body</span></span>

<span data-ttu-id="d9294-130">在此方法的请求正文中提供修改的 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9294-130">Provide the modified [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="d9294-131">属性</span><span class="sxs-lookup"><span data-stu-id="d9294-131">Property</span></span>     | <span data-ttu-id="d9294-132">类型</span><span class="sxs-lookup"><span data-stu-id="d9294-132">Type</span></span>        | <span data-ttu-id="d9294-133">说明</span><span class="sxs-lookup"><span data-stu-id="d9294-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9294-134">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="d9294-134">draftOpenShift</span></span>|<span data-ttu-id="d9294-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="d9294-135">openShiftItem</span></span>|<span data-ttu-id="d9294-136">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="d9294-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="d9294-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="d9294-137">schedulingGroupId</span></span>|<span data-ttu-id="d9294-138">String</span><span class="sxs-lookup"><span data-stu-id="d9294-138">String</span></span>| <span data-ttu-id="d9294-139">计划组 ID。</span><span class="sxs-lookup"><span data-stu-id="d9294-139">Scheduling group ID.</span></span> |
|<span data-ttu-id="d9294-140">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="d9294-140">sharedOpenShift</span></span>|<span data-ttu-id="d9294-141">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="d9294-141">openShiftItem</span></span>|<span data-ttu-id="d9294-142">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="d9294-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="d9294-143">响应</span><span class="sxs-lookup"><span data-stu-id="d9294-143">Response</span></span>

<span data-ttu-id="d9294-144">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [openShift](../resources/openshift.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9294-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9294-145">示例</span><span class="sxs-lookup"><span data-stu-id="d9294-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9294-146">请求</span><span class="sxs-lookup"><span data-stu-id="d9294-146">Request</span></span>

<span data-ttu-id="d9294-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9294-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9294-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9294-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
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
# <a name="c"></a>[<span data-ttu-id="d9294-149">C#</span><span class="sxs-lookup"><span data-stu-id="d9294-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9294-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9294-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9294-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9294-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9294-152">Java</span><span class="sxs-lookup"><span data-stu-id="d9294-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="d9294-153">响应</span><span class="sxs-lookup"><span data-stu-id="d9294-153">Response</span></span>

<span data-ttu-id="d9294-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9294-154">The following is an example of the response.</span></span>

> <span data-ttu-id="d9294-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9294-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

