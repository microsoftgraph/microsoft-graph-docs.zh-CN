---
title: 更新 openShift
description: 更新 openShift 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5863b3a52eb195fed205788480cf1e5eda1237eb
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895609"
---
# <a name="update-openshift"></a><span data-ttu-id="5e0f5-103">更新 openShift</span><span class="sxs-lookup"><span data-stu-id="5e0f5-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e0f5-104">更新[openShift](../resources/openshift.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e0f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="5e0f5-105">Permissions</span></span>

<span data-ttu-id="5e0f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e0f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e0f5-108">Permission type</span></span>                        | <span data-ttu-id="5e0f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e0f5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5e0f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e0f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e0f5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e0f5-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5e0f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e0f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e0f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-113">Not supported.</span></span> |
| <span data-ttu-id="5e0f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e0f5-114">Application</span></span>                            | <span data-ttu-id="5e0f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e0f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e0f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="5e0f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e0f5-117">Request headers</span></span>

| <span data-ttu-id="5e0f5-118">名称</span><span class="sxs-lookup"><span data-stu-id="5e0f5-118">Name</span></span>       | <span data-ttu-id="5e0f5-119">说明</span><span class="sxs-lookup"><span data-stu-id="5e0f5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e0f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e0f5-120">Authorization</span></span> | <span data-ttu-id="5e0f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e0f5-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="5e0f5-123">Content-type</span></span> | <span data-ttu-id="5e0f5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5e0f5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e0f5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e0f5-126">Request body</span></span>

<span data-ttu-id="5e0f5-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5e0f5-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5e0f5-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e0f5-130">属性</span><span class="sxs-lookup"><span data-stu-id="5e0f5-130">Property</span></span>     | <span data-ttu-id="5e0f5-131">类型</span><span class="sxs-lookup"><span data-stu-id="5e0f5-131">Type</span></span>        | <span data-ttu-id="5e0f5-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e0f5-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e0f5-133">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="5e0f5-133">draftOpenShift</span></span>|<span data-ttu-id="5e0f5-134">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="5e0f5-134">openShiftItem</span></span>|<span data-ttu-id="5e0f5-135">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="5e0f5-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="5e0f5-136">schedulingGroupId</span></span>|<span data-ttu-id="5e0f5-137">字符串</span><span class="sxs-lookup"><span data-stu-id="5e0f5-137">String</span></span>| <span data-ttu-id="5e0f5-138">计划组 id。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-138">Scheduling group id.</span></span> |
|<span data-ttu-id="5e0f5-139">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="5e0f5-139">sharedOpenShift</span></span>|<span data-ttu-id="5e0f5-140">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="5e0f5-140">openShiftItem</span></span>|<span data-ttu-id="5e0f5-141">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="5e0f5-142">响应</span><span class="sxs-lookup"><span data-stu-id="5e0f5-142">Response</span></span>

<span data-ttu-id="5e0f5-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e0f5-144">示例</span><span class="sxs-lookup"><span data-stu-id="5e0f5-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e0f5-145">请求</span><span class="sxs-lookup"><span data-stu-id="5e0f5-145">Request</span></span>

<span data-ttu-id="5e0f5-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263"
}
```

### <a name="response"></a><span data-ttu-id="5e0f5-147">响应</span><span class="sxs-lookup"><span data-stu-id="5e0f5-147">Response</span></span>

<span data-ttu-id="5e0f5-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-148">The following is an example of the response.</span></span>

> <span data-ttu-id="5e0f5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e0f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "schedulingGroupId-value"
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
