---
title: 更新 workforceIntegration
description: 更新 workforceIntegration 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ac4ee0543adb2054782c2b66a454451a20d98c2
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154015"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="99c0b-103">更新 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="99c0b-103">Update workforceIntegration</span></span>

<span data-ttu-id="99c0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99c0b-105">更新[workforceIntegration](../resources/workforceintegration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99c0b-105">Update the properties of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99c0b-106">权限</span><span class="sxs-lookup"><span data-stu-id="99c0b-106">Permissions</span></span>

<span data-ttu-id="99c0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99c0b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99c0b-109">Permission type</span></span>                        | <span data-ttu-id="99c0b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99c0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="99c0b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99c0b-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="99c0b-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="99c0b-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="99c0b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99c0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99c0b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c0b-114">Not supported.</span></span> |
| <span data-ttu-id="99c0b-115">Application</span><span class="sxs-lookup"><span data-stu-id="99c0b-115">Application</span></span>                            | <span data-ttu-id="99c0b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c0b-116">Not supported.</span></span> |

> <span data-ttu-id="99c0b-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="99c0b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="99c0b-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="99c0b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="99c0b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99c0b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="99c0b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99c0b-120">Request headers</span></span>

| <span data-ttu-id="99c0b-121">名称</span><span class="sxs-lookup"><span data-stu-id="99c0b-121">Name</span></span>       | <span data-ttu-id="99c0b-122">说明</span><span class="sxs-lookup"><span data-stu-id="99c0b-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="99c0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99c0b-123">Authorization</span></span> | <span data-ttu-id="99c0b-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="99c0b-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="99c0b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="99c0b-125">Request body</span></span>

<span data-ttu-id="99c0b-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="99c0b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="99c0b-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="99c0b-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="99c0b-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="99c0b-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99c0b-129">属性</span><span class="sxs-lookup"><span data-stu-id="99c0b-129">Property</span></span>     | <span data-ttu-id="99c0b-130">类型</span><span class="sxs-lookup"><span data-stu-id="99c0b-130">Type</span></span>        | <span data-ttu-id="99c0b-131">Description</span><span class="sxs-lookup"><span data-stu-id="99c0b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99c0b-132">apiVersion</span><span class="sxs-lookup"><span data-stu-id="99c0b-132">apiVersion</span></span>|<span data-ttu-id="99c0b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="99c0b-133">Int32</span></span>|<span data-ttu-id="99c0b-134">回调 URL 的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="99c0b-134">API version for the call back URL.</span></span> <span data-ttu-id="99c0b-135">从1开始。</span><span class="sxs-lookup"><span data-stu-id="99c0b-135">Start with 1.</span></span>|
|<span data-ttu-id="99c0b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="99c0b-136">displayName</span></span>|<span data-ttu-id="99c0b-137">String</span><span class="sxs-lookup"><span data-stu-id="99c0b-137">String</span></span>|<span data-ttu-id="99c0b-138">劳动力集成的名称。</span><span class="sxs-lookup"><span data-stu-id="99c0b-138">Name of the workforce integration.</span></span>|
|<span data-ttu-id="99c0b-139">技术</span><span class="sxs-lookup"><span data-stu-id="99c0b-139">encryption</span></span>|<span data-ttu-id="99c0b-140">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="99c0b-140">workforceIntegrationEncryption</span></span>|<span data-ttu-id="99c0b-141">劳动力集成加密资源。</span><span class="sxs-lookup"><span data-stu-id="99c0b-141">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="99c0b-142">isActive</span><span class="sxs-lookup"><span data-stu-id="99c0b-142">isActive</span></span>|<span data-ttu-id="99c0b-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="99c0b-143">Boolean</span></span>|<span data-ttu-id="99c0b-144">指示此劳动力集成当前是否处于活动状态且可用。</span><span class="sxs-lookup"><span data-stu-id="99c0b-144">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="99c0b-145">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="99c0b-145">supportedEntities</span></span>|<span data-ttu-id="99c0b-146">string</span><span class="sxs-lookup"><span data-stu-id="99c0b-146">string</span></span>| <span data-ttu-id="99c0b-147">可取值为：`none`、`shift`、`swapRequest`、`openshift`、`openShiftRequest`、`userShiftPreferences`。</span><span class="sxs-lookup"><span data-stu-id="99c0b-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="99c0b-148">如果选择多个值，则所有值必须以大写形式的第一个字母开头。</span><span class="sxs-lookup"><span data-stu-id="99c0b-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="99c0b-149">url</span><span class="sxs-lookup"><span data-stu-id="99c0b-149">url</span></span>|<span data-ttu-id="99c0b-150">String</span><span class="sxs-lookup"><span data-stu-id="99c0b-150">String</span></span>| <span data-ttu-id="99c0b-151">劳动力集成 URL，用于从班次服务进行回调。</span><span class="sxs-lookup"><span data-stu-id="99c0b-151">Workforce integration URL for callbacks from the shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="99c0b-152">响应</span><span class="sxs-lookup"><span data-stu-id="99c0b-152">Response</span></span>

<span data-ttu-id="99c0b-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99c0b-153">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99c0b-154">示例</span><span class="sxs-lookup"><span data-stu-id="99c0b-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99c0b-155">请求</span><span class="sxs-lookup"><span data-stu-id="99c0b-155">Request</span></span>

<span data-ttu-id="99c0b-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99c0b-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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
---


### <a name="response"></a><span data-ttu-id="99c0b-157">响应</span><span class="sxs-lookup"><span data-stu-id="99c0b-157">Response</span></span>

<span data-ttu-id="99c0b-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99c0b-158">The following is an example of the response.</span></span>

> <span data-ttu-id="99c0b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="99c0b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="examples-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="99c0b-161">WorkforceIntegration 实体的示例用例用于按 WFM 规则资格进行筛选</span><span class="sxs-lookup"><span data-stu-id="99c0b-161">Examples Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-replace-an-existing-workforceintegration-to-enable-swaprequest-for-eligibility-filtering"></a><span data-ttu-id="99c0b-162">用例：替换现有的 WorkforceIntegration 以启用 SwapRequest 的资格筛选</span><span class="sxs-lookup"><span data-stu-id="99c0b-162">Use case: Replace an existing WorkforceIntegration to enable SwapRequest for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="99c0b-163">请求</span><span class="sxs-lookup"><span data-stu-id="99c0b-163">Request</span></span>

<span data-ttu-id="99c0b-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99c0b-164">The following is an example of the request.</span></span> 
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
### <a name="response"></a><span data-ttu-id="99c0b-165">响应</span><span class="sxs-lookup"><span data-stu-id="99c0b-165">Response</span></span>

<span data-ttu-id="99c0b-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99c0b-166">The following is an example of the response.</span></span>
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
<span data-ttu-id="99c0b-167">若要了解如何创建具有 SwapRequest 的新 workforceintegration 以启用资格筛选，请参阅[create](../api/workforceintegration-post.md)。</span><span class="sxs-lookup"><span data-stu-id="99c0b-167">To see how to create a new workforceintegration with SwapRequest enabled for eligibility filtering, see [Create](../api/workforceintegration-post.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="99c0b-168">EligibilityFilteringEnabledEntities 中包含 SwapRequest 时获取符合条件的班次的示例</span><span class="sxs-lookup"><span data-stu-id="99c0b-168">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="99c0b-169">倒班应用和劳动力集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="99c0b-169">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="99c0b-170">请求</span><span class="sxs-lookup"><span data-stu-id="99c0b-170">Request</span></span>

<span data-ttu-id="99c0b-171">下面的示例演示了如何通过转到劳动力集成终结点来获取交换请求的符合条件的请求。</span><span class="sxs-lookup"><span data-stu-id="99c0b-171">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="99c0b-172">响应</span><span class="sxs-lookup"><span data-stu-id="99c0b-172">Response</span></span>

<span data-ttu-id="99c0b-173">以下是劳动力集成服务响应的示例。</span><span class="sxs-lookup"><span data-stu-id="99c0b-173">The following is an example of the response from the workforce integration service.</span></span>
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
