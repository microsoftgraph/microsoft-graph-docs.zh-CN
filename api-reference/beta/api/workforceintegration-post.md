---
title: Create workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76cb01efb15f7937c9e71e1fa26eb8d425f2b4d7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054684"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="f555a-103">Create workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="f555a-103">Create workforceIntegration</span></span>

<span data-ttu-id="f555a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f555a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f555a-105">创建新的 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f555a-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f555a-106">权限</span><span class="sxs-lookup"><span data-stu-id="f555a-106">Permissions</span></span>

<span data-ttu-id="f555a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f555a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f555a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f555a-109">Permission type</span></span>                        | <span data-ttu-id="f555a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f555a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f555a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f555a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f555a-112">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f555a-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f555a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f555a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f555a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f555a-114">Not supported.</span></span> |
| <span data-ttu-id="f555a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f555a-115">Application</span></span>                            | <span data-ttu-id="f555a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f555a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f555a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f555a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="f555a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f555a-118">Request headers</span></span>

| <span data-ttu-id="f555a-119">名称</span><span class="sxs-lookup"><span data-stu-id="f555a-119">Name</span></span>          | <span data-ttu-id="f555a-120">说明</span><span class="sxs-lookup"><span data-stu-id="f555a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f555a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f555a-121">Authorization</span></span> | <span data-ttu-id="f555a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f555a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f555a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="f555a-124">Content-type</span></span> | <span data-ttu-id="f555a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f555a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f555a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f555a-127">Request body</span></span>

<span data-ttu-id="f555a-128">在请求正文中，提供 [workforceIntegration](../resources/workforceintegration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f555a-128">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f555a-129">响应</span><span class="sxs-lookup"><span data-stu-id="f555a-129">Response</span></span>

<span data-ttu-id="f555a-130">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和新 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f555a-130">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f555a-131">示例</span><span class="sxs-lookup"><span data-stu-id="f555a-131">Examples</span></span>

### <a name="example-1-create-a-new-workforceintegration-object"></a><span data-ttu-id="f555a-132">示例 1：创建新的 workforceIntegration 对象。</span><span class="sxs-lookup"><span data-stu-id="f555a-132">Example 1: Create a new workforceIntegration object.</span></span>

#### <a name="request"></a><span data-ttu-id="f555a-133">请求</span><span class="sxs-lookup"><span data-stu-id="f555a-133">Request</span></span>

<span data-ttu-id="f555a-134">下面是一个请求创建新的 **workforceIntegration** 对象的示例。</span><span class="sxs-lookup"><span data-stu-id="f555a-134">The following is an example of a request to create a new **workforceIntegration** object.</span></span>

# <a name="http"></a>[<span data-ttu-id="f555a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f555a-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f555a-136">C#</span><span class="sxs-lookup"><span data-stu-id="f555a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f555a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f555a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f555a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f555a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f555a-139">Java</span><span class="sxs-lookup"><span data-stu-id="f555a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f555a-140">响应</span><span class="sxs-lookup"><span data-stu-id="f555a-140">Response</span></span>

<span data-ttu-id="f555a-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f555a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f555a-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f555a-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="f555a-143">示例 2：新建一个针对资格筛选启用 SwapRequest 的 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="f555a-143">Example 2: Create a new workforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

<span data-ttu-id="f555a-144">下面是一个请求示例，请求启用了 SwapRequest 进行资格筛选。</span><span class="sxs-lookup"><span data-stu-id="f555a-144">The following is an example of a request with SwapRequest enabled for eligibility filtering.</span></span> 

#### <a name="request"></a><span data-ttu-id="f555a-145">请求</span><span class="sxs-lookup"><span data-stu-id="f555a-145">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="f555a-146">响应</span><span class="sxs-lookup"><span data-stu-id="f555a-146">Response</span></span>

<span data-ttu-id="f555a-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f555a-147">The following is an example of the response.</span></span>
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
<span data-ttu-id="f555a-148">若要使用启用了资格筛选的 SwapRequest 更新现有的 **workforceIntegration** 对象，请参阅 [Update](../api/workforceintegration-update.md) 方法。</span><span class="sxs-lookup"><span data-stu-id="f555a-148">To update an existing **workforceIntegration** object with SwapRequest enabled for eligibility filtering, see the [Update](../api/workforceintegration-update.md) method.</span></span>

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="f555a-149">示例 3：在 SwapRequest 包含在 eligiblyFilteringEnabledEntities 中时提取符合条件的班次</span><span class="sxs-lookup"><span data-stu-id="f555a-149">Example 3: Fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>

<span data-ttu-id="f555a-150">班次应用和员工集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="f555a-150">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="f555a-151">请求</span><span class="sxs-lookup"><span data-stu-id="f555a-151">Request</span></span>

<span data-ttu-id="f555a-152">下面是 Shifts 向员工集成终结点请求获取交换请求的合格班次的示例。</span><span class="sxs-lookup"><span data-stu-id="f555a-152">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="f555a-153">响应</span><span class="sxs-lookup"><span data-stu-id="f555a-153">Response</span></span>

<span data-ttu-id="f555a-154">下面是员工集成服务的响应示例。</span><span class="sxs-lookup"><span data-stu-id="f555a-154">The following is an example of the response from the workforce integration service.</span></span>
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


