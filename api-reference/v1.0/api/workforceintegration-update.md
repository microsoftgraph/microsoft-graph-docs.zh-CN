---
title: 更新工作人员集成
description: 更新 workforceIntegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5efd624bf4a8104465e7663a41b758ec8661a2eb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031515"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="97cac-103">更新工作人员集成</span><span class="sxs-lookup"><span data-stu-id="97cac-103">Update workforceIntegration</span></span>

<span data-ttu-id="97cac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97cac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97cac-105">更新 [workforceIntegration 对象](../resources/workforceintegration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="97cac-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97cac-106">权限</span><span class="sxs-lookup"><span data-stu-id="97cac-106">Permissions</span></span>

<span data-ttu-id="97cac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97cac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97cac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97cac-109">Permission type</span></span>                        | <span data-ttu-id="97cac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97cac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97cac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97cac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="97cac-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97cac-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="97cac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97cac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97cac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97cac-114">Not supported.</span></span> |
| <span data-ttu-id="97cac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97cac-115">Application</span></span>                            | <span data-ttu-id="97cac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97cac-116">Not supported.</span></span> |

> <span data-ttu-id="97cac-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="97cac-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="97cac-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="97cac-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="97cac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97cac-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="97cac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="97cac-120">Request headers</span></span>

| <span data-ttu-id="97cac-121">名称</span><span class="sxs-lookup"><span data-stu-id="97cac-121">Name</span></span>       | <span data-ttu-id="97cac-122">说明</span><span class="sxs-lookup"><span data-stu-id="97cac-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97cac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97cac-123">Authorization</span></span> | <span data-ttu-id="97cac-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="97cac-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="97cac-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="97cac-125">Request body</span></span>

<span data-ttu-id="97cac-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="97cac-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="97cac-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="97cac-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="97cac-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="97cac-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97cac-129">属性</span><span class="sxs-lookup"><span data-stu-id="97cac-129">Property</span></span>     | <span data-ttu-id="97cac-130">类型</span><span class="sxs-lookup"><span data-stu-id="97cac-130">Type</span></span>        | <span data-ttu-id="97cac-131">说明</span><span class="sxs-lookup"><span data-stu-id="97cac-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97cac-132">apiVersion</span><span class="sxs-lookup"><span data-stu-id="97cac-132">apiVersion</span></span>|<span data-ttu-id="97cac-133">Int32</span><span class="sxs-lookup"><span data-stu-id="97cac-133">Int32</span></span>|<span data-ttu-id="97cac-134">用于回叫 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="97cac-134">API version for the call back URL.</span></span> <span data-ttu-id="97cac-135">从 1 开始。</span><span class="sxs-lookup"><span data-stu-id="97cac-135">Start with 1.</span></span>|
|<span data-ttu-id="97cac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="97cac-136">displayName</span></span>|<span data-ttu-id="97cac-137">String</span><span class="sxs-lookup"><span data-stu-id="97cac-137">String</span></span>|<span data-ttu-id="97cac-138">员工集成的名称。</span><span class="sxs-lookup"><span data-stu-id="97cac-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="97cac-139">加密</span><span class="sxs-lookup"><span data-stu-id="97cac-139">encryption</span></span>|<span data-ttu-id="97cac-140">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="97cac-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="97cac-141">员工集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="97cac-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="97cac-142">isActive</span><span class="sxs-lookup"><span data-stu-id="97cac-142">isActive</span></span>|<span data-ttu-id="97cac-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="97cac-143">Boolean</span></span>|<span data-ttu-id="97cac-144">指示此员工集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="97cac-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="97cac-145">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="97cac-145">supportedEntities</span></span>|<span data-ttu-id="97cac-146">string</span><span class="sxs-lookup"><span data-stu-id="97cac-146">string</span></span>| <span data-ttu-id="97cac-147">可取值为：`none`、`shift`、`swapRequest`、`openshift`、`openShiftRequest`、`userShiftPreferences`。</span><span class="sxs-lookup"><span data-stu-id="97cac-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="97cac-148">如果选择多个值，则所有值必须以大写字母开头。</span><span class="sxs-lookup"><span data-stu-id="97cac-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="97cac-149">url</span><span class="sxs-lookup"><span data-stu-id="97cac-149">url</span></span>|<span data-ttu-id="97cac-150">String</span><span class="sxs-lookup"><span data-stu-id="97cac-150">String</span></span>| <span data-ttu-id="97cac-151">轮班服务中回调的员工集成 URL。</span><span class="sxs-lookup"><span data-stu-id="97cac-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="97cac-152">响应</span><span class="sxs-lookup"><span data-stu-id="97cac-152">Response</span></span>

<span data-ttu-id="97cac-153">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97cac-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97cac-154">示例</span><span class="sxs-lookup"><span data-stu-id="97cac-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97cac-155">请求</span><span class="sxs-lookup"><span data-stu-id="97cac-155">Request</span></span>

<span data-ttu-id="97cac-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97cac-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="97cac-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="97cac-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
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
  "supportedEntities": "supportedEntities-value"
}
```
# <a name="c"></a>[<span data-ttu-id="97cac-158">C#</span><span class="sxs-lookup"><span data-stu-id="97cac-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97cac-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97cac-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97cac-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97cac-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97cac-161">Java</span><span class="sxs-lookup"><span data-stu-id="97cac-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="97cac-162">响应</span><span class="sxs-lookup"><span data-stu-id="97cac-162">Response</span></span>

<span data-ttu-id="97cac-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97cac-163">The following is an example of the response.</span></span>

> <span data-ttu-id="97cac-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="97cac-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="97cac-165">示例 按 WFM 规则资格筛选的 WorkforceIntegration 实体用例</span><span class="sxs-lookup"><span data-stu-id="97cac-165">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="97cac-166">用例：替换现有的 WorkforceIntegration 以启用适用于资格筛选的 SwapRequest</span><span class="sxs-lookup"><span data-stu-id="97cac-166">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="97cac-167">请求</span><span class="sxs-lookup"><span data-stu-id="97cac-167">Request</span></span>

<span data-ttu-id="97cac-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97cac-168">The following is an example of the request.</span></span> 
```
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationid}
{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    - "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
```
### <a name="response"></a><span data-ttu-id="97cac-169">响应</span><span class="sxs-lookup"><span data-stu-id="97cac-169">Response</span></span>

<span data-ttu-id="97cac-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97cac-170">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
Content-type: application/json
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
<span data-ttu-id="97cac-171">若要了解如何创建启用了 SwapRequest 进行资格筛选的新员工社区，请参阅 [创建](../api/workforceintegration-post.md)。</span><span class="sxs-lookup"><span data-stu-id="97cac-171">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="97cac-172">当 SwapRequest 包含在 eligiblyFilteringEnabledEntities 中时提取合格班次的示例</span><span class="sxs-lookup"><span data-stu-id="97cac-172">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="97cac-173">班次应用和员工集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="97cac-173">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="97cac-174">请求</span><span class="sxs-lookup"><span data-stu-id="97cac-174">Request</span></span>

<span data-ttu-id="97cac-175">下面是 Shifts 向员工集成终结点请求获取交换请求的合格班次的示例。</span><span class="sxs-lookup"><span data-stu-id="97cac-175">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="97cac-176">响应</span><span class="sxs-lookup"><span data-stu-id="97cac-176">Response</span></span>

<span data-ttu-id="97cac-177">下面是员工集成服务的响应示例。</span><span class="sxs-lookup"><span data-stu-id="97cac-177">The following is an example of the response from the workforce integration service.</span></span>
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

