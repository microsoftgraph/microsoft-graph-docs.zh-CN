---
title: 创建 temporaryAccessPassAuthenticationMethod
description: 创建新的 temporaryAccessPassAuthenticationMethod 对象。
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 504b81b94252ffde5e9247e0357763e05fb806ac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049658"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="88b71-103">创建 temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88b71-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="88b71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88b71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88b71-105">在用户上 [创建新的 temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88b71-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="88b71-106">用户只能有一个临时访问传递。</span><span class="sxs-lookup"><span data-stu-id="88b71-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="88b71-107">可以在临时访问传递的开始时间和结束时间之间使用密码。</span><span class="sxs-lookup"><span data-stu-id="88b71-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="88b71-108">如果用户需要新的临时访问通道：</span><span class="sxs-lookup"><span data-stu-id="88b71-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="88b71-109">当前临时访问传递有效时 ， 管理员需要删除现有的临时访问通道，并创建用户的新传递。</span><span class="sxs-lookup"><span data-stu-id="88b71-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="88b71-110">删除有效的临时访问通道将撤消用户的会话。</span><span class="sxs-lookup"><span data-stu-id="88b71-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="88b71-111">临时访问传递过期后 - 新的临时访问传递将覆盖当前临时访问传递，并且不会撤消用户的会话。</span><span class="sxs-lookup"><span data-stu-id="88b71-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="88b71-112">权限</span><span class="sxs-lookup"><span data-stu-id="88b71-112">Permissions</span></span>

<span data-ttu-id="88b71-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88b71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="88b71-115">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="88b71-115">Permissions acting on self</span></span>

|<span data-ttu-id="88b71-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="88b71-116">Permission type</span></span>      | <span data-ttu-id="88b71-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88b71-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="88b71-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88b71-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="88b71-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88b71-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="88b71-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88b71-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88b71-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="88b71-121">Not supported.</span></span> |
| <span data-ttu-id="88b71-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="88b71-122">Application</span></span>                            | <span data-ttu-id="88b71-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="88b71-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="88b71-124">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="88b71-124">Permissions acting on other users</span></span>

|<span data-ttu-id="88b71-125">权限类型</span><span class="sxs-lookup"><span data-stu-id="88b71-125">Permission type</span></span>      | <span data-ttu-id="88b71-126">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88b71-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="88b71-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88b71-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="88b71-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b71-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="88b71-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88b71-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88b71-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="88b71-130">Not supported.</span></span> |
| <span data-ttu-id="88b71-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="88b71-131">Application</span></span>                            | <span data-ttu-id="88b71-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b71-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="88b71-133">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="88b71-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="88b71-134">全局管理员</span><span class="sxs-lookup"><span data-stu-id="88b71-134">Global admin</span></span>
* <span data-ttu-id="88b71-135">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="88b71-135">Privileged authentication admin</span></span>
* <span data-ttu-id="88b71-136">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="88b71-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="88b71-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88b71-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="88b71-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="88b71-138">Request headers</span></span>
|<span data-ttu-id="88b71-139">名称</span><span class="sxs-lookup"><span data-stu-id="88b71-139">Name</span></span>|<span data-ttu-id="88b71-140">说明</span><span class="sxs-lookup"><span data-stu-id="88b71-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88b71-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="88b71-141">Authorization</span></span>|<span data-ttu-id="88b71-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88b71-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88b71-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88b71-144">Content-Type</span></span>|<span data-ttu-id="88b71-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="88b71-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88b71-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="88b71-147">Request body</span></span>
<span data-ttu-id="88b71-148">在请求正文中，提供 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88b71-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="88b71-149">下表介绍在创建 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)时可以使用的可选属性。</span><span class="sxs-lookup"><span data-stu-id="88b71-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="88b71-150">属性</span><span class="sxs-lookup"><span data-stu-id="88b71-150">Property</span></span>|<span data-ttu-id="88b71-151">类型</span><span class="sxs-lookup"><span data-stu-id="88b71-151">Type</span></span>|<span data-ttu-id="88b71-152">说明</span><span class="sxs-lookup"><span data-stu-id="88b71-152">Description</span></span>|<span data-ttu-id="88b71-153">必需</span><span class="sxs-lookup"><span data-stu-id="88b71-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="88b71-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="88b71-154">startDateTime</span></span>|<span data-ttu-id="88b71-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88b71-155">DateTimeOffset</span></span>|<span data-ttu-id="88b71-156">temporaryAccessPass 可供使用的日期和时间（如果未设置，则创建时可以使用临时访问传递）。</span><span class="sxs-lookup"><span data-stu-id="88b71-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="88b71-157">不支持</span><span class="sxs-lookup"><span data-stu-id="88b71-157">No</span></span>|
|<span data-ttu-id="88b71-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="88b71-158">lifetimeInMinutes</span></span>|<span data-ttu-id="88b71-159">Int32</span><span class="sxs-lookup"><span data-stu-id="88b71-159">Int32</span></span>|<span data-ttu-id="88b71-160">temporaryAccessPass 的生存期，以分钟计，从创建时间开始或 startDateTime（如果已设置）。</span><span class="sxs-lookup"><span data-stu-id="88b71-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="88b71-161">最少 10 天，最多 43200 (相当于 30 天) 。</span><span class="sxs-lookup"><span data-stu-id="88b71-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="88b71-162">不支持</span><span class="sxs-lookup"><span data-stu-id="88b71-162">No</span></span>|
|<span data-ttu-id="88b71-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="88b71-163">isUsableOnce</span></span>|<span data-ttu-id="88b71-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="88b71-164">Boolean</span></span>|<span data-ttu-id="88b71-165">确定是否将传递限制为一次使用。</span><span class="sxs-lookup"><span data-stu-id="88b71-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="88b71-166">如果为 True，则传递可以使用一次，如果为 False，则临时AccessPass 生命周期内可以多次使用传递。</span><span class="sxs-lookup"><span data-stu-id="88b71-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="88b71-167">多用途临时访问 (isUsableOnce = false) ，只有在临时访问传递身份验证方法策略允许时，才能创建并用于登录。</span><span class="sxs-lookup"><span data-stu-id="88b71-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="88b71-168">不支持</span><span class="sxs-lookup"><span data-stu-id="88b71-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="88b71-169">响应</span><span class="sxs-lookup"><span data-stu-id="88b71-169">Response</span></span>

<span data-ttu-id="88b71-170">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88b71-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88b71-171">示例</span><span class="sxs-lookup"><span data-stu-id="88b71-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88b71-172">请求</span><span class="sxs-lookup"><span data-stu-id="88b71-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="88b71-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="88b71-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
  "lifetimeInMinutes": 60,
  "isUsableOnce": false
}
```
# <a name="c"></a>[<span data-ttu-id="88b71-174">C#</span><span class="sxs-lookup"><span data-stu-id="88b71-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88b71-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88b71-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88b71-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88b71-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88b71-177">Java</span><span class="sxs-lookup"><span data-stu-id="88b71-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88b71-178">响应</span><span class="sxs-lookup"><span data-stu-id="88b71-178">Response</span></span>
<span data-ttu-id="88b71-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88b71-179">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```
