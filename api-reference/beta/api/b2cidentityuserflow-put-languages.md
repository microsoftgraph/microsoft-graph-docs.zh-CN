---
title: 创建语言
description: 在 Azure AD B2C 用户流中创建自定义语言。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e24841cebf0385563a1445a576cda8e8609f40c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438188"
---
# <a name="create-languages"></a><span data-ttu-id="e3de8-103">创建语言</span><span class="sxs-lookup"><span data-stu-id="e3de8-103">Create languages</span></span>

<span data-ttu-id="e3de8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3de8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3de8-105">此方法用于在 Azure AD B2C 用户流中创建或更新自定义语言。</span><span class="sxs-lookup"><span data-stu-id="e3de8-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="e3de8-106">**注意：** 必须先在 Azure AD B2C 用户流中启用语言自定义，然后才能创建自定义语言。</span><span class="sxs-lookup"><span data-stu-id="e3de8-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="e3de8-107">有关详细信息，请参阅 [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md)。</span><span class="sxs-lookup"><span data-stu-id="e3de8-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3de8-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3de8-108">Permissions</span></span>

<span data-ttu-id="e3de8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3de8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3de8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3de8-111">Permission type</span></span>      | <span data-ttu-id="e3de8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3de8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3de8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3de8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3de8-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3de8-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e3de8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3de8-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e3de8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3de8-116">Not supported.</span></span>|
|<span data-ttu-id="e3de8-117">Application</span><span class="sxs-lookup"><span data-stu-id="e3de8-117">Application</span></span>|<span data-ttu-id="e3de8-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3de8-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e3de8-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="e3de8-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e3de8-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e3de8-120">Global administrator</span></span>
* <span data-ttu-id="e3de8-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="e3de8-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e3de8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3de8-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3de8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3de8-123">Request headers</span></span>

|<span data-ttu-id="e3de8-124">名称</span><span class="sxs-lookup"><span data-stu-id="e3de8-124">Name</span></span>|<span data-ttu-id="e3de8-125">说明</span><span class="sxs-lookup"><span data-stu-id="e3de8-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3de8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3de8-126">Authorization</span></span>|<span data-ttu-id="e3de8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3de8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e3de8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3de8-129">Content-Type</span></span>|<span data-ttu-id="e3de8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e3de8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3de8-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3de8-132">Request body</span></span>

<span data-ttu-id="e3de8-133">在请求正文中，提供 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3de8-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="e3de8-134">下表显示创建 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)时可以选择提供的属性。</span><span class="sxs-lookup"><span data-stu-id="e3de8-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="e3de8-135">属性</span><span class="sxs-lookup"><span data-stu-id="e3de8-135">Property</span></span>|<span data-ttu-id="e3de8-136">类型</span><span class="sxs-lookup"><span data-stu-id="e3de8-136">Type</span></span>|<span data-ttu-id="e3de8-137">说明</span><span class="sxs-lookup"><span data-stu-id="e3de8-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3de8-138">id</span><span class="sxs-lookup"><span data-stu-id="e3de8-138">id</span></span>|<span data-ttu-id="e3de8-139">String</span><span class="sxs-lookup"><span data-stu-id="e3de8-139">String</span></span>|<span data-ttu-id="e3de8-140">语言的标识符。</span><span class="sxs-lookup"><span data-stu-id="e3de8-140">The identifier of the language.</span></span> <span data-ttu-id="e3de8-141">此字段符合语言 ID 标记 [RFC 5646，](https://tools.ietf.org/html/rfc5646) 并且必须是已记录的语言 ID。</span><span class="sxs-lookup"><span data-stu-id="e3de8-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="e3de8-142">如果在请求正文中提供，则它必须与请求 URL 中提供的标识相匹配。</span><span class="sxs-lookup"><span data-stu-id="e3de8-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="e3de8-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e3de8-143">isEnabled</span></span>|<span data-ttu-id="e3de8-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3de8-144">Boolean</span></span>|<span data-ttu-id="e3de8-145">指示是否在用户流中启用语言。</span><span class="sxs-lookup"><span data-stu-id="e3de8-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="e3de8-146">如果未在请求中提供，isEnabled 将设置为"true"。</span><span class="sxs-lookup"><span data-stu-id="e3de8-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="e3de8-147">响应</span><span class="sxs-lookup"><span data-stu-id="e3de8-147">Response</span></span>

<span data-ttu-id="e3de8-148">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3de8-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3de8-149">示例</span><span class="sxs-lookup"><span data-stu-id="e3de8-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="e3de8-150">示例 1：在 Azure AD B2C 用户流中创建自定义语言</span><span class="sxs-lookup"><span data-stu-id="e3de8-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="e3de8-151">请求</span><span class="sxs-lookup"><span data-stu-id="e3de8-151">Request</span></span>

<span data-ttu-id="e3de8-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3de8-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3de8-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3de8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "id": "es-ES",
  "isEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="e3de8-154">C#</span><span class="sxs-lookup"><span data-stu-id="e3de8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3de8-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3de8-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3de8-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3de8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3de8-157">Java</span><span class="sxs-lookup"><span data-stu-id="e3de8-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3de8-158">响应</span><span class="sxs-lookup"><span data-stu-id="e3de8-158">Response</span></span>

<span data-ttu-id="e3de8-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3de8-159">The following is an example of the response.</span></span>

<span data-ttu-id="e3de8-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e3de8-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages/$entity",
  "id": "es-ES",
  "isEnabled": true,
  "displayName": "Spanish (Spain)"
}
```

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="e3de8-161">示例 2：更新 Azure AD B2C 用户流中的自定义语言</span><span class="sxs-lookup"><span data-stu-id="e3de8-161">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="e3de8-162">请求</span><span class="sxs-lookup"><span data-stu-id="e3de8-162">Request</span></span>

<span data-ttu-id="e3de8-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3de8-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="e3de8-164">响应</span><span class="sxs-lookup"><span data-stu-id="e3de8-164">Response</span></span>

<span data-ttu-id="e3de8-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3de8-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
