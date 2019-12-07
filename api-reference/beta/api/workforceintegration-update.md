---
title: 更新 workforceintegration
description: 更新 workforceintegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1aa2afb19f380a07d147e82fe37a10304dc097be
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895582"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="f366d-103">更新 workforceintegration</span><span class="sxs-lookup"><span data-stu-id="f366d-103">Update workforceintegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f366d-104">更新[workforceintegration](../resources/workforceintegration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f366d-104">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f366d-105">权限</span><span class="sxs-lookup"><span data-stu-id="f366d-105">Permissions</span></span>

<span data-ttu-id="f366d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f366d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f366d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f366d-108">Permission type</span></span>                        | <span data-ttu-id="f366d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f366d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f366d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f366d-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="f366d-111">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="f366d-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f366d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f366d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f366d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f366d-113">Not supported.</span></span> |
| <span data-ttu-id="f366d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f366d-114">Application</span></span>                            | <span data-ttu-id="f366d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f366d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f366d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f366d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="f366d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f366d-117">Request headers</span></span>

| <span data-ttu-id="f366d-118">名称</span><span class="sxs-lookup"><span data-stu-id="f366d-118">Name</span></span>       | <span data-ttu-id="f366d-119">说明</span><span class="sxs-lookup"><span data-stu-id="f366d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f366d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f366d-120">Authorization</span></span> | <span data-ttu-id="f366d-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f366d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f366d-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="f366d-122">Request body</span></span>

<span data-ttu-id="f366d-123">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f366d-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f366d-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f366d-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f366d-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f366d-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f366d-126">属性</span><span class="sxs-lookup"><span data-stu-id="f366d-126">Property</span></span>     | <span data-ttu-id="f366d-127">类型</span><span class="sxs-lookup"><span data-stu-id="f366d-127">Type</span></span>        | <span data-ttu-id="f366d-128">说明</span><span class="sxs-lookup"><span data-stu-id="f366d-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f366d-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="f366d-129">apiVersion</span></span>|<span data-ttu-id="f366d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f366d-130">Int32</span></span>|<span data-ttu-id="f366d-131">回调 url 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="f366d-131">API version for the call back url.</span></span> <span data-ttu-id="f366d-132">从1开始。</span><span class="sxs-lookup"><span data-stu-id="f366d-132">Start with 1.</span></span>|
|<span data-ttu-id="f366d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f366d-133">displayName</span></span>|<span data-ttu-id="f366d-134">String</span><span class="sxs-lookup"><span data-stu-id="f366d-134">String</span></span>|<span data-ttu-id="f366d-135">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="f366d-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="f366d-136">技术</span><span class="sxs-lookup"><span data-stu-id="f366d-136">encryption</span></span>|<span data-ttu-id="f366d-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="f366d-137">workforceIntegrationEncryption</span></span>|<span data-ttu-id="f366d-138">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="f366d-138">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="f366d-139">isActive</span><span class="sxs-lookup"><span data-stu-id="f366d-139">isActive</span></span>|<span data-ttu-id="f366d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f366d-140">Boolean</span></span>|<span data-ttu-id="f366d-141">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="f366d-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="f366d-142">支持</span><span class="sxs-lookup"><span data-stu-id="f366d-142">supports</span></span>|<span data-ttu-id="f366d-143">string</span><span class="sxs-lookup"><span data-stu-id="f366d-143">string</span></span>| <span data-ttu-id="f366d-144">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="f366d-144"></span></span> <span data-ttu-id="f366d-145">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="f366d-145">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="f366d-146">url</span><span class="sxs-lookup"><span data-stu-id="f366d-146">url</span></span>|<span data-ttu-id="f366d-147">String</span><span class="sxs-lookup"><span data-stu-id="f366d-147">String</span></span>| <span data-ttu-id="f366d-148">劳动力集成 url，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="f366d-148">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="f366d-149">响应</span><span class="sxs-lookup"><span data-stu-id="f366d-149">Response</span></span>

<span data-ttu-id="f366d-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f366d-150">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f366d-151">示例</span><span class="sxs-lookup"><span data-stu-id="f366d-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f366d-152">请求</span><span class="sxs-lookup"><span data-stu-id="f366d-152">Request</span></span>

<span data-ttu-id="f366d-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f366d-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f366d-154">响应</span><span class="sxs-lookup"><span data-stu-id="f366d-154">Response</span></span>

<span data-ttu-id="f366d-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f366d-155">The following is an example of the response.</span></span>

> <span data-ttu-id="f366d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f366d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
