---
title: Create workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2eee6b620bcd22e571a2b526d4a43e70fe91416a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055643"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="0bb62-103">Create workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="0bb62-103">Create workforceIntegration</span></span>

<span data-ttu-id="0bb62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bb62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bb62-105">创建新的 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bb62-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>
<span data-ttu-id="0bb62-106">您可以设置要接收 Shifts 同步更改通知的实体，并设置实体以按 WFM 规则资格配置筛选，包括交换请求。</span><span class="sxs-lookup"><span data-stu-id="0bb62-106">You can set up which entities you want to receive Shifts synchronous change notifications on and set entities to configure filtering by WFM rules eligibility for, including swap requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bb62-107">权限</span><span class="sxs-lookup"><span data-stu-id="0bb62-107">Permissions</span></span>

<span data-ttu-id="0bb62-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bb62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0bb62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bb62-110">Permission type</span></span>                        | <span data-ttu-id="0bb62-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bb62-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0bb62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb62-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0bb62-113">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bb62-113">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="0bb62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bb62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb62-115">Not supported.</span></span> |
| <span data-ttu-id="0bb62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bb62-116">Application</span></span>                            | <span data-ttu-id="0bb62-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb62-117">Not supported.</span></span> |

> <span data-ttu-id="0bb62-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0bb62-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0bb62-119">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="0bb62-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0bb62-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bb62-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="0bb62-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bb62-121">Request headers</span></span>

| <span data-ttu-id="0bb62-122">名称</span><span class="sxs-lookup"><span data-stu-id="0bb62-122">Name</span></span>          | <span data-ttu-id="0bb62-123">说明</span><span class="sxs-lookup"><span data-stu-id="0bb62-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0bb62-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bb62-124">Authorization</span></span> | <span data-ttu-id="0bb62-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0bb62-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bb62-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="0bb62-127">Content-type</span></span> | <span data-ttu-id="0bb62-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0bb62-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bb62-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bb62-130">Request body</span></span>

<span data-ttu-id="0bb62-131">在请求正文中，提供 [workforceIntegration](../resources/workforceintegration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bb62-131">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0bb62-132">响应</span><span class="sxs-lookup"><span data-stu-id="0bb62-132">Response</span></span>

<span data-ttu-id="0bb62-133">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和新 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bb62-133">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bb62-134">示例</span><span class="sxs-lookup"><span data-stu-id="0bb62-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0bb62-135">请求</span><span class="sxs-lookup"><span data-stu-id="0bb62-135">Request</span></span>

<span data-ttu-id="0bb62-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0bb62-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0bb62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bb62-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0bb62-138">C#</span><span class="sxs-lookup"><span data-stu-id="0bb62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bb62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bb62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bb62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bb62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0bb62-141">Java</span><span class="sxs-lookup"><span data-stu-id="0bb62-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="0bb62-142">响应</span><span class="sxs-lookup"><span data-stu-id="0bb62-142">Response</span></span>

<span data-ttu-id="0bb62-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0bb62-143">The following is an example of the response.</span></span>

> <span data-ttu-id="0bb62-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0bb62-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

## <a name="examples-for-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="0bb62-145">按 WFM 规则资格筛选的 WorkforceIntegration 实体用例示例</span><span class="sxs-lookup"><span data-stu-id="0bb62-145">Examples for Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="0bb62-146">用例：新建一个启用 SwapRequest 进行资格筛选的 WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="0bb62-146">Use case: Create a new WorkforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="0bb62-147">请求</span><span class="sxs-lookup"><span data-stu-id="0bb62-147">Request</span></span>

<span data-ttu-id="0bb62-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0bb62-148">The following is an example of the request.</span></span> 
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
### <a name="response"></a><span data-ttu-id="0bb62-149">响应</span><span class="sxs-lookup"><span data-stu-id="0bb62-149">Response</span></span>

<span data-ttu-id="0bb62-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0bb62-150">The following is an example of the response.</span></span>
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
<span data-ttu-id="0bb62-151">若要了解如何使用启用了资格筛选的 SwapRequest 更新现有员工集成，请参阅 [更新](../api/workforceintegration-update.md)。</span><span class="sxs-lookup"><span data-stu-id="0bb62-151">To see how to update an existing workforceintegration with SwapRequest enabled for eligibility filtering, see [Update](../api/workforceintegration-update.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="0bb62-152">当 SwapRequest 包含在 eligiblyFilteringEnabledEntities 中时提取合格班次的示例</span><span class="sxs-lookup"><span data-stu-id="0bb62-152">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="0bb62-153">班次应用和员工集成终结点之间的交互将遵循现有模式。</span><span class="sxs-lookup"><span data-stu-id="0bb62-153">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="0bb62-154">请求</span><span class="sxs-lookup"><span data-stu-id="0bb62-154">Request</span></span>

<span data-ttu-id="0bb62-155">下面是 Shifts 向员工集成终结点请求获取交换请求的合格班次的示例。</span><span class="sxs-lookup"><span data-stu-id="0bb62-155">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

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
### <a name="response"></a><span data-ttu-id="0bb62-156">响应</span><span class="sxs-lookup"><span data-stu-id="0bb62-156">Response</span></span>

<span data-ttu-id="0bb62-157">下面是员工集成服务的响应示例。</span><span class="sxs-lookup"><span data-stu-id="0bb62-157">The following is an example of the response from the workforce integration service.</span></span>
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

