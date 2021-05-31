---
title: 列出用户
description: 检索用户对象列表。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2636830f993626cc2d220c5a09543640f8da181f
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703543"
---
# <a name="list-users"></a><span data-ttu-id="9ed55-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="9ed55-103">List users</span></span>

<span data-ttu-id="9ed55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ed55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed55-105">检索 [user](../resources/user.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9ed55-105">Retrieve a list of [user](../resources/user.md) objects.</span></span>

<span data-ttu-id="9ed55-106">默认情况下，此操作仅返回每位用户较常用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="9ed55-106">This operation returns by default only a subset of the more commonly used properties for each user.</span></span> <span data-ttu-id="9ed55-107">这些 _默认_ 属性将记录在 [属性](../resources/user.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="9ed55-107">These _default_ properties are noted in the [Properties](../resources/user.md#properties) section.</span></span> <span data-ttu-id="9ed55-108">要获取 _非_ 默认返回的属性，请对用户执行 [GET](user-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="9ed55-108">To get properties that are _not_ returned by default, do a [GET operation](user-get.md) for the user and specify the properties in a `$select` OData query option.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed55-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ed55-109">Permissions</span></span>

<span data-ttu-id="9ed55-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ed55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed55-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ed55-112">Permission type</span></span>      | <span data-ttu-id="9ed55-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ed55-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed55-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed55-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed55-115">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ed55-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9ed55-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed55-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed55-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ed55-117">Not supported.</span></span>    |
|<span data-ttu-id="9ed55-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ed55-118">Application</span></span> | <span data-ttu-id="9ed55-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed55-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed55-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ed55-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ed55-121">Optional query parameters</span></span>

<span data-ttu-id="9ed55-122">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="9ed55-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9ed55-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="9ed55-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9ed55-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="9ed55-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9ed55-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="9ed55-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> <span data-ttu-id="9ed55-126">`$count` 和 `$search` 参数当前在 Azure AD B2C 租户中不可用。</span><span class="sxs-lookup"><span data-stu-id="9ed55-126">The `$count` and `$search` parameters are currently not available in Azure AD B2C tenants.</span></span>

<span data-ttu-id="9ed55-p104">某些属性无法在用户集合中返回。以下属性仅在 [检索单个用户](./user-get.md) 时受支持：**aboutMe**、**birthday**、**hireDate**、**interests**、**mySite**、**pastProjects**、**preferredName**、**responsibilities**、**schools**、**skills**、**mailboxSettings**。</span><span class="sxs-lookup"><span data-stu-id="9ed55-p104">Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving a single user](./user-get.md): **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **mailboxSettings**.</span></span>

<span data-ttu-id="9ed55-129">个人 Microsoft 帐户不支持下列属性，并且将 `null`： **关于Me**、 **生日**、 **感兴趣的**、 **mySite**， **pastProj 主要**、 **首选名称**、 **、**、 **学校**、 **技能**、 **街道地址**。</span><span class="sxs-lookup"><span data-stu-id="9ed55-129">The following properties are not supported in personal Microsoft accounts and will be `null`: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, **skills**, **streetAddress**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ed55-130">请求头</span><span class="sxs-lookup"><span data-stu-id="9ed55-130">Request headers</span></span>

| <span data-ttu-id="9ed55-131">标头</span><span class="sxs-lookup"><span data-stu-id="9ed55-131">Header</span></span> | <span data-ttu-id="9ed55-132">值</span><span class="sxs-lookup"><span data-stu-id="9ed55-132">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="9ed55-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed55-133">Authorization</span></span> | <span data-ttu-id="9ed55-134">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="9ed55-134">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="9ed55-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9ed55-135">ConsistencyLevel</span></span> | <span data-ttu-id="9ed55-136">最终。</span><span class="sxs-lookup"><span data-stu-id="9ed55-136">eventual.</span></span> <span data-ttu-id="9ed55-137">`$count` 使用 `$search`时、将 `$filter` 与 `$orderby` 查询参数一同使用时，或者将 `$filter` 与 `endsWith` 运算符一起使用时，和要求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-137">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter, or `$filter` with the `endsWith` logical operator.</span></span> <span data-ttu-id="9ed55-138">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="9ed55-138">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed55-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ed55-139">Request body</span></span>

<span data-ttu-id="9ed55-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ed55-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ed55-141">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-141">Response</span></span>

<span data-ttu-id="9ed55-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9ed55-142">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ed55-143">示例</span><span class="sxs-lookup"><span data-stu-id="9ed55-143">Examples</span></span>

### <a name="example-1-get-all-users"></a><span data-ttu-id="9ed55-144">示例 1：列出所有用户</span><span class="sxs-lookup"><span data-stu-id="9ed55-144">Example 1: Get all users</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-145">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-145">Request</span></span>

<span data-ttu-id="9ed55-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed55-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed55-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users
```
# <a name="c"></a>[<span data-ttu-id="9ed55-148">C#</span><span class="sxs-lookup"><span data-stu-id="9ed55-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed55-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed55-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed55-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed55-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed55-151">Java</span><span class="sxs-lookup"><span data-stu-id="9ed55-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9ed55-152">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-152">Response</span></span>

<span data-ttu-id="9ed55-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-153">The following is an example of the response.</span></span> 
><span data-ttu-id="9ed55-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-user-account-using-a-sign-in-name"></a><span data-ttu-id="9ed55-155">示例 2：使用登录名创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="9ed55-155">Example 2: Get a user account using a sign-in name</span></span>

<span data-ttu-id="9ed55-156">使用登录名（也称为本地帐户）查找用户帐户。</span><span class="sxs-lookup"><span data-stu-id="9ed55-156">Find a user account using a sign-in name (also known as a local account).</span></span>

>[!NOTE]
><span data-ttu-id="9ed55-157">根据 **identities** 进行筛选时，必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="9ed55-157">When filtering on **identities**, you must supply both **issuer** and **issuerAssignedId**.</span></span> <span data-ttu-id="9ed55-158">**issuerAssignedId** 的值必须是用户帐户的电子邮件地址，不能是用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="9ed55-158">The value of **issuerAssignedId** must be the email address of the user account, not the user principal name (UPN).</span></span> <span data-ttu-id="9ed55-159">如果使用了 UPN，响应将为一个空列表。</span><span class="sxs-lookup"><span data-stu-id="9ed55-159">If a UPN is used, the response will be an empty list.</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-160">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-160">Request</span></span>

<span data-ttu-id="9ed55-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed55-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed55-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signinname_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,id&$filter=identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="9ed55-163">C#</span><span class="sxs-lookup"><span data-stu-id="9ed55-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signinname-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed55-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed55-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signinname-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed55-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed55-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signinname-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed55-166">Java</span><span class="sxs-lookup"><span data-stu-id="9ed55-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signinname-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9ed55-167">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-167">Response</span></span>

<span data-ttu-id="9ed55-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-168">The following is an example of the response.</span></span> 
> <span data-ttu-id="9ed55-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-users-including-their-last-sign-in-time"></a><span data-ttu-id="9ed55-170">示例3：列出用户，包括其上次登录时间</span><span class="sxs-lookup"><span data-stu-id="9ed55-170">Example 3: Get users including their last sign-in time</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-171">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-171">Request</span></span>

<span data-ttu-id="9ed55-p107">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="9ed55-p107">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ed55-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed55-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=displayName,userPrincipalName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9ed55-175">C#</span><span class="sxs-lookup"><span data-stu-id="9ed55-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed55-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed55-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed55-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed55-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed55-178">Java</span><span class="sxs-lookup"><span data-stu-id="9ed55-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9ed55-179">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-179">Response</span></span>

<span data-ttu-id="9ed55-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-180">The following is an example of the response.</span></span> 
> <span data-ttu-id="9ed55-181">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-181">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-list-the-last-sign-in-time-of-users-with-a-specific-display-name"></a><span data-ttu-id="9ed55-182">示例 4：列出具有特定显示名称的用户的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="9ed55-182">Example 4: List the last sign-in time of users with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-183">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-183">Request</span></span>

<span data-ttu-id="9ed55-p108">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="9ed55-p108">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed55-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed55-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_last_time_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'Eric')&$select=displayName,signInActivity
```
# <a name="c"></a>[<span data-ttu-id="9ed55-187">C#</span><span class="sxs-lookup"><span data-stu-id="9ed55-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-last-time-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed55-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed55-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-last-time-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed55-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed55-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-last-time-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed55-190">Java</span><span class="sxs-lookup"><span data-stu-id="9ed55-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-last-time-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ed55-191">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-191">Response</span></span>

<span data-ttu-id="9ed55-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-192">The following is an example of the response.</span></span> 
> <span data-ttu-id="9ed55-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-193">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-list-the-last-sign-in-time-of-users-in-a-specific-time-range"></a><span data-ttu-id="9ed55-194">示例 5：列出用户在特定时间范围内的上次登录时间</span><span class="sxs-lookup"><span data-stu-id="9ed55-194">Example 5: List the last sign-in time of users in a specific time range</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-195">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-195">Request</span></span>

<span data-ttu-id="9ed55-p109">以下是请求示例。有关" **signInActivity** 属性的详细信息，需要 Azure AD Premium P1/P2 许可证和 AuditLog.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="9ed55-p109">The following is an example of the request. Details for the **signInActivity** property require an Azure AD Premium P1/P2 license and the AuditLog.Read.All permission.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_signin_last_time_range"
}-->
```http
GET https://graph.microsoft.com/beta/users?filter=signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="9ed55-198">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-198">Response</span></span>

<span data-ttu-id="9ed55-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-199">The following is an example of the response.</span></span> 
> <span data-ttu-id="9ed55-200">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-200">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-6-get-only-a-count-of-users"></a><span data-ttu-id="9ed55-201">示例 6：仅获取用户数量</span><span class="sxs-lookup"><span data-stu-id="9ed55-201">Example 6: Get only a count of users</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-202">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-202">Request</span></span>

<span data-ttu-id="9ed55-203">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9ed55-204">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-204">Response</span></span>

<span data-ttu-id="9ed55-205">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-205">The following is an example of the response.</span></span>

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

### <a name="example-7-use-filter-and-top-to-get-one-user-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9ed55-206">示例 7：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。</span><span class="sxs-lookup"><span data-stu-id="9ed55-206">Example 7: Use $filter and $top to get one user with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-207">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-207">Request</span></span>

<span data-ttu-id="9ed55-208">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-208">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=startswith(displayName,'a')&$orderby=displayName&$count=true&$top=1
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9ed55-209">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-209">Response</span></span>

<span data-ttu-id="9ed55-210">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-210">The following is an example of the response.</span></span>
><span data-ttu-id="9ed55-211">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-211">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-8-use-filter-to-get-all-users-with-a-mail-that-ends-with-acontosocom-including-a-count-of-returned-objects-with-the-results-ordered-by-userprincipalname"></a><span data-ttu-id="9ed55-212">示例 8：使用 $filter 获取以 'a@contoso.com' 结尾的邮件的所有用户（包括返回对象的计数），结果按 userPrincipalName 排序</span><span class="sxs-lookup"><span data-stu-id="9ed55-212">Example 8: Use $filter to get all users with a mail that ends with 'a@contoso.com', including a count of returned objects, with the results ordered by userPrincipalName</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-213">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-213">Request</span></span>

<span data-ttu-id="9ed55-214">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-214">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ed55-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed55-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count_endsWith"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=endswith(mail,'a@contoso.com')&$orderby=userPrincipalName&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="9ed55-216">C#</span><span class="sxs-lookup"><span data-stu-id="9ed55-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-endswith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed55-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed55-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-endswith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed55-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed55-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-endswith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed55-219">Java</span><span class="sxs-lookup"><span data-stu-id="9ed55-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-endswith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ed55-220">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-220">Response</span></span>

<span data-ttu-id="9ed55-221">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-221">The following is an example of the response.</span></span>

><span data-ttu-id="9ed55-222">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-222">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-9-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-including-a-count-of-returned-objects"></a><span data-ttu-id="9ed55-223">示例 9：使用 $search 获取显示名称中包含字母“wa”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="9ed55-223">Example 9: Use $search to get users with display names that contain the letters 'wa' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-224">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-224">Request</span></span>

<span data-ttu-id="9ed55-225">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-225">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_wa_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9ed55-226">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-226">Response</span></span>

<span data-ttu-id="9ed55-227">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-227">The following is an example of the response.</span></span>
><span data-ttu-id="9ed55-228">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-228">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-10-use-search-to-get-users-with-display-names-that-contain-the-letters-wa-or-the-letters-to-including-a-count-of-returned-objects"></a><span data-ttu-id="9ed55-229">示例 10：使用 $search 获取显示名称中包含字母“wa”或“to”（包括返回的对象数）的用户。</span><span class="sxs-lookup"><span data-stu-id="9ed55-229">Example 10: Use $search to get users with display names that contain the letters 'wa' or the letters 'to' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-230">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-230">Request</span></span>

<span data-ttu-id="9ed55-231">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-231">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_to_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$search="displayName:wa" OR "displayName:to"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9ed55-232">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-232">Response</span></span>

<span data-ttu-id="9ed55-233">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-233">The following is an example of the response.</span></span> 
> <span data-ttu-id="9ed55-234">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ed55-234">**Note:** The response object shown here might be shortened for readability.</span></span>

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


### <a name="example-11-use-filter-to-get-users-who-are-assigned-a-specific-license"></a><span data-ttu-id="9ed55-235">示例 11：使用 $filter为用户分配特定许可证</span><span class="sxs-lookup"><span data-stu-id="9ed55-235">Example 11: Use $filter to get users who are assigned a specific license</span></span>

#### <a name="request"></a><span data-ttu-id="9ed55-236">请求</span><span class="sxs-lookup"><span data-stu-id="9ed55-236">Request</span></span>

<span data-ttu-id="9ed55-237">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed55-237">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_user_assignedLicenses"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,mail,assignedLicenses&$filter=assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)
```

#### <a name="response"></a><span data-ttu-id="9ed55-238">响应</span><span class="sxs-lookup"><span data-stu-id="9ed55-238">Response</span></span>

<span data-ttu-id="9ed55-239">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed55-239">The following is an example of the response.</span></span>

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
