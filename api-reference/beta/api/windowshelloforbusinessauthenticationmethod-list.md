---
title: 列出 windowsHelloForBusinessAuthenticationMethods
description: 获取 windowsHelloForBusinessAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8891e6a6afb6f2656740122081fe86aadd7bbd0f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516370"
---
# <a name="list-windowshelloforbusinessauthenticationmethods"></a><span data-ttu-id="4c6a7-103">列出 windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="4c6a7-103">List windowsHelloForBusinessAuthenticationMethods</span></span>
<span data-ttu-id="4c6a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c6a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c6a7-105">获取 [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-105">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c6a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c6a7-106">Permissions</span></span>

<span data-ttu-id="4c6a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4c6a7-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="4c6a7-109">Permissions acting on self</span></span>

|<span data-ttu-id="4c6a7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c6a7-110">Permission type</span></span>      | <span data-ttu-id="4c6a7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4c6a7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c6a7-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c6a7-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4c6a7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c6a7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-115">Not supported.</span></span> |
| <span data-ttu-id="4c6a7-116">Application</span><span class="sxs-lookup"><span data-stu-id="4c6a7-116">Application</span></span>                            | <span data-ttu-id="4c6a7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4c6a7-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="4c6a7-118">Permissions acting on other users</span></span>

|<span data-ttu-id="4c6a7-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c6a7-119">Permission type</span></span>      | <span data-ttu-id="4c6a7-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4c6a7-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c6a7-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6a7-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4c6a7-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c6a7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c6a7-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-124">Not supported.</span></span> |
| <span data-ttu-id="4c6a7-125">Application</span><span class="sxs-lookup"><span data-stu-id="4c6a7-125">Application</span></span>                            | <span data-ttu-id="4c6a7-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6a7-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4c6a7-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="4c6a7-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4c6a7-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4c6a7-128">Global admin</span></span>
* <span data-ttu-id="4c6a7-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="4c6a7-129">Global reader</span></span>
* <span data-ttu-id="4c6a7-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="4c6a7-130">Privileged authentication admin</span></span>
* <span data-ttu-id="4c6a7-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="4c6a7-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="4c6a7-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c6a7-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c6a7-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4c6a7-133">Optional query parameters</span></span>

<span data-ttu-id="4c6a7-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c6a7-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c6a7-135">Request headers</span></span>
|<span data-ttu-id="4c6a7-136">名称</span><span class="sxs-lookup"><span data-stu-id="4c6a7-136">Name</span></span>|<span data-ttu-id="4c6a7-137">说明</span><span class="sxs-lookup"><span data-stu-id="4c6a7-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4c6a7-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c6a7-138">Authorization</span></span>|<span data-ttu-id="4c6a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c6a7-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c6a7-141">Request body</span></span>
<span data-ttu-id="4c6a7-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c6a7-143">响应</span><span class="sxs-lookup"><span data-stu-id="4c6a7-143">Response</span></span>

<span data-ttu-id="4c6a7-144">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-144">If successful, this method returns a `200 OK` response code and a collection of [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c6a7-145">示例</span><span class="sxs-lookup"><span data-stu-id="4c6a7-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c6a7-146">请求</span><span class="sxs-lookup"><span data-stu-id="4c6a7-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4c6a7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c6a7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods
```
# <a name="c"></a>[<span data-ttu-id="4c6a7-148">C#</span><span class="sxs-lookup"><span data-stu-id="4c6a7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-windowshelloforbusinessauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c6a7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c6a7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-windowshelloforbusinessauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c6a7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c6a7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-windowshelloforbusinessauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c6a7-151">Java</span><span class="sxs-lookup"><span data-stu-id="4c6a7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-windowshelloforbusinessauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4c6a7-152">响应</span><span class="sxs-lookup"><span data-stu-id="4c6a7-152">Response</span></span>
<span data-ttu-id="4c6a7-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4c6a7-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsHelloForBusinessAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
      "displayName": "Jordan's Surface Book",
      "createdDateTime": "2020-11-27T23:12:49Z",
      "keyStrength": "normal"
    },
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "e6dab818-e68d-433e-89d5-547357870cb2",
      "displayName": "New Surface Duo",
      "createdDateTime": "2020-12-25T02:20:13Z",
      "keyStrength": "normal"
    }
  ]
}
```

