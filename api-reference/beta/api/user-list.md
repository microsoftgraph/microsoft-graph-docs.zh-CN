---
title: 列出用户
description: 检索用户对象列表。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 09c296c88fc2b7ceab48018745b2686c08b8db21
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400983"
---
# <a name="list-users"></a><span data-ttu-id="1b77b-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="1b77b-103">List users</span></span>

<span data-ttu-id="1b77b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b77b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b77b-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1b77b-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="1b77b-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="1b77b-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="1b77b-107">这些 _默认_ 属性将记录在 [属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="1b77b-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="1b77b-108">要获取 _非_ 默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="1b77b-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b77b-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="1b77b-109">Permissions</span></span>

<span data-ttu-id="1b77b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b77b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b77b-112">Permission type</span></span>      | <span data-ttu-id="1b77b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b77b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b77b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b77b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b77b-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b77b-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1b77b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b77b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b77b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b77b-117">Not supported.</span></span>    |
|<span data-ttu-id="1b77b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b77b-118">Application</span></span> | <span data-ttu-id="1b77b-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b77b-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b77b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b77b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b77b-121">Optional query parameters</span></span>

<span data-ttu-id="1b77b-122">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-122">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="1b77b-123">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="1b77b-123">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="1b77b-124">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-124">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="1b77b-125">`$count` 和 `$search` 参数当前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="1b77b-125">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="1b77b-p104">某些属性无法在用户集合中返回。以下属性仅在 [检索单个用户](./user-get.md) 时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="1b77b-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="1b77b-128">个人 Microsoft 帐户不支持下列属性，且将为 `null`：**aboutMe**、**birthday**、**interests**、**mySite**，**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**streetAddress**。</span><span class="sxs-lookup"><span data-stu-id="1b77b-128">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b77b-129">请求头</span><span class="sxs-lookup"><span data-stu-id="1b77b-129">Request headers</span></span>

| <span data-ttu-id="1b77b-130">标头</span><span class="sxs-lookup"><span data-stu-id="1b77b-130">Header</span></span> | <span data-ttu-id="1b77b-131">值</span><span class="sxs-lookup"><span data-stu-id="1b77b-131">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="1b77b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b77b-132">Authorization</span></span> | <span data-ttu-id="1b77b-133">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="1b77b-133">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="1b77b-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1b77b-134">ConsistencyLevel</span></span> | <span data-ttu-id="1b77b-135">最终。</span><span class="sxs-lookup"><span data-stu-id="1b77b-135">eventual.</span></span> <span data-ttu-id="1b77b-136">当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。</span><span class="sxs-lookup"><span data-stu-id="1b77b-136">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="1b77b-137">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-137">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b77b-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b77b-138">Request body</span></span>

<span data-ttu-id="1b77b-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b77b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b77b-140">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-140">Response</span></span>

<span data-ttu-id="1b77b-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1b77b-141">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b77b-142">示例</span><span class="sxs-lookup"><span data-stu-id="1b77b-142">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="1b77b-143">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="1b77b-143">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-144">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-144">Request</span></span>

<span data-ttu-id="1b77b-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b77b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b77b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="1b77b-147">C#</span><span class="sxs-lookup"><span data-stu-id="1b77b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b77b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b77b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b77b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b77b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b77b-150">Java</span><span class="sxs-lookup"><span data-stu-id="1b77b-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1b77b-151">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-151">Response</span></span>

<span data-ttu-id="1b77b-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-152">The following is an example of the response.</span></span> 
><span data-ttu-id="1b77b-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "otherMails":["contoso1@gmail.com"],
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="1b77b-154">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="1b77b-154">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="1b77b-155">使用登录名（也称为本地帐户）查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="1b77b-155">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="1b77b-156">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="1b77b-156">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="1b77b-157">**issuerAssignedId** 的值必须是用户帐户的电子邮件地址，不能是用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-157">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="1b77b-158">如果使用了 UPN，响应将为一个空列表。</span><span class="sxs-lookup"><span data-stu-id="1b77b-158">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-159">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-159">Request</span></span>

<span data-ttu-id="1b77b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b77b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b77b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="1b77b-162">C#</span><span class="sxs-lookup"><span data-stu-id="1b77b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b77b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b77b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b77b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b77b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b77b-165">Java</span><span class="sxs-lookup"><span data-stu-id="1b77b-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1b77b-166">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-166">Response</span></span>

<span data-ttu-id="1b77b-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-167">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b77b-168">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "John Smith"
    }
  ]
}
```

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="1b77b-169">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="1b77b-169">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-170">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-170">Request</span></span>

<span data-ttu-id="1b77b-p107">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="1b77b-p107">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b77b-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b77b-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="1b77b-174">C#</span><span class="sxs-lookup"><span data-stu-id="1b77b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b77b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b77b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b77b-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b77b-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b77b-177">Java</span><span class="sxs-lookup"><span data-stu-id="1b77b-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1b77b-178">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-178">Response</span></span>

<span data-ttu-id="1b77b-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-179">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b77b-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(displayName,userPrincipalName,signInActivity)",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2017-07-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="1b77b-181">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="1b77b-181">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-182">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-182">Request</span></span>

<span data-ttu-id="1b77b-p108">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="1b77b-p108">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b77b-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b77b-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="1b77b-186">C#</span><span class="sxs-lookup"><span data-stu-id="1b77b-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b77b-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b77b-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b77b-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b77b-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b77b-189">Java</span><span class="sxs-lookup"><span data-stu-id="1b77b-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b77b-190">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-190">Response</span></span>

<span data-ttu-id="1b77b-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-191">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b77b-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-192">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity",
  "value": [
    {
      "displayName": "Eric Solomon",
      "signInActivity": {
        "lastSignInDateTime": "2017-09-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    }
  ]
}
```

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="1b77b-193">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="1b77b-193">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-194">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-194">Request</span></span>

<span data-ttu-id="1b77b-p109">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="1b77b-p109">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="1b77b-197">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-197">Response</span></span>

<span data-ttu-id="1b77b-198">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-198">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b77b-199">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z",
  "value": [
    {
      "displayName": "Adele Vance",
      "userPrincipalName": "AdeleV@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-05-04T15:35:02Z",
        "lastSignInRequestId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
      }
    },
    {
      "displayName": "Alex Wilber",
      "userPrincipalName": "AlexW@contoso.com",
      "signInActivity": {
        "lastSignInDateTime": "2019-04-29T02:16:18Z",
        "lastSignInRequestId": "90d8b3f8-712e-4f7b-aa1e-62e7ae6cbe96"
      }
    }
  ]
}
```

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="1b77b-200">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="1b77b-200">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-201">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-201">Request</span></span>

<span data-ttu-id="1b77b-202">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-202">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-203">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="1b77b-203">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="1b77b-204">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-204">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1b77b-205">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-205">Response</span></span>

<span data-ttu-id="1b77b-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-206">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1b77b-207">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="1b77b-207">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-208">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-208">Request</span></span>

<span data-ttu-id="1b77b-209">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-209">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-210">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="1b77b-210">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="1b77b-211">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-211">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1b77b-212">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-212">Response</span></span>

<span data-ttu-id="1b77b-213">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-213">The following is an example of the response.</span></span>
><span data-ttu-id="1b77b-214">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-214">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mail":"a@contoso.com",
      "mailNickname":"a_contoso.com#EXT#",
      "otherMails":["a@contoso.com"],
      "proxyAddresses":["SMTP:a@contoso.com"],
      "userPrincipalName":"a_contoso.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="1b77b-215">示例 8：使用 $filter 获取以 'a@contoso.com' 结尾的邮件的所有用户（包括返回对象的计数），结果按 userPrincipalName 排序</span><span class="sxs-lookup"><span data-stu-id="1b77b-215">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-216">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-216">Request</span></span>

<span data-ttu-id="1b77b-217">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-217">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-218">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数，并且还使用 `endsWith` 运算符。</span><span class="sxs-lookup"><span data-stu-id="1b77b-218">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters, and also uses the `endsWith` operator.</span></span> <span data-ttu-id="1b77b-219">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-219">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


# <a name="http"></a>[<span data-ttu-id="1b77b-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b77b-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1b77b-221">C#</span><span class="sxs-lookup"><span data-stu-id="1b77b-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b77b-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b77b-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b77b-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b77b-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b77b-224">Java</span><span class="sxs-lookup"><span data-stu-id="1b77b-224">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b77b-225">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-225">Response</span></span>

<span data-ttu-id="1b77b-226">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-226">The following is an example of the response.</span></span>

><span data-ttu-id="1b77b-227">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-227">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count": 1,
  "value": [
    {
      "displayName": "Grady Archie",
      "givenName": "Grady",
      "jobTitle": "Designer",
      "mail": "GradyA@contoso.com",
      "userPrincipalName": "GradyA@contoso.com",
      "id": "e8b753b5-4117-464e-9a08-713e1ff266b3"
      }
    ]
}
```

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="1b77b-228">示例 9：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="1b77b-228">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-229">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-229">Request</span></span>

<span data-ttu-id="1b77b-230">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-230">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-231">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。</span><span class="sxs-lookup"><span data-stu-id="1b77b-231">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="1b77b-232">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-232">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1b77b-233">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-233">Response</span></span>

<span data-ttu-id="1b77b-234">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-234">The following is an example of the response.</span></span>
><span data-ttu-id="1b77b-235">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-235">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    }
  ]
}

```

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="1b77b-236">示例 10：使用 $search 获取显示名称中包含字母“wa”或“to”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="1b77b-236">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-237">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-237">Request</span></span>

<span data-ttu-id="1b77b-238">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-238">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-239">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。</span><span class="sxs-lookup"><span data-stu-id="1b77b-239">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="1b77b-240">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-240">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="1b77b-241">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-241">Response</span></span>

<span data-ttu-id="1b77b-242">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-242">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b77b-243">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b77b-243">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Oscar Ward",
      "givenName":"Oscar",
      "mail":"oscarward@contoso.com",
      "mailNickname":"oscward",
      "userPrincipalName":"oscarward@contoso.com"
    },
    {
      "displayName":"contoso1",
      "mail":"'contoso1@gmail.com",
      "mailNickname":"contoso1_gmail.com#EXT#",
      "proxyAddresses":["SMTP:contoso1@gmail.com"], 
      "userPrincipalName":"contoso1_gmail.com#EXT#@microsoft.onmicrosoft.com"
    }
  ]
}
```


### <a name="example-11-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="1b77b-244">示例 11：使用 $filter为用户分配特定许可证</span><span class="sxs-lookup"><span data-stu-id="1b77b-244">Example 11: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="1b77b-245">请求</span><span class="sxs-lookup"><span data-stu-id="1b77b-245">Request</span></span>

<span data-ttu-id="1b77b-246">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b77b-246">The following is an example of the request.</span></span> <span data-ttu-id="1b77b-247">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。</span><span class="sxs-lookup"><span data-stu-id="1b77b-247">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` is in the request.</span></span> <span data-ttu-id="1b77b-248">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="1b77b-248">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="1b77b-249">响应</span><span class="sxs-lookup"><span data-stu-id="1b77b-249">Response</span></span>

<span data-ttu-id="1b77b-250">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b77b-250">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,mail,assignedLicenses)",
  "value": [
    {
      "id": "cb4954e8-467f-4a6d-a8c8-28b9034fadbc",
      "mail": "admin@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    },
    {
      "id": "81a133c2-bdf2-4e67-8755-7264366b04ee",
      "mail": "DebraB@contoso.com",
      "assignedLicenses": [
        {
          "disabledPlans": [],
          "skuId": "cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
