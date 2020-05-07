---
title: 创建 workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b810e83e1444312ede43933edaf2d29d76ab9b07
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154092"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="10253-103">创建 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="10253-103">Create workforceIntegration</span></span>

<span data-ttu-id="10253-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10253-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10253-105">创建新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10253-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10253-106">权限</span><span class="sxs-lookup"><span data-stu-id="10253-106">Permissions</span></span>

<span data-ttu-id="10253-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10253-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10253-109">Permission type</span></span>                        | <span data-ttu-id="10253-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10253-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10253-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10253-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10253-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="10253-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="10253-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10253-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10253-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="10253-114">Not supported.</span></span> |
| <span data-ttu-id="10253-115">Application</span><span class="sxs-lookup"><span data-stu-id="10253-115">Application</span></span>                            | <span data-ttu-id="10253-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10253-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10253-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10253-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="10253-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="10253-118">Request headers</span></span>

| <span data-ttu-id="10253-119">名称</span><span class="sxs-lookup"><span data-stu-id="10253-119">Name</span></span>          | <span data-ttu-id="10253-120">说明</span><span class="sxs-lookup"><span data-stu-id="10253-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10253-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10253-121">Authorization</span></span> | <span data-ttu-id="10253-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10253-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10253-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="10253-124">Content-type</span></span> | <span data-ttu-id="10253-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="10253-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10253-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10253-127">Request body</span></span>

<span data-ttu-id="10253-128">在请求正文中，提供[workforceIntegration](../resources/workforceintegration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10253-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10253-129">响应</span><span class="sxs-lookup"><span data-stu-id="10253-129">Response</span></span>

<span data-ttu-id="10253-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10253-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10253-131">示例</span><span class="sxs-lookup"><span data-stu-id="10253-131">Examples</span></span>

### <a name="example-1-create-a-new-workforceintegration-object"></a><span data-ttu-id="10253-132">示例1：创建新的 workforceIntegration 对象。</span><span class="sxs-lookup"><span data-stu-id="10253-132">Example 1: Create a new workforceIntegration object.</span></span>

#### <a name="request"></a><span data-ttu-id="10253-133">请求</span><span class="sxs-lookup"><span data-stu-id="10253-133">Request</span></span>

<span data-ttu-id="10253-134">下面是创建新的**workforceIntegration**对象的请求示例。</span><span class="sxs-lookup"><span data-stu-id="10253-134">The following is an example of a request to create a new **workforceIntegration** object.</span></span>

# <a name="http"></a>[<span data-ttu-id="10253-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="10253-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
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
# <a name="c"></a>[<span data-ttu-id="10253-136">C#</span><span class="sxs-lookup"><span data-stu-id="10253-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10253-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10253-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10253-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10253-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10253-139">响应</span><span class="sxs-lookup"><span data-stu-id="10253-139">Response</span></span>

<span data-ttu-id="10253-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="10253-140">The following is an example of the response.</span></span>

> <span data-ttu-id="10253-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="10253-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="10253-143">示例2：创建一个新的 workforceIntegration，并为其启用 SwapRequest 的资格筛选</span><span class="sxs-lookup"><span data-stu-id="10253-143">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="10253-144">以下是对 SwapRequest 启用了资格筛选的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="10253-144">The following is an example of a request with SwapRequest enabled for eligibility filtering.</span></span> 

#### <a name="request"></a><span data-ttu-id="10253-145">请求</span><span class="sxs-lookup"><span data-stu-id="10253-145">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="10253-146">响应</span><span class="sxs-lookup"><span data-stu-id="10253-146">Response</span></span>

<span data-ttu-id="10253-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="10253-147">The following is an example of the response.</span></span>
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
<span data-ttu-id="10253-148">若要更新启用了 SwapRequest 的现有**workforceIntegration**对象以进行资格筛选，请参阅[update](../api/workforceintegration-update.md)方法。</span><span class="sxs-lookup"><span data-stu-id="10253-148">To update an existing **workforceIntegration** object with SwapRequest enabled for eligibility filtering, see the [Update](../api/workforceintegration-update.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="10253-149">示例3：在 eligibilityFilteringEnabledEntities 中包含 SwapRequest 时提取符合条件的班次</span><span class="sxs-lookup"><span data-stu-id="10253-149">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="10253-150">倒班应用和劳动力集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="10253-150">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="10253-151">请求</span><span class="sxs-lookup"><span data-stu-id="10253-151">Request</span></span>

<span data-ttu-id="10253-152">下面的示例演示了如何通过转到劳动力集成终结点来获取交换请求的符合条件的请求。</span><span class="sxs-lookup"><span data-stu-id="10253-152">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="10253-153">响应</span><span class="sxs-lookup"><span data-stu-id="10253-153">Response</span></span>

<span data-ttu-id="10253-154">以下是劳动力集成服务响应的示例。</span><span class="sxs-lookup"><span data-stu-id="10253-154">The following is an example of the response from the workforce integration service.</span></span>
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
