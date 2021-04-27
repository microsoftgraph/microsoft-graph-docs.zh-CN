---
title: 更新工作人员重新参与
description: 更新 workforceintegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2da287f8b78beae39ce5842307c08ff15ef78007
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054677"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="287ec-103">更新工作人员重新参与</span><span class="sxs-lookup"><span data-stu-id="287ec-103">Update workforceintegration</span></span>

<span data-ttu-id="287ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="287ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="287ec-105">更新 [workforceintegration 对象](../resources/workforceintegration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="287ec-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="287ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="287ec-106">Permissions</span></span>

<span data-ttu-id="287ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="287ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="287ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="287ec-109">Permission type</span></span>                        | <span data-ttu-id="287ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="287ec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="287ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="287ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="287ec-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="287ec-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="287ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="287ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="287ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="287ec-114">Not supported.</span></span> |
| <span data-ttu-id="287ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="287ec-115">Application</span></span>                            | <span data-ttu-id="287ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="287ec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="287ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="287ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="287ec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="287ec-118">Request headers</span></span>

| <span data-ttu-id="287ec-119">名称</span><span class="sxs-lookup"><span data-stu-id="287ec-119">Name</span></span>       | <span data-ttu-id="287ec-120">说明</span><span class="sxs-lookup"><span data-stu-id="287ec-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="287ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="287ec-121">Authorization</span></span> | <span data-ttu-id="287ec-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="287ec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="287ec-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="287ec-123">Request body</span></span>

<span data-ttu-id="287ec-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="287ec-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="287ec-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="287ec-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="287ec-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="287ec-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="287ec-127">属性</span><span class="sxs-lookup"><span data-stu-id="287ec-127">Property</span></span>     | <span data-ttu-id="287ec-128">类型</span><span class="sxs-lookup"><span data-stu-id="287ec-128">Type</span></span>        | <span data-ttu-id="287ec-129">说明</span><span class="sxs-lookup"><span data-stu-id="287ec-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="287ec-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="287ec-130">apiVersion</span></span>|<span data-ttu-id="287ec-131">Int32</span><span class="sxs-lookup"><span data-stu-id="287ec-131">Int32</span></span>|<span data-ttu-id="287ec-132">用于回叫 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="287ec-132">API version for the call back url.</span></span> <span data-ttu-id="287ec-133">从 1 开始。</span><span class="sxs-lookup"><span data-stu-id="287ec-133">Start with 1.</span></span>|
|<span data-ttu-id="287ec-134">displayName</span><span class="sxs-lookup"><span data-stu-id="287ec-134">displayName</span></span>|<span data-ttu-id="287ec-135">String</span><span class="sxs-lookup"><span data-stu-id="287ec-135">String</span></span>|<span data-ttu-id="287ec-136">员工集成的名称。</span><span class="sxs-lookup"><span data-stu-id="287ec-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="287ec-137">加密</span><span class="sxs-lookup"><span data-stu-id="287ec-137">encryption</span></span>|<span data-ttu-id="287ec-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="287ec-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="287ec-139">员工集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="287ec-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="287ec-140">isActive</span><span class="sxs-lookup"><span data-stu-id="287ec-140">isActive</span></span>|<span data-ttu-id="287ec-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="287ec-141">Boolean</span></span>|<span data-ttu-id="287ec-142">指示此员工集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="287ec-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="287ec-143">支持</span><span class="sxs-lookup"><span data-stu-id="287ec-143">supports</span></span>|<span data-ttu-id="287ec-144">string</span><span class="sxs-lookup"><span data-stu-id="287ec-144">string</span></span>| <span data-ttu-id="287ec-145">可能的值是 `none` `shift` `swapRequest` 、、、、、。 `openshift` `openShiftRequest` `userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="287ec-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="287ec-146">如果选择多个值，则所有值必须以大写字母开头。</span><span class="sxs-lookup"><span data-stu-id="287ec-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="287ec-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="287ec-147">supportedEntities</span></span>|<span data-ttu-id="287ec-148">string</span><span class="sxs-lookup"><span data-stu-id="287ec-148">string</span></span>| <span data-ttu-id="287ec-149">此属性 **将替换** v1.0 中的 supports。</span><span class="sxs-lookup"><span data-stu-id="287ec-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="287ec-150">我们建议你使用此属性，而不是 **支持**。</span><span class="sxs-lookup"><span data-stu-id="287ec-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="287ec-151">**目前，supports** 属性在 beta 版中仍受支持。</span><span class="sxs-lookup"><span data-stu-id="287ec-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="287ec-152">可能的值是 `none` `shift` `swapRequest` 、、、、、。 `openshift` `openShiftRequest` `userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="287ec-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="287ec-153">如果选择多个值，则所有值必须以大写字母开头。</span><span class="sxs-lookup"><span data-stu-id="287ec-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="287ec-154">url</span><span class="sxs-lookup"><span data-stu-id="287ec-154">url</span></span>|<span data-ttu-id="287ec-155">String</span><span class="sxs-lookup"><span data-stu-id="287ec-155">String</span></span>| <span data-ttu-id="287ec-156">班次服务中回调的员工集成 URL。</span><span class="sxs-lookup"><span data-stu-id="287ec-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="287ec-157">响应</span><span class="sxs-lookup"><span data-stu-id="287ec-157">Response</span></span>

<span data-ttu-id="287ec-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="287ec-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="287ec-159">示例</span><span class="sxs-lookup"><span data-stu-id="287ec-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="287ec-160">示例 1：更新一个 workforceIntegration 对象</span><span class="sxs-lookup"><span data-stu-id="287ec-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="287ec-161">以下示例更新 **一个 workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="287ec-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="287ec-162">请求</span><span class="sxs-lookup"><span data-stu-id="287ec-162">Request</span></span>

<span data-ttu-id="287ec-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="287ec-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="287ec-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="287ec-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
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
# <a name="c"></a>[<span data-ttu-id="287ec-165">C#</span><span class="sxs-lookup"><span data-stu-id="287ec-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="287ec-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="287ec-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="287ec-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="287ec-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="287ec-168">Java</span><span class="sxs-lookup"><span data-stu-id="287ec-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="287ec-169">响应</span><span class="sxs-lookup"><span data-stu-id="287ec-169">Response</span></span>

<span data-ttu-id="287ec-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="287ec-170">The following is an example of the response.</span></span>

> <span data-ttu-id="287ec-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="287ec-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="287ec-172">示例 2：新建一个针对资格筛选启用 SwapRequest 的 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="287ec-172">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="287ec-173">以下示例创建一个新的 **workforceIntegration，** 并启用 SwapRequest 进行资格筛选。</span><span class="sxs-lookup"><span data-stu-id="287ec-173">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="287ec-174">请求</span><span class="sxs-lookup"><span data-stu-id="287ec-174">Request</span></span>

<span data-ttu-id="287ec-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="287ec-175">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a><span data-ttu-id="287ec-176">响应</span><span class="sxs-lookup"><span data-stu-id="287ec-176">Response</span></span>

<span data-ttu-id="287ec-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="287ec-177">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
<span data-ttu-id="287ec-178">若要创建新的 **workforceIntegration，** 并启用 SwapRequest 进行资格筛选，请参阅 [Create](../api/workforceintegration-post.md) 方法。</span><span class="sxs-lookup"><span data-stu-id="287ec-178">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="287ec-179">示例 3：在 SwapRequest 包含在 eligiblyFilteringEnabledEntities 中时提取符合条件的班次</span><span class="sxs-lookup"><span data-stu-id="287ec-179">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="287ec-180">班次应用和员工集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="287ec-180">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="287ec-181">请求</span><span class="sxs-lookup"><span data-stu-id="287ec-181">Request</span></span>

<span data-ttu-id="287ec-182">下面是 Shifts 向员工集成终结点请求获取交换请求的合格班次的示例。</span><span class="sxs-lookup"><span data-stu-id="287ec-182">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
#### <a name="response"></a><span data-ttu-id="287ec-183">响应</span><span class="sxs-lookup"><span data-stu-id="287ec-183">Response</span></span>

<span data-ttu-id="287ec-184">下面是员工集成服务的响应示例。</span><span class="sxs-lookup"><span data-stu-id="287ec-184">The following is an example of the response from the workforce integration service.</span></span>
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
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


