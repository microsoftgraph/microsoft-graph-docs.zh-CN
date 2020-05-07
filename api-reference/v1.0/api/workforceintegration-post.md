---
title: 创建 workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 74481ea9bcb843b89bb1de3fdf444e359762aaa4
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154036"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="74025-103">创建 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="74025-103">Create workforceIntegration</span></span>

<span data-ttu-id="74025-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74025-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74025-105">创建新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74025-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>
<span data-ttu-id="74025-106">您可以设置要接收其上的同步更改通知的实体并设置实体以配置按 WFM 规则（包括交换请求）的筛选的筛选器。</span><span class="sxs-lookup"><span data-stu-id="74025-106">You can set up which entities you want to receive Shifts synchronous change notifications on and set entities to configure filtering by WFM rules eligibility for, including swap requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="74025-107">权限</span><span class="sxs-lookup"><span data-stu-id="74025-107">Permissions</span></span>

<span data-ttu-id="74025-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74025-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74025-110">Permission type</span></span>                        | <span data-ttu-id="74025-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74025-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74025-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74025-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="74025-113">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="74025-113">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="74025-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74025-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74025-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74025-115">Not supported.</span></span> |
| <span data-ttu-id="74025-116">Application</span><span class="sxs-lookup"><span data-stu-id="74025-116">Application</span></span>                            | <span data-ttu-id="74025-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="74025-117">Not supported.</span></span> |

> <span data-ttu-id="74025-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="74025-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="74025-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="74025-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="74025-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74025-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="74025-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="74025-121">Request headers</span></span>

| <span data-ttu-id="74025-122">名称</span><span class="sxs-lookup"><span data-stu-id="74025-122">Name</span></span>          | <span data-ttu-id="74025-123">说明</span><span class="sxs-lookup"><span data-stu-id="74025-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="74025-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="74025-124">Authorization</span></span> | <span data-ttu-id="74025-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74025-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74025-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="74025-127">Content-type</span></span> | <span data-ttu-id="74025-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="74025-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74025-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="74025-130">Request body</span></span>

<span data-ttu-id="74025-131">在请求正文中，提供[workforceIntegration](../resources/workforceintegration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74025-131">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="74025-132">响应</span><span class="sxs-lookup"><span data-stu-id="74025-132">Response</span></span>

<span data-ttu-id="74025-133">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74025-133">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74025-134">示例</span><span class="sxs-lookup"><span data-stu-id="74025-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74025-135">请求</span><span class="sxs-lookup"><span data-stu-id="74025-135">Request</span></span>

<span data-ttu-id="74025-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74025-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
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


### <a name="response"></a><span data-ttu-id="74025-137">响应</span><span class="sxs-lookup"><span data-stu-id="74025-137">Response</span></span>

<span data-ttu-id="74025-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74025-138">The following is an example of the response.</span></span>

> <span data-ttu-id="74025-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="74025-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
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

## <a name="examples-for-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="74025-141">用于按 WFM 规则资格进行筛选的 WorkforceIntegration 实体的用例示例</span><span class="sxs-lookup"><span data-stu-id="74025-141">Examples for Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="74025-142">用例：创建具有 SwapRequest 的新 WorkforceIntegration 以启用资格筛选</span><span class="sxs-lookup"><span data-stu-id="74025-142">Use case: Create a new WorkforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="74025-143">请求</span><span class="sxs-lookup"><span data-stu-id="74025-143">Request</span></span>

<span data-ttu-id="74025-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74025-144">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/
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
Authorization: Bearer {token}
Content-type: application/json
```
### <a name="response"></a><span data-ttu-id="74025-145">响应</span><span class="sxs-lookup"><span data-stu-id="74025-145">Response</span></span>

<span data-ttu-id="74025-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74025-146">The following is an example of the response.</span></span>
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
<span data-ttu-id="74025-147">若要了解如何更新启用了 SwapRequest 的现有 workforceintegration 以进行资格筛选，请参阅[更新](../api/workforceintegration-update.md)。</span><span class="sxs-lookup"><span data-stu-id="74025-147">To see how to update an existing workforceintegration with SwapRequest enabled for eligibility filtering, see [Update](../api/workforceintegration-update.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="74025-148">EligibilityFilteringEnabledEntities 中包含 SwapRequest 时获取符合条件的班次的示例</span><span class="sxs-lookup"><span data-stu-id="74025-148">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="74025-149">倒班应用和劳动力集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="74025-149">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="74025-150">请求</span><span class="sxs-lookup"><span data-stu-id="74025-150">Request</span></span>

<span data-ttu-id="74025-151">下面的示例演示了如何通过转到劳动力集成终结点来获取交换请求的符合条件的请求。</span><span class="sxs-lookup"><span data-stu-id="74025-151">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="74025-152">响应</span><span class="sxs-lookup"><span data-stu-id="74025-152">Response</span></span>

<span data-ttu-id="74025-153">以下是劳动力集成服务响应的示例。</span><span class="sxs-lookup"><span data-stu-id="74025-153">The following is an example of the response from the workforce integration service.</span></span>
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
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
