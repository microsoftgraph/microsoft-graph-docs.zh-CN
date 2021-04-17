---
title: 更新 identityUserFlowAttribute
description: 更新 identityUserFlowAttribute 的属性。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: d998a5501443c026d685ac8eaec7910312d35967
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882966"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="c5a23-103">更新 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="c5a23-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="c5a23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5a23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5a23-105">更新 [identityUserFlowAttribute 对象](../resources/identityuserflowattribute.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c5a23-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="c5a23-106">只能更新自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="c5a23-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5a23-107">权限</span><span class="sxs-lookup"><span data-stu-id="c5a23-107">Permissions</span></span>

<span data-ttu-id="c5a23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5a23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5a23-110">Permission type</span></span>      | <span data-ttu-id="c5a23-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5a23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5a23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a23-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a23-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a23-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c5a23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a23-115">Not supported.</span></span>|
|<span data-ttu-id="c5a23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5a23-116">Application</span></span>| <span data-ttu-id="c5a23-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a23-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c5a23-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="c5a23-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c5a23-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c5a23-119">Global administrator</span></span>
* <span data-ttu-id="c5a23-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="c5a23-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c5a23-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5a23-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c5a23-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5a23-122">Request headers</span></span>

|<span data-ttu-id="c5a23-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5a23-123">Name</span></span>|<span data-ttu-id="c5a23-124">说明</span><span class="sxs-lookup"><span data-stu-id="c5a23-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c5a23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a23-125">Authorization</span></span>|<span data-ttu-id="c5a23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a23-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c5a23-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5a23-128">Content-Type</span></span>|<span data-ttu-id="c5a23-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c5a23-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a23-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5a23-131">Request body</span></span>

<span data-ttu-id="c5a23-132">在请求正文中，为 JSON 对象提供一个或多个需要为 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象更新的属性。</span><span class="sxs-lookup"><span data-stu-id="c5a23-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="c5a23-133">**注意：** 只能 **更新 description** 属性。</span><span class="sxs-lookup"><span data-stu-id="c5a23-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="c5a23-134">属性</span><span class="sxs-lookup"><span data-stu-id="c5a23-134">Property</span></span>|<span data-ttu-id="c5a23-135">类型</span><span class="sxs-lookup"><span data-stu-id="c5a23-135">Type</span></span>|<span data-ttu-id="c5a23-136">说明</span><span class="sxs-lookup"><span data-stu-id="c5a23-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5a23-137">说明</span><span class="sxs-lookup"><span data-stu-id="c5a23-137">description</span></span>|<span data-ttu-id="c5a23-138">String</span><span class="sxs-lookup"><span data-stu-id="c5a23-138">String</span></span>|<span data-ttu-id="c5a23-139">用户流属性的说明。</span><span class="sxs-lookup"><span data-stu-id="c5a23-139">The description of the user flow attribute.</span></span> <span data-ttu-id="c5a23-140">它在注册时显示给用户。</span><span class="sxs-lookup"><span data-stu-id="c5a23-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="c5a23-141">响应</span><span class="sxs-lookup"><span data-stu-id="c5a23-141">Response</span></span>

<span data-ttu-id="c5a23-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c5a23-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="c5a23-143">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="c5a23-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="c5a23-144">示例</span><span class="sxs-lookup"><span data-stu-id="c5a23-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5a23-145">请求</span><span class="sxs-lookup"><span data-stu-id="c5a23-145">Request</span></span>

<span data-ttu-id="c5a23-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5a23-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```

### <a name="response"></a><span data-ttu-id="c5a23-147">响应</span><span class="sxs-lookup"><span data-stu-id="c5a23-147">Response</span></span>

<span data-ttu-id="c5a23-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5a23-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
