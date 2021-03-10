---
title: 更新 identityUserFlowAttribute
description: 更新 identityUserFlowAttribute 的属性。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7f9f5589069e6b96115f73edb653d7262efe445a
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625812"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="857ce-103">更新 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="857ce-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="857ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="857ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="857ce-105">更新 [identityUserFlowAttribute 对象](../resources/identityuserflowattribute.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="857ce-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="857ce-106">只能更新自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="857ce-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="857ce-107">权限</span><span class="sxs-lookup"><span data-stu-id="857ce-107">Permissions</span></span>

<span data-ttu-id="857ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="857ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="857ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="857ce-110">Permission type</span></span>      | <span data-ttu-id="857ce-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="857ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="857ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="857ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="857ce-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857ce-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="857ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="857ce-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="857ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="857ce-115">Not supported.</span></span>|
|<span data-ttu-id="857ce-116">Application</span><span class="sxs-lookup"><span data-stu-id="857ce-116">Application</span></span>| <span data-ttu-id="857ce-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="857ce-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="857ce-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="857ce-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="857ce-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="857ce-119">Global administrator</span></span>
* <span data-ttu-id="857ce-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="857ce-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="857ce-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="857ce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="857ce-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="857ce-122">Request headers</span></span>

|<span data-ttu-id="857ce-123">名称</span><span class="sxs-lookup"><span data-stu-id="857ce-123">Name</span></span>|<span data-ttu-id="857ce-124">说明</span><span class="sxs-lookup"><span data-stu-id="857ce-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="857ce-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="857ce-125">Authorization</span></span>|<span data-ttu-id="857ce-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="857ce-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="857ce-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="857ce-128">Content-Type</span></span>|<span data-ttu-id="857ce-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="857ce-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="857ce-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="857ce-131">Request body</span></span>

<span data-ttu-id="857ce-132">在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要针对 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象进行更新。</span><span class="sxs-lookup"><span data-stu-id="857ce-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="857ce-133">**注意：** 只能 **更新 description** 属性。</span><span class="sxs-lookup"><span data-stu-id="857ce-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="857ce-134">属性</span><span class="sxs-lookup"><span data-stu-id="857ce-134">Property</span></span>|<span data-ttu-id="857ce-135">类型</span><span class="sxs-lookup"><span data-stu-id="857ce-135">Type</span></span>|<span data-ttu-id="857ce-136">说明</span><span class="sxs-lookup"><span data-stu-id="857ce-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="857ce-137">说明</span><span class="sxs-lookup"><span data-stu-id="857ce-137">description</span></span>|<span data-ttu-id="857ce-138">String</span><span class="sxs-lookup"><span data-stu-id="857ce-138">String</span></span>|<span data-ttu-id="857ce-139">用户流属性的说明。</span><span class="sxs-lookup"><span data-stu-id="857ce-139">The description of the user flow attribute.</span></span> <span data-ttu-id="857ce-140">它在注册时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="857ce-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="857ce-141">响应</span><span class="sxs-lookup"><span data-stu-id="857ce-141">Response</span></span>

<span data-ttu-id="857ce-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="857ce-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="857ce-143">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="857ce-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="857ce-144">示例</span><span class="sxs-lookup"><span data-stu-id="857ce-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="857ce-145">请求</span><span class="sxs-lookup"><span data-stu-id="857ce-145">Request</span></span>

<span data-ttu-id="857ce-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="857ce-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="857ce-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="857ce-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```
# <a name="c"></a>[<span data-ttu-id="857ce-148">C#</span><span class="sxs-lookup"><span data-stu-id="857ce-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="857ce-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="857ce-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="857ce-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="857ce-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="857ce-151">Java</span><span class="sxs-lookup"><span data-stu-id="857ce-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="857ce-152">响应</span><span class="sxs-lookup"><span data-stu-id="857ce-152">Response</span></span>

<span data-ttu-id="857ce-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="857ce-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
