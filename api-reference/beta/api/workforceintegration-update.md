---
title: 更新 workforceintegration
description: 更新 workforceintegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e1f7c6486e42ecc2f41604866eef9dd7d069651
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970540"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="cb381-103">更新 workforceintegration</span><span class="sxs-lookup"><span data-stu-id="cb381-103">Update workforceintegration</span></span>

<span data-ttu-id="cb381-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb381-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb381-105">更新 [workforceintegration](../resources/workforceintegration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb381-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb381-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb381-106">Permissions</span></span>

<span data-ttu-id="cb381-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb381-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb381-109">Permission type</span></span>                        | <span data-ttu-id="cb381-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb381-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb381-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb381-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb381-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="cb381-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="cb381-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb381-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb381-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb381-114">Not supported.</span></span> |
| <span data-ttu-id="cb381-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb381-115">Application</span></span>                            | <span data-ttu-id="cb381-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb381-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb381-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb381-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="cb381-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb381-118">Request headers</span></span>

| <span data-ttu-id="cb381-119">名称</span><span class="sxs-lookup"><span data-stu-id="cb381-119">Name</span></span>       | <span data-ttu-id="cb381-120">说明</span><span class="sxs-lookup"><span data-stu-id="cb381-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cb381-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb381-121">Authorization</span></span> | <span data-ttu-id="cb381-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="cb381-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb381-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb381-123">Request body</span></span>

<span data-ttu-id="cb381-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="cb381-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cb381-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="cb381-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cb381-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cb381-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cb381-127">属性</span><span class="sxs-lookup"><span data-stu-id="cb381-127">Property</span></span>     | <span data-ttu-id="cb381-128">类型</span><span class="sxs-lookup"><span data-stu-id="cb381-128">Type</span></span>        | <span data-ttu-id="cb381-129">说明</span><span class="sxs-lookup"><span data-stu-id="cb381-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb381-130">apiVersion</span><span class="sxs-lookup"><span data-stu-id="cb381-130">apiVersion</span></span>|<span data-ttu-id="cb381-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cb381-131">Int32</span></span>|<span data-ttu-id="cb381-132">回调 url 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="cb381-132">API version for the call back url.</span></span> <span data-ttu-id="cb381-133">从1开始。</span><span class="sxs-lookup"><span data-stu-id="cb381-133">Start with 1.</span></span>|
|<span data-ttu-id="cb381-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cb381-134">displayName</span></span>|<span data-ttu-id="cb381-135">String</span><span class="sxs-lookup"><span data-stu-id="cb381-135">String</span></span>|<span data-ttu-id="cb381-136">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="cb381-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="cb381-137">技术</span><span class="sxs-lookup"><span data-stu-id="cb381-137">encryption</span></span>|<span data-ttu-id="cb381-138">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="cb381-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="cb381-139">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="cb381-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="cb381-140">isActive</span><span class="sxs-lookup"><span data-stu-id="cb381-140">isActive</span></span>|<span data-ttu-id="cb381-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb381-141">Boolean</span></span>|<span data-ttu-id="cb381-142">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="cb381-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="cb381-143">支持</span><span class="sxs-lookup"><span data-stu-id="cb381-143">supports</span></span>|<span data-ttu-id="cb381-144">string</span><span class="sxs-lookup"><span data-stu-id="cb381-144">string</span></span>| <span data-ttu-id="cb381-145">可能的值为、、、、 `none` `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` 。</span><span class="sxs-lookup"><span data-stu-id="cb381-145">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="cb381-146">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="cb381-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="cb381-147">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="cb381-147">supportedEntities</span></span>|<span data-ttu-id="cb381-148">string</span><span class="sxs-lookup"><span data-stu-id="cb381-148">string</span></span>| <span data-ttu-id="cb381-149">此属性将替换1.0 版中的 **支持** 。</span><span class="sxs-lookup"><span data-stu-id="cb381-149">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="cb381-150">建议使用此属性，而不 **支持** 。</span><span class="sxs-lookup"><span data-stu-id="cb381-150">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="cb381-151">**支持** 属性将在 beta 中仍受支持。</span><span class="sxs-lookup"><span data-stu-id="cb381-151">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="cb381-152">可能的值为、、、、 `none` `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` 。</span><span class="sxs-lookup"><span data-stu-id="cb381-152">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="cb381-153">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="cb381-153">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="cb381-154">url</span><span class="sxs-lookup"><span data-stu-id="cb381-154">url</span></span>|<span data-ttu-id="cb381-155">String</span><span class="sxs-lookup"><span data-stu-id="cb381-155">String</span></span>| <span data-ttu-id="cb381-156">劳动力集成 url，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="cb381-156">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="cb381-157">响应</span><span class="sxs-lookup"><span data-stu-id="cb381-157">Response</span></span>

<span data-ttu-id="cb381-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb381-158">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb381-159">示例</span><span class="sxs-lookup"><span data-stu-id="cb381-159">Examples</span></span>

### <a name="example-1-update-a-workforceintegration-object"></a><span data-ttu-id="cb381-160">示例1：更新 workforceIntegration 对象</span><span class="sxs-lookup"><span data-stu-id="cb381-160">Example 1: Update a workforceIntegration object</span></span>

<span data-ttu-id="cb381-161">下面的示例更新一个 **workforceIntegration** 对象。</span><span class="sxs-lookup"><span data-stu-id="cb381-161">The following example updates a **workforceIntegration** object.</span></span>

#### <a name="request"></a><span data-ttu-id="cb381-162">请求</span><span class="sxs-lookup"><span data-stu-id="cb381-162">Request</span></span>

<span data-ttu-id="cb381-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb381-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb381-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb381-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cb381-165">C#</span><span class="sxs-lookup"><span data-stu-id="cb381-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb381-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb381-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb381-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb381-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb381-168">Java</span><span class="sxs-lookup"><span data-stu-id="cb381-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb381-169">响应</span><span class="sxs-lookup"><span data-stu-id="cb381-169">Response</span></span>

<span data-ttu-id="cb381-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb381-170">The following is an example of the response.</span></span>

> <span data-ttu-id="cb381-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cb381-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="cb381-173">示例2：创建一个新的 workforceIntegration，并为其启用 SwapRequest 的资格筛选</span><span class="sxs-lookup"><span data-stu-id="cb381-173">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="cb381-174">下面的示例将创建一个新的 **workforceIntegration** ，其中 SwapRequest 启用了资格筛选。</span><span class="sxs-lookup"><span data-stu-id="cb381-174">The following example creates a new **workforceIntegration** with SwapRequest enabled for eligibility filtering.</span></span>

#### <a name="request"></a><span data-ttu-id="cb381-175">请求</span><span class="sxs-lookup"><span data-stu-id="cb381-175">Request</span></span>

<span data-ttu-id="cb381-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb381-176">The following is an example of the request.</span></span> 
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
#### <a name="response"></a><span data-ttu-id="cb381-177">响应</span><span class="sxs-lookup"><span data-stu-id="cb381-177">Response</span></span>

<span data-ttu-id="cb381-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb381-178">The following is an example of the response.</span></span>
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
<span data-ttu-id="cb381-179">若要创建新的 **workforceIntegration** 并启用 SwapRequest 的资格筛选，请参阅 [create](../api/workforceintegration-post.md) 方法。</span><span class="sxs-lookup"><span data-stu-id="cb381-179">To create a new **workforceIntegration** with SwapRequest enabled for eligibility filtering, see the [Create](../api/workforceintegration-post.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="cb381-180">示例3：在 eligibilityFilteringEnabledEntities 中包含 SwapRequest 时提取符合条件的班次</span><span class="sxs-lookup"><span data-stu-id="cb381-180">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="cb381-181">倒班应用和劳动力集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="cb381-181">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

#### <a name="request"></a><span data-ttu-id="cb381-182">请求</span><span class="sxs-lookup"><span data-stu-id="cb381-182">Request</span></span>

<span data-ttu-id="cb381-183">下面的示例演示了如何通过转到劳动力集成终结点来获取交换请求的符合条件的请求。</span><span class="sxs-lookup"><span data-stu-id="cb381-183">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
#### <a name="response"></a><span data-ttu-id="cb381-184">响应</span><span class="sxs-lookup"><span data-stu-id="cb381-184">Response</span></span>

<span data-ttu-id="cb381-185">以下是劳动力集成服务响应的示例。</span><span class="sxs-lookup"><span data-stu-id="cb381-185">The following is an example of the response from the workforce integration service.</span></span>
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


