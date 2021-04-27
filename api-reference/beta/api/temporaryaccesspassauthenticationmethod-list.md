---
title: 列出 temporaryAccessPassAuthenticationMethods
description: 获取 temporaryAccessPassAuthenticationMethod 对象及其属性的列表。
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 42af0e77a33bc4cc569cf57ad156c3b8f49a2c15
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049665"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a><span data-ttu-id="77a2f-103">列出 temporaryAccessPassAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="77a2f-103">List temporaryAccessPassAuthenticationMethods</span></span>
<span data-ttu-id="77a2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77a2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77a2f-105">检索用户的临时 [AccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="77a2f-105">Retrieve a list of a user's [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  objects and their properties.</span></span> <span data-ttu-id="77a2f-106">此调用将仅返回单个对象，因为只能为用户设置一个临时访问传递方法。</span><span class="sxs-lookup"><span data-stu-id="77a2f-106">This call will only return a single object as only one Temporary Access Pass method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="77a2f-107">权限</span><span class="sxs-lookup"><span data-stu-id="77a2f-107">Permissions</span></span>
<span data-ttu-id="77a2f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77a2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="77a2f-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="77a2f-110">Permissions acting on self</span></span>

|<span data-ttu-id="77a2f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77a2f-111">Permission type</span></span>      | <span data-ttu-id="77a2f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77a2f-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="77a2f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77a2f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="77a2f-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77a2f-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="77a2f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77a2f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a2f-116">Not supported.</span></span> |
| <span data-ttu-id="77a2f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77a2f-117">Application</span></span>                            | <span data-ttu-id="77a2f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a2f-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="77a2f-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="77a2f-119">Permissions acting on other users</span></span>

|<span data-ttu-id="77a2f-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="77a2f-120">Permission type</span></span>      | <span data-ttu-id="77a2f-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77a2f-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="77a2f-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77a2f-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="77a2f-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a2f-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="77a2f-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77a2f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a2f-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a2f-125">Not supported.</span></span> |
| <span data-ttu-id="77a2f-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="77a2f-126">Application</span></span>                            | <span data-ttu-id="77a2f-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77a2f-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |


<span data-ttu-id="77a2f-128">对于管理员正在操作其他用户的委派方案，管理员需要下列角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="77a2f-128">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="77a2f-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="77a2f-129">Global admin</span></span>
* <span data-ttu-id="77a2f-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="77a2f-130">Global reader</span></span>
* <span data-ttu-id="77a2f-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="77a2f-131">Privileged authentication admin</span></span>
* <span data-ttu-id="77a2f-132">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="77a2f-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="77a2f-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77a2f-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77a2f-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77a2f-134">Optional query parameters</span></span>
<span data-ttu-id="77a2f-135">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="77a2f-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77a2f-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="77a2f-136">Request headers</span></span>
|<span data-ttu-id="77a2f-137">名称</span><span class="sxs-lookup"><span data-stu-id="77a2f-137">Name</span></span>|<span data-ttu-id="77a2f-138">说明</span><span class="sxs-lookup"><span data-stu-id="77a2f-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77a2f-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a2f-139">Authorization</span></span>|<span data-ttu-id="77a2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77a2f-p103">Bearer {token}. Required.</span></span>|

## <a name="request"></a><span data-ttu-id="77a2f-142">请求</span><span class="sxs-lookup"><span data-stu-id="77a2f-142">Request</span></span> 
<span data-ttu-id="77a2f-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77a2f-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77a2f-144">响应</span><span class="sxs-lookup"><span data-stu-id="77a2f-144">Response</span></span>

<span data-ttu-id="77a2f-145">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77a2f-145">If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.</span></span>  <span data-ttu-id="77a2f-146">此调用将仅返回一个对象，因为只能为用户设置一个 **temporaryAccessPassAuthenticationMethod。**</span><span class="sxs-lookup"><span data-stu-id="77a2f-146">This call will only return a single object because only one **temporaryAccessPassAuthenticationMethod** can be set on users.</span></span>

## <a name="examples"></a><span data-ttu-id="77a2f-147">示例</span><span class="sxs-lookup"><span data-stu-id="77a2f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77a2f-148">请求</span><span class="sxs-lookup"><span data-stu-id="77a2f-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="77a2f-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="77a2f-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```
# <a name="c"></a>[<span data-ttu-id="77a2f-150">C#</span><span class="sxs-lookup"><span data-stu-id="77a2f-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77a2f-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a2f-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77a2f-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77a2f-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77a2f-153">Java</span><span class="sxs-lookup"><span data-stu-id="77a2f-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="77a2f-154">响应</span><span class="sxs-lookup"><span data-stu-id="77a2f-154">Response</span></span>
<span data-ttu-id="77a2f-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77a2f-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
      "id": "String",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer",
      "isUsableOnce": "Boolean",
      "isUsable": "Boolean",
      "methodUsabilityReason": "String"
    }
  ]
}
```
