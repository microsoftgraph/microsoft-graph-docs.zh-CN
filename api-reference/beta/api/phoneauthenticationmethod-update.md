---
title: 更新 phoneAuthenticationMethod
description: 更新与 phoneAuthenticationMethod 对象关联的电话号码。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae9f5bc036fd75e72bc7d698aa715447f1be552f
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796624"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="4f6e2-103">更新 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f6e2-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="4f6e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f6e2-105">更新与电话身份验证方法 [相关联的电话号码](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="4f6e2-106">你无法更改电话的类型。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-106">You can't change a phone's type.</span></span> <span data-ttu-id="4f6e2-107">若要更改电话的类型，请添加所需类型的新号码，然后删除具有原始类型的对象。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="4f6e2-108">如果策略允许用户使用短信登录，并且号码已更改，系统将尝试注册号码 `mobile` 以用于该系统。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f6e2-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f6e2-109">Permissions</span></span>

<span data-ttu-id="4f6e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4f6e2-112">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="4f6e2-112">Permissions acting on self</span></span>

|<span data-ttu-id="4f6e2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f6e2-113">Permission type</span></span>      | <span data-ttu-id="4f6e2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4f6e2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f6e2-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f6e2-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4f6e2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6e2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-118">Not supported.</span></span> |
| <span data-ttu-id="4f6e2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f6e2-119">Application</span></span>                            | <span data-ttu-id="4f6e2-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4f6e2-121">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="4f6e2-121">Permissions acting on other users</span></span>

|<span data-ttu-id="4f6e2-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f6e2-122">Permission type</span></span>      | <span data-ttu-id="4f6e2-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="4f6e2-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f6e2-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6e2-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4f6e2-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6e2-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6e2-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-127">Not supported.</span></span> |
| <span data-ttu-id="4f6e2-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f6e2-128">Application</span></span>                            | <span data-ttu-id="4f6e2-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6e2-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4f6e2-130">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="4f6e2-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4f6e2-131">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4f6e2-131">Global admin</span></span>
* <span data-ttu-id="4f6e2-132">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4f6e2-132">Privileged authentication admin</span></span>
* <span data-ttu-id="4f6e2-133">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4f6e2-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4f6e2-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f6e2-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4f6e2-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f6e2-135">Request headers</span></span>

| <span data-ttu-id="4f6e2-136">名称</span><span class="sxs-lookup"><span data-stu-id="4f6e2-136">Name</span></span>       | <span data-ttu-id="4f6e2-137">说明</span><span class="sxs-lookup"><span data-stu-id="4f6e2-137">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4f6e2-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f6e2-138">Authorization</span></span> | <span data-ttu-id="4f6e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f6e2-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="4f6e2-141">Content-type</span></span>  | <span data-ttu-id="4f6e2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4f6e2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f6e2-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f6e2-144">Request body</span></span>

<span data-ttu-id="4f6e2-145">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-145">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4f6e2-146">请求正文中未包含的现有属性将基于其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-146">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="4f6e2-147">属性</span><span class="sxs-lookup"><span data-stu-id="4f6e2-147">Property</span></span>     | <span data-ttu-id="4f6e2-148">类型</span><span class="sxs-lookup"><span data-stu-id="4f6e2-148">Type</span></span>        | <span data-ttu-id="4f6e2-149">说明</span><span class="sxs-lookup"><span data-stu-id="4f6e2-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f6e2-150">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4f6e2-150">phoneNumber</span></span>|<span data-ttu-id="4f6e2-151">String</span><span class="sxs-lookup"><span data-stu-id="4f6e2-151">String</span></span>|<span data-ttu-id="4f6e2-152">发短信或呼叫进行身份验证的电话号码。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-152">The phone number to text or call for authentication.</span></span> <span data-ttu-id="4f6e2-153">电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机是可选的。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-153">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="4f6e2-154">例如，+1 5555551234 或 +1 5555551234x123 有效。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-154">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="4f6e2-155">如果数字与所需格式不匹配，则创建/更新时将拒绝数字。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-155">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="4f6e2-156">phoneType</span><span class="sxs-lookup"><span data-stu-id="4f6e2-156">phoneType</span></span>|<span data-ttu-id="4f6e2-157">string</span><span class="sxs-lookup"><span data-stu-id="4f6e2-157">string</span></span>| <span data-ttu-id="4f6e2-158">可能的值是： `mobile` ， `alternateMobile` 或 `office` 。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-158">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="4f6e2-159">响应</span><span class="sxs-lookup"><span data-stu-id="4f6e2-159">Response</span></span>

<span data-ttu-id="4f6e2-160">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-160">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f6e2-161">示例</span><span class="sxs-lookup"><span data-stu-id="4f6e2-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f6e2-162">请求</span><span class="sxs-lookup"><span data-stu-id="4f6e2-162">Request</span></span>

<span data-ttu-id="4f6e2-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f6e2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f6e2-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[<span data-ttu-id="4f6e2-165">C#</span><span class="sxs-lookup"><span data-stu-id="4f6e2-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f6e2-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f6e2-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f6e2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f6e2-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f6e2-168">Java</span><span class="sxs-lookup"><span data-stu-id="4f6e2-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f6e2-169">响应</span><span class="sxs-lookup"><span data-stu-id="4f6e2-169">Response</span></span>

<span data-ttu-id="4f6e2-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-170">The following is an example of the response.</span></span>

> <span data-ttu-id="4f6e2-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f6e2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
