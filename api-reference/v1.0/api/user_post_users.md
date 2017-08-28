# <a name="create-user"></a><span data-ttu-id="314ea-101">创建用户</span><span class="sxs-lookup"><span data-stu-id="314ea-101">Create User</span></span>

<span data-ttu-id="314ea-p101">使用此 API 新建用户。请求正文包含要创建的用户。至少必须指定必需的用户属性。可以选择指定其他任意可写属性。</span><span class="sxs-lookup"><span data-stu-id="314ea-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="314ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="314ea-106">Permissions</span></span>
<span data-ttu-id="314ea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="314ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="314ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="314ea-109">Permission type</span></span>      | <span data-ttu-id="314ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="314ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="314ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="314ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="314ea-112">User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="314ea-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="314ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="314ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="314ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="314ea-114">Not supported.</span></span>    |
|<span data-ttu-id="314ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="314ea-115">Application</span></span> | <span data-ttu-id="314ea-116">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="314ea-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="314ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="314ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="314ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="314ea-118">Request headers</span></span>
| <span data-ttu-id="314ea-119">标头</span><span class="sxs-lookup"><span data-stu-id="314ea-119">Header</span></span>       | <span data-ttu-id="314ea-120">值</span><span class="sxs-lookup"><span data-stu-id="314ea-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="314ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="314ea-121">Authorization</span></span>  | <span data-ttu-id="314ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="314ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="314ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="314ea-124">Content-Type</span></span>  | <span data-ttu-id="314ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="314ea-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="314ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="314ea-126">Request body</span></span>
<span data-ttu-id="314ea-127">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="314ea-127">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="314ea-128">下表显示创建用户时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="314ea-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="314ea-129">参数</span><span class="sxs-lookup"><span data-stu-id="314ea-129">Parameter</span></span> | <span data-ttu-id="314ea-130">类型</span><span class="sxs-lookup"><span data-stu-id="314ea-130">Type</span></span> | <span data-ttu-id="314ea-131">说明</span><span class="sxs-lookup"><span data-stu-id="314ea-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="314ea-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="314ea-132">accountEnabled</span></span> |<span data-ttu-id="314ea-133">boolean</span><span class="sxs-lookup"><span data-stu-id="314ea-133">boolean</span></span> |<span data-ttu-id="314ea-134">启用此帐户时为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="314ea-134">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="314ea-135">displayName</span><span class="sxs-lookup"><span data-stu-id="314ea-135">displayName</span></span> |<span data-ttu-id="314ea-136">string</span><span class="sxs-lookup"><span data-stu-id="314ea-136">string</span></span> |<span data-ttu-id="314ea-137">要在用户的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="314ea-137">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="314ea-138">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="314ea-138">onPremisesImmutableId</span></span> |<span data-ttu-id="314ea-139">string</span><span class="sxs-lookup"><span data-stu-id="314ea-139">string</span></span> |<span data-ttu-id="314ea-140">如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。</span><span class="sxs-lookup"><span data-stu-id="314ea-140">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="314ea-141">mailNickname</span><span class="sxs-lookup"><span data-stu-id="314ea-141">mailNickname</span></span> |<span data-ttu-id="314ea-142">string</span><span class="sxs-lookup"><span data-stu-id="314ea-142">string</span></span> |<span data-ttu-id="314ea-143">用户的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="314ea-143">The mail alias for the user.</span></span>|
|<span data-ttu-id="314ea-144">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="314ea-144">passwordProfile</span></span>|[<span data-ttu-id="314ea-145">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="314ea-145">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="314ea-146">用户的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="314ea-146">The password profile for the user.</span></span>|
|<span data-ttu-id="314ea-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="314ea-147">userPrincipalName</span></span> |<span data-ttu-id="314ea-148">string</span><span class="sxs-lookup"><span data-stu-id="314ea-148">string</span></span> |<span data-ttu-id="314ea-149">用户主体名称 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="314ea-149">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="314ea-150">响应</span><span class="sxs-lookup"><span data-stu-id="314ea-150">Response</span></span>

<span data-ttu-id="314ea-151">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="314ea-151">If successful, this method returns `201, Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="314ea-152">示例</span><span class="sxs-lookup"><span data-stu-id="314ea-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="314ea-153">请求</span><span class="sxs-lookup"><span data-stu-id="314ea-153">Request</span></span>
<span data-ttu-id="314ea-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="314ea-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="314ea-155">在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="314ea-155">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="314ea-156">响应</span><span class="sxs-lookup"><span data-stu-id="314ea-156">Response</span></span>
<span data-ttu-id="314ea-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="314ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
