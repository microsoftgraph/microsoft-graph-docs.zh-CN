---
title: 更新 workforceintegration
description: 更新 workforceintegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c87031c5d8957e4014f491f671c05b7a10b4934
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451264"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="b4ed6-103">更新 workforceintegration</span><span class="sxs-lookup"><span data-stu-id="b4ed6-103">Update workforceintegration</span></span>

<span data-ttu-id="b4ed6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b4ed6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ed6-105">更新[workforceintegration](../resources/workforceintegration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ed6-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4ed6-106">Permissions</span></span>

<span data-ttu-id="b4ed6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4ed6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4ed6-109">Permission type</span></span>                        | <span data-ttu-id="b4ed6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4ed6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="b4ed6-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b4ed6-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b4ed6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ed6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ed6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-114">Not supported.</span></span> |
| <span data-ttu-id="b4ed6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4ed6-115">Application</span></span>                            | <span data-ttu-id="b4ed6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ed6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4ed6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="b4ed6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4ed6-118">Request headers</span></span>

| <span data-ttu-id="b4ed6-119">名称</span><span class="sxs-lookup"><span data-stu-id="b4ed6-119">Name</span></span>       | <span data-ttu-id="b4ed6-120">说明</span><span class="sxs-lookup"><span data-stu-id="b4ed6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4ed6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ed6-121">Authorization</span></span> | <span data-ttu-id="b4ed6-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b4ed6-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ed6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4ed6-123">Request body</span></span>

<span data-ttu-id="b4ed6-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4ed6-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4ed6-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4ed6-127">属性</span><span class="sxs-lookup"><span data-stu-id="b4ed6-127">Property</span></span>     | <span data-ttu-id="b4ed6-128">类型</span><span class="sxs-lookup"><span data-stu-id="b4ed6-128">Type</span></span>        | <span data-ttu-id="b4ed6-129">说明</span><span class="sxs-lookup"><span data-stu-id="b4ed6-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4ed6-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="b4ed6-130">apiVersion</span></span>|<span data-ttu-id="b4ed6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b4ed6-131">Int32</span></span>|<span data-ttu-id="b4ed6-132">回调 url 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-132">API version for the call back url.</span></span> <span data-ttu-id="b4ed6-133">从1开始。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-133">Start with 1.</span></span>|
|<span data-ttu-id="b4ed6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b4ed6-134">displayName</span></span>|<span data-ttu-id="b4ed6-135">String</span><span class="sxs-lookup"><span data-stu-id="b4ed6-135">String</span></span>|<span data-ttu-id="b4ed6-136">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="b4ed6-137">技术</span><span class="sxs-lookup"><span data-stu-id="b4ed6-137">encryption</span></span>|<span data-ttu-id="b4ed6-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="b4ed6-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="b4ed6-139">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="b4ed6-140">isActive</span><span class="sxs-lookup"><span data-stu-id="b4ed6-140">isActive</span></span>|<span data-ttu-id="b4ed6-141">布尔</span><span class="sxs-lookup"><span data-stu-id="b4ed6-141">Boolean</span></span>|<span data-ttu-id="b4ed6-142">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="b4ed6-143">支持</span><span class="sxs-lookup"><span data-stu-id="b4ed6-143">supports</span></span>|<span data-ttu-id="b4ed6-144">string</span><span class="sxs-lookup"><span data-stu-id="b4ed6-144">string</span></span>| <span data-ttu-id="b4ed6-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="b4ed6-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="b4ed6-146">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="b4ed6-147">url</span><span class="sxs-lookup"><span data-stu-id="b4ed6-147">url</span></span>|<span data-ttu-id="b4ed6-148">String</span><span class="sxs-lookup"><span data-stu-id="b4ed6-148">String</span></span>| <span data-ttu-id="b4ed6-149">劳动力集成 url，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-149">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="b4ed6-150">响应</span><span class="sxs-lookup"><span data-stu-id="b4ed6-150">Response</span></span>

<span data-ttu-id="b4ed6-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-151">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4ed6-152">示例</span><span class="sxs-lookup"><span data-stu-id="b4ed6-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4ed6-153">请求</span><span class="sxs-lookup"><span data-stu-id="b4ed6-153">Request</span></span>

<span data-ttu-id="b4ed6-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4ed6-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ed6-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b4ed6-156">C#</span><span class="sxs-lookup"><span data-stu-id="b4ed6-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4ed6-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ed6-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4ed6-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4ed6-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4ed6-159">响应</span><span class="sxs-lookup"><span data-stu-id="b4ed6-159">Response</span></span>

<span data-ttu-id="b4ed6-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-160">The following is an example of the response.</span></span>

> <span data-ttu-id="b4ed6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4ed6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
