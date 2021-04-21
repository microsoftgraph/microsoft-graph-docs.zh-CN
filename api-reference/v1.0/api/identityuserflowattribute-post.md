---
title: 创建 identityUserFlowAttribute
description: 创建新的 identityUserFlowAttribute 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: ac068b6956c48f67245f6c93dca764cb575e3ba3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920843"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="a96dc-103">创建 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="a96dc-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="a96dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a96dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a96dc-105">创建新的 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a96dc-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a96dc-106">权限</span><span class="sxs-lookup"><span data-stu-id="a96dc-106">Permissions</span></span>

<span data-ttu-id="a96dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a96dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a96dc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a96dc-109">Permission type</span></span>      | <span data-ttu-id="a96dc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a96dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a96dc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a96dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a96dc-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96dc-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a96dc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a96dc-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a96dc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a96dc-114">Not supported.</span></span>|
|<span data-ttu-id="a96dc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a96dc-115">Application</span></span>|<span data-ttu-id="a96dc-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96dc-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a96dc-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="a96dc-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a96dc-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a96dc-118">Global administrator</span></span>
* <span data-ttu-id="a96dc-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="a96dc-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a96dc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a96dc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="a96dc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a96dc-121">Request headers</span></span>

|<span data-ttu-id="a96dc-122">名称</span><span class="sxs-lookup"><span data-stu-id="a96dc-122">Name</span></span>|<span data-ttu-id="a96dc-123">说明</span><span class="sxs-lookup"><span data-stu-id="a96dc-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a96dc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a96dc-124">Authorization</span></span>|<span data-ttu-id="a96dc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a96dc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a96dc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a96dc-127">Content-Type</span></span>|<span data-ttu-id="a96dc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a96dc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a96dc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a96dc-130">Request body</span></span>

<span data-ttu-id="a96dc-131">在请求正文中，提供 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a96dc-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="a96dc-132">属性</span><span class="sxs-lookup"><span data-stu-id="a96dc-132">Property</span></span>|<span data-ttu-id="a96dc-133">类型</span><span class="sxs-lookup"><span data-stu-id="a96dc-133">Type</span></span>|<span data-ttu-id="a96dc-134">说明</span><span class="sxs-lookup"><span data-stu-id="a96dc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a96dc-135">id</span><span class="sxs-lookup"><span data-stu-id="a96dc-135">id</span></span>|<span data-ttu-id="a96dc-136">String</span><span class="sxs-lookup"><span data-stu-id="a96dc-136">String</span></span>|<span data-ttu-id="a96dc-137">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="a96dc-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="a96dc-138">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="a96dc-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="a96dc-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a96dc-139">displayName</span></span>|<span data-ttu-id="a96dc-140">String</span><span class="sxs-lookup"><span data-stu-id="a96dc-140">String</span></span>|<span data-ttu-id="a96dc-141">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a96dc-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="a96dc-142">说明</span><span class="sxs-lookup"><span data-stu-id="a96dc-142">description</span></span>|<span data-ttu-id="a96dc-143">String</span><span class="sxs-lookup"><span data-stu-id="a96dc-143">String</span></span>|<span data-ttu-id="a96dc-144">用户流属性的说明。</span><span class="sxs-lookup"><span data-stu-id="a96dc-144">The description of the user flow attribute.</span></span> <span data-ttu-id="a96dc-145">注册时，它向用户显示。</span><span class="sxs-lookup"><span data-stu-id="a96dc-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="a96dc-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="a96dc-146">userFlowAttributeType</span></span>|<span data-ttu-id="a96dc-147">String</span><span class="sxs-lookup"><span data-stu-id="a96dc-147">String</span></span>|<span data-ttu-id="a96dc-148">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="a96dc-148">The type of the user flow attribute.</span></span> <span data-ttu-id="a96dc-149">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="a96dc-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="a96dc-150">此属性的值将是 `builtIn` 或 `custom`，具体取决于属性的类型。</span><span class="sxs-lookup"><span data-stu-id="a96dc-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="a96dc-151">DataType</span><span class="sxs-lookup"><span data-stu-id="a96dc-151">dataType</span></span>|<span data-ttu-id="a96dc-152">String</span><span class="sxs-lookup"><span data-stu-id="a96dc-152">String</span></span>|<span data-ttu-id="a96dc-153">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="a96dc-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="a96dc-154">一旦创建自定义用户流属性，就无法对其进行修改。</span><span class="sxs-lookup"><span data-stu-id="a96dc-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="a96dc-155">**dataType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="a96dc-155">The supported values for **dataType** are:</span></span><br/><ul><li>`string` </li><li>`boolean`</li><li>`int64`</li></ul>|

## <a name="response"></a><span data-ttu-id="a96dc-156">响应</span><span class="sxs-lookup"><span data-stu-id="a96dc-156">Response</span></span>

<span data-ttu-id="a96dc-157">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a96dc-157">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="a96dc-158">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="a96dc-158">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="a96dc-159">示例</span><span class="sxs-lookup"><span data-stu-id="a96dc-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a96dc-160">请求</span><span class="sxs-lookup"><span data-stu-id="a96dc-160">Request</span></span>

<span data-ttu-id="a96dc-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a96dc-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a96dc-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="a96dc-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[<span data-ttu-id="a96dc-163">C#</span><span class="sxs-lookup"><span data-stu-id="a96dc-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a96dc-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a96dc-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a96dc-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a96dc-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a96dc-166">Java</span><span class="sxs-lookup"><span data-stu-id="a96dc-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a96dc-167">响应</span><span class="sxs-lookup"><span data-stu-id="a96dc-167">Response</span></span>

<span data-ttu-id="a96dc-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a96dc-168">The following is an example of the response.</span></span>

<span data-ttu-id="a96dc-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a96dc-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
