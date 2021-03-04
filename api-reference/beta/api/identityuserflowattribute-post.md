---
title: 创建 identityUserFlowAttribute
description: 创建新的 identityUserFlowAttribute 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f6cdbf3d22e7b51e656e3dbe3d44180232a1467b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435252"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="f9947-103">创建 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="f9947-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="f9947-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9947-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9947-105">创建新的 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9947-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9947-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9947-106">Permissions</span></span>

<span data-ttu-id="f9947-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9947-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9947-109">Permission type</span></span>      | <span data-ttu-id="f9947-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9947-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9947-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9947-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9947-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9947-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f9947-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9947-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f9947-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9947-114">Not supported.</span></span>|
|<span data-ttu-id="f9947-115">Application</span><span class="sxs-lookup"><span data-stu-id="f9947-115">Application</span></span>|<span data-ttu-id="f9947-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9947-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f9947-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f9947-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f9947-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f9947-118">Global administrator</span></span>
* <span data-ttu-id="f9947-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="f9947-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f9947-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9947-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="f9947-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9947-121">Request headers</span></span>

|<span data-ttu-id="f9947-122">名称</span><span class="sxs-lookup"><span data-stu-id="f9947-122">Name</span></span>|<span data-ttu-id="f9947-123">说明</span><span class="sxs-lookup"><span data-stu-id="f9947-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f9947-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9947-124">Authorization</span></span>|<span data-ttu-id="f9947-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9947-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f9947-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9947-127">Content-Type</span></span>|<span data-ttu-id="f9947-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f9947-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9947-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9947-130">Request body</span></span>

<span data-ttu-id="f9947-131">在请求正文中，提供 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9947-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="f9947-132">属性</span><span class="sxs-lookup"><span data-stu-id="f9947-132">Property</span></span>|<span data-ttu-id="f9947-133">类型</span><span class="sxs-lookup"><span data-stu-id="f9947-133">Type</span></span>|<span data-ttu-id="f9947-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9947-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9947-135">id</span><span class="sxs-lookup"><span data-stu-id="f9947-135">id</span></span>|<span data-ttu-id="f9947-136">String</span><span class="sxs-lookup"><span data-stu-id="f9947-136">String</span></span>|<span data-ttu-id="f9947-137">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="f9947-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="f9947-138">这是自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="f9947-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="f9947-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f9947-139">displayName</span></span>|<span data-ttu-id="f9947-140">String</span><span class="sxs-lookup"><span data-stu-id="f9947-140">String</span></span>|<span data-ttu-id="f9947-141">用户显示名称属性的属性值。</span><span class="sxs-lookup"><span data-stu-id="f9947-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="f9947-142">说明</span><span class="sxs-lookup"><span data-stu-id="f9947-142">description</span></span>|<span data-ttu-id="f9947-143">String</span><span class="sxs-lookup"><span data-stu-id="f9947-143">String</span></span>|<span data-ttu-id="f9947-144">用户流属性的说明。</span><span class="sxs-lookup"><span data-stu-id="f9947-144">The description of the user flow attribute.</span></span> <span data-ttu-id="f9947-145">它在注册时显示给用户。</span><span class="sxs-lookup"><span data-stu-id="f9947-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="f9947-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="f9947-146">userFlowAttributeType</span></span>|<span data-ttu-id="f9947-147">String</span><span class="sxs-lookup"><span data-stu-id="f9947-147">String</span></span>|<span data-ttu-id="f9947-148">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="f9947-148">The type of the user flow attribute.</span></span> <span data-ttu-id="f9947-149">这是自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="f9947-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="f9947-150">根据属性的类型，此属性的值将为 `builtIn` 或 `custom` 。</span><span class="sxs-lookup"><span data-stu-id="f9947-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="f9947-151">DataType</span><span class="sxs-lookup"><span data-stu-id="f9947-151">dataType</span></span>|<span data-ttu-id="f9947-152">String</span><span class="sxs-lookup"><span data-stu-id="f9947-152">String</span></span>|<span data-ttu-id="f9947-153">用户数据类型属性的属性值。</span><span class="sxs-lookup"><span data-stu-id="f9947-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="f9947-154">创建自定义用户流属性后，无法修改此属性。</span><span class="sxs-lookup"><span data-stu-id="f9947-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="f9947-155">dataType **支持的值** 包括：</span><span class="sxs-lookup"><span data-stu-id="f9947-155">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="f9947-156">`string` ： 表示 identityUserFlowAttribute 的 dataType 是字符串。</span><span class="sxs-lookup"><span data-stu-id="f9947-156">`string` : denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="f9947-157">`boolean` ： 表示 identityUserFlowAttribute 的 dataType 为布尔值。</span><span class="sxs-lookup"><span data-stu-id="f9947-157">`boolean` : denotes that the dataType for the identityUserFlowAttribute is a boolean.</span></span></li><li><span data-ttu-id="f9947-158">`int64` ： 表示 identityUserFlowAttribute 的 dataType 是一个整数。</span><span class="sxs-lookup"><span data-stu-id="f9947-158">`int64` : denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="response"></a><span data-ttu-id="f9947-159">响应</span><span class="sxs-lookup"><span data-stu-id="f9947-159">Response</span></span>

<span data-ttu-id="f9947-160">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9947-160">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="f9947-161">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="f9947-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="f9947-162">示例</span><span class="sxs-lookup"><span data-stu-id="f9947-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9947-163">请求</span><span class="sxs-lookup"><span data-stu-id="f9947-163">Request</span></span>

<span data-ttu-id="f9947-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f9947-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9947-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9947-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[<span data-ttu-id="f9947-166">C#</span><span class="sxs-lookup"><span data-stu-id="f9947-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9947-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9947-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9947-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9947-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9947-169">Java</span><span class="sxs-lookup"><span data-stu-id="f9947-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9947-170">响应</span><span class="sxs-lookup"><span data-stu-id="f9947-170">Response</span></span>

<span data-ttu-id="f9947-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f9947-171">The following is an example of the response.</span></span>

<span data-ttu-id="f9947-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9947-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
