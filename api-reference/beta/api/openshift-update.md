---
title: 更新 openShift
description: 更新 openShift 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 821ad6579d7e77959263aab91511e71e0352e364
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867787"
---
# <a name="update-openshift"></a><span data-ttu-id="2158f-103">更新 openShift</span><span class="sxs-lookup"><span data-stu-id="2158f-103">Update openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2158f-104">更新[openShift](../resources/openshift.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2158f-104">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2158f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2158f-105">Permissions</span></span>

<span data-ttu-id="2158f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2158f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2158f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2158f-108">Permission type</span></span>                        | <span data-ttu-id="2158f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2158f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2158f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2158f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2158f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2158f-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2158f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2158f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2158f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2158f-113">Not supported.</span></span> |
| <span data-ttu-id="2158f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2158f-114">Application</span></span>                            | <span data-ttu-id="2158f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2158f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2158f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2158f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/openShifts
```

## <a name="request-headers"></a><span data-ttu-id="2158f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2158f-117">Request headers</span></span>

| <span data-ttu-id="2158f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2158f-118">Name</span></span>       | <span data-ttu-id="2158f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2158f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2158f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2158f-120">Authorization</span></span> | <span data-ttu-id="2158f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2158f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2158f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="2158f-123">Content-type</span></span> | <span data-ttu-id="2158f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2158f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2158f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2158f-126">Request body</span></span>

<span data-ttu-id="2158f-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2158f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2158f-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2158f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2158f-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2158f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2158f-130">属性</span><span class="sxs-lookup"><span data-stu-id="2158f-130">Property</span></span>     | <span data-ttu-id="2158f-131">类型</span><span class="sxs-lookup"><span data-stu-id="2158f-131">Type</span></span>        | <span data-ttu-id="2158f-132">说明</span><span class="sxs-lookup"><span data-stu-id="2158f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2158f-133">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="2158f-133">draftOpenShift</span></span>|<span data-ttu-id="2158f-134">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="2158f-134">openShiftItem</span></span>|<span data-ttu-id="2158f-135">未发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="2158f-135">An unpublished open shift.</span></span>|
|<span data-ttu-id="2158f-136">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="2158f-136">schedulingGroupId</span></span>|<span data-ttu-id="2158f-137">String</span><span class="sxs-lookup"><span data-stu-id="2158f-137">String</span></span>| <span data-ttu-id="2158f-138">计划组 id。</span><span class="sxs-lookup"><span data-stu-id="2158f-138">Scheduling group id.</span></span> |
|<span data-ttu-id="2158f-139">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="2158f-139">sharedOpenShift</span></span>|<span data-ttu-id="2158f-140">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="2158f-140">openShiftItem</span></span>|<span data-ttu-id="2158f-141">已发布的打开班次。</span><span class="sxs-lookup"><span data-stu-id="2158f-141">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="2158f-142">响应</span><span class="sxs-lookup"><span data-stu-id="2158f-142">Response</span></span>

<span data-ttu-id="2158f-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2158f-143">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2158f-144">示例</span><span class="sxs-lookup"><span data-stu-id="2158f-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2158f-145">请求</span><span class="sxs-lookup"><span data-stu-id="2158f-145">Request</span></span>

<span data-ttu-id="2158f-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2158f-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2158f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2158f-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2158f-148">C#</span><span class="sxs-lookup"><span data-stu-id="2158f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2158f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2158f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2158f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2158f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2158f-151">响应</span><span class="sxs-lookup"><span data-stu-id="2158f-151">Response</span></span>

<span data-ttu-id="2158f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2158f-152">The following is an example of the response.</span></span>

> <span data-ttu-id="2158f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2158f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
