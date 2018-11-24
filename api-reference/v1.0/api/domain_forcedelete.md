# <a name="force-domain-deletion"></a><span data-ttu-id="626d6-101">强制域删除</span><span class="sxs-lookup"><span data-stu-id="626d6-101">Force domain deletion</span></span>

<span data-ttu-id="626d6-102">删除使用长时间运行的异步操作的域。</span><span class="sxs-lookup"><span data-stu-id="626d6-102">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="626d6-103">此操作的一部分执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="626d6-103">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="626d6-104">更新`userPrincipalName`， `mail`，和`proxyAddresses`属性`users`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="626d6-104">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="626d6-105">更新`mail`属性`groups`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="626d6-105">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="626d6-106">更新`identifierUris`属性`applications`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="626d6-106">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="626d6-107">如果要重命名的对象的数量大于 1000年，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="626d6-107">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="626d6-108">如果的`applications`要重命名为多租户应用程序，则返回一个错误。</span><span class="sxs-lookup"><span data-stu-id="626d6-108">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="626d6-109">域删除完成后，已删除的域的 API 操作将返回 HTTP 404 状态代码。</span><span class="sxs-lookup"><span data-stu-id="626d6-109">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="626d6-110">若要验证删除的域，可以执行[get 域](domain_get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="626d6-110">To verify deletion of a domain, you can perform a [get domain](domain_get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="626d6-111">权限</span><span class="sxs-lookup"><span data-stu-id="626d6-111">Permissions</span></span>

<span data-ttu-id="626d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="626d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="626d6-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="626d6-114">Permission type</span></span>      | <span data-ttu-id="626d6-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="626d6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="626d6-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="626d6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="626d6-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="626d6-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="626d6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="626d6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="626d6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="626d6-119">Not supported.</span></span>    |
|<span data-ttu-id="626d6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="626d6-120">Application</span></span> | <span data-ttu-id="626d6-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626d6-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="626d6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="626d6-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="626d6-123">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="626d6-123">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="626d6-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="626d6-124">Request headers</span></span>

| <span data-ttu-id="626d6-125">名称</span><span class="sxs-lookup"><span data-stu-id="626d6-125">Name</span></span> | <span data-ttu-id="626d6-126">说明</span><span class="sxs-lookup"><span data-stu-id="626d6-126">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="626d6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="626d6-127">Authorization</span></span>  | <span data-ttu-id="626d6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="626d6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="626d6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="626d6-130">Content-Type</span></span>  | <span data-ttu-id="626d6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="626d6-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="626d6-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="626d6-132">Request body</span></span>

<span data-ttu-id="626d6-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="626d6-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="626d6-134">参数</span><span class="sxs-lookup"><span data-stu-id="626d6-134">Parameter</span></span> | <span data-ttu-id="626d6-135">类型</span><span class="sxs-lookup"><span data-stu-id="626d6-135">Type</span></span> | <span data-ttu-id="626d6-136">说明</span><span class="sxs-lookup"><span data-stu-id="626d6-136">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="626d6-137">若要禁用其重命名用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="626d6-137">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="626d6-138">如果禁用的用户帐户，则用户将不允许登录。</span><span class="sxs-lookup"><span data-stu-id="626d6-138">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="626d6-139">如果设置为**true** `users`更新为属于此操作将被禁用。</span><span class="sxs-lookup"><span data-stu-id="626d6-139">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="626d6-140">默认值为**true**。</span><span class="sxs-lookup"><span data-stu-id="626d6-140">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="626d6-141">响应正文</span><span class="sxs-lookup"><span data-stu-id="626d6-141">Response body</span></span>

<span data-ttu-id="626d6-142">如果成功，此方法返回`HTTP/1.1 204 OK`状态代码。</span><span class="sxs-lookup"><span data-stu-id="626d6-142">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="626d6-143">示例</span><span class="sxs-lookup"><span data-stu-id="626d6-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="626d6-144">请求</span><span class="sxs-lookup"><span data-stu-id="626d6-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="626d6-145">响应</span><span class="sxs-lookup"><span data-stu-id="626d6-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->