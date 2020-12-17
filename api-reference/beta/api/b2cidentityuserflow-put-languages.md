---
title: 创建语言
description: 在 Azure AD B2C 用户流中创建自定义语言。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a45e19b056b040d700bdb246e07eefee471342b2
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706230"
---
# <a name="create-languages"></a><span data-ttu-id="3a23b-103">创建语言</span><span class="sxs-lookup"><span data-stu-id="3a23b-103">Create languages</span></span>

<span data-ttu-id="3a23b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a23b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a23b-105">此方法用于在 Azure AD B2C 用户流中创建或更新自定义语言。</span><span class="sxs-lookup"><span data-stu-id="3a23b-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="3a23b-106">**注意：** 必须先在 Azure AD B2C 用户流中启用语言自定义，然后才能创建自定义语言。</span><span class="sxs-lookup"><span data-stu-id="3a23b-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="3a23b-107">有关详细信息，请参阅[Update b2cIdentityUserFlow。](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="3a23b-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a23b-108">权限</span><span class="sxs-lookup"><span data-stu-id="3a23b-108">Permissions</span></span>

<span data-ttu-id="3a23b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a23b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a23b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a23b-111">Permission type</span></span>      | <span data-ttu-id="3a23b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a23b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a23b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a23b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a23b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a23b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3a23b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a23b-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3a23b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a23b-116">Not supported.</span></span>|
|<span data-ttu-id="3a23b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a23b-117">Application</span></span>|<span data-ttu-id="3a23b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a23b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3a23b-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="3a23b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3a23b-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3a23b-120">Global administrator</span></span>
* <span data-ttu-id="3a23b-121">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="3a23b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3a23b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a23b-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3a23b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a23b-123">Request headers</span></span>

|<span data-ttu-id="3a23b-124">名称</span><span class="sxs-lookup"><span data-stu-id="3a23b-124">Name</span></span>|<span data-ttu-id="3a23b-125">说明</span><span class="sxs-lookup"><span data-stu-id="3a23b-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a23b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a23b-126">Authorization</span></span>|<span data-ttu-id="3a23b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a23b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3a23b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a23b-129">Content-Type</span></span>|<span data-ttu-id="3a23b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3a23b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a23b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a23b-132">Request body</span></span>

<span data-ttu-id="3a23b-133">在请求正文中，提供 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a23b-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="3a23b-134">下表显示创建 [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md)时可以选择提供的属性。</span><span class="sxs-lookup"><span data-stu-id="3a23b-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="3a23b-135">属性</span><span class="sxs-lookup"><span data-stu-id="3a23b-135">Property</span></span>|<span data-ttu-id="3a23b-136">类型</span><span class="sxs-lookup"><span data-stu-id="3a23b-136">Type</span></span>|<span data-ttu-id="3a23b-137">说明</span><span class="sxs-lookup"><span data-stu-id="3a23b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a23b-138">id</span><span class="sxs-lookup"><span data-stu-id="3a23b-138">id</span></span>|<span data-ttu-id="3a23b-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3a23b-139">String</span></span>|<span data-ttu-id="3a23b-140">语言的标识符。</span><span class="sxs-lookup"><span data-stu-id="3a23b-140">The identifier of the language.</span></span> <span data-ttu-id="3a23b-141">此字段符合语言 ID 标记 [RFC 5646，](https://tools.ietf.org/html/rfc5646) 并且必须是记录的语言 ID。</span><span class="sxs-lookup"><span data-stu-id="3a23b-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="3a23b-142">如果在请求正文中提供，则它必须与请求 URL 中提供的标识相匹配。</span><span class="sxs-lookup"><span data-stu-id="3a23b-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="3a23b-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3a23b-143">isEnabled</span></span>|<span data-ttu-id="3a23b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a23b-144">Boolean</span></span>|<span data-ttu-id="3a23b-145">指示是否在用户流中启用语言。</span><span class="sxs-lookup"><span data-stu-id="3a23b-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="3a23b-146">如果请求中未提供，isEnabled 将设置为"true"。</span><span class="sxs-lookup"><span data-stu-id="3a23b-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="3a23b-147">响应</span><span class="sxs-lookup"><span data-stu-id="3a23b-147">Response</span></span>

<span data-ttu-id="3a23b-148">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a23b-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a23b-149">示例</span><span class="sxs-lookup"><span data-stu-id="3a23b-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="3a23b-150">示例 1：在 Azure AD B2C 用户流中创建自定义语言</span><span class="sxs-lookup"><span data-stu-id="3a23b-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="3a23b-151">请求</span><span class="sxs-lookup"><span data-stu-id="3a23b-151">Request</span></span>

<span data-ttu-id="3a23b-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3a23b-152">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="3a23b-153">响应</span><span class="sxs-lookup"><span data-stu-id="3a23b-153">Response</span></span>

<span data-ttu-id="3a23b-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3a23b-154">The following is an example of the response.</span></span>

<span data-ttu-id="3a23b-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3a23b-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="3a23b-156">示例 2：更新 Azure AD B2C 用户流中的自定义语言</span><span class="sxs-lookup"><span data-stu-id="3a23b-156">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="3a23b-157">请求</span><span class="sxs-lookup"><span data-stu-id="3a23b-157">Request</span></span>

<span data-ttu-id="3a23b-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3a23b-158">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="3a23b-159">响应</span><span class="sxs-lookup"><span data-stu-id="3a23b-159">Response</span></span>

<span data-ttu-id="3a23b-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3a23b-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
