---
title: 更新 swapShiftsChangeRequest
description: 更新 swapShiftsChangeRequest 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0955428ce82f585bbdb085e0d6d2f2f6023f92f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870786"
---
# <a name="update-swapshiftschangerequest"></a><span data-ttu-id="28a33-103">更新 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="28a33-103">Update swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28a33-104">更新[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28a33-104">Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28a33-105">权限</span><span class="sxs-lookup"><span data-stu-id="28a33-105">Permissions</span></span>

<span data-ttu-id="28a33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28a33-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="28a33-108">Permission type</span></span>                        | <span data-ttu-id="28a33-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28a33-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="28a33-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28a33-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="28a33-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28a33-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="28a33-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28a33-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28a33-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="28a33-113">Not supported.</span></span> |
|<span data-ttu-id="28a33-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="28a33-114">Application</span></span> | <span data-ttu-id="28a33-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="28a33-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="28a33-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="28a33-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="28a33-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28a33-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="28a33-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="28a33-118">Request headers</span></span>

| <span data-ttu-id="28a33-119">名称</span><span class="sxs-lookup"><span data-stu-id="28a33-119">Name</span></span>       | <span data-ttu-id="28a33-120">说明</span><span class="sxs-lookup"><span data-stu-id="28a33-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28a33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28a33-121">Authorization</span></span> | <span data-ttu-id="28a33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28a33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28a33-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="28a33-124">Content-type</span></span> | <span data-ttu-id="28a33-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="28a33-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28a33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28a33-127">Request body</span></span>

<span data-ttu-id="28a33-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="28a33-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="28a33-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="28a33-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="28a33-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="28a33-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28a33-131">属性</span><span class="sxs-lookup"><span data-stu-id="28a33-131">Property</span></span>     | <span data-ttu-id="28a33-132">类型</span><span class="sxs-lookup"><span data-stu-id="28a33-132">Type</span></span>        | <span data-ttu-id="28a33-133">说明</span><span class="sxs-lookup"><span data-stu-id="28a33-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28a33-134">recipientShiftId</span><span class="sxs-lookup"><span data-stu-id="28a33-134">recipientShiftId</span></span>|<span data-ttu-id="28a33-135">String</span><span class="sxs-lookup"><span data-stu-id="28a33-135">String</span></span>|<span data-ttu-id="28a33-136">交换请求的收件人的 ID。</span><span class="sxs-lookup"><span data-stu-id="28a33-136">The ID of the recipient of the swap request.</span></span> <span data-ttu-id="28a33-137">这是请求与之交换的用户。</span><span class="sxs-lookup"><span data-stu-id="28a33-137">This is the user who is requested to swap with.</span></span>|

## <a name="response"></a><span data-ttu-id="28a33-138">响应</span><span class="sxs-lookup"><span data-stu-id="28a33-138">Response</span></span>

<span data-ttu-id="28a33-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28a33-139">If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28a33-140">示例</span><span class="sxs-lookup"><span data-stu-id="28a33-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28a33-141">请求</span><span class="sxs-lookup"><span data-stu-id="28a33-141">Request</span></span>

<span data-ttu-id="28a33-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28a33-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28a33-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="28a33-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_swapshiftschangerequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28a33-144">C#</span><span class="sxs-lookup"><span data-stu-id="28a33-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28a33-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28a33-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28a33-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28a33-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28a33-147">响应</span><span class="sxs-lookup"><span data-stu-id="28a33-147">Response</span></span>

<span data-ttu-id="28a33-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28a33-148">The following is an example of the response.</span></span>

> <span data-ttu-id="28a33-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28a33-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update swapshiftschangerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
