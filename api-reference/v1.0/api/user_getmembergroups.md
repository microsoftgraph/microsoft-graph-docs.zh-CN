# <a name="user-getmembergroups"></a><span data-ttu-id="7b4eb-101">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7b4eb-101">user: getMemberGroups</span></span>
<span data-ttu-id="7b4eb-p101">返回用户是其成员的所有组。检查是可传递的，这和读取 [memberOf](../api/user_list_memberof.md) 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p101">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user_list_memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="7b4eb-p102">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b4eb-108">权限</span><span class="sxs-lookup"><span data-stu-id="7b4eb-108">Permissions</span></span>
<span data-ttu-id="7b4eb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="7b4eb-111">**注意：**此 API 当前需要 Directory.Read.All 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="7b4eb-112">将 User.Read 或 User.ReadBasic.All 权限与 Group.Read.All 权限结合使用将返回错误。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-112">Using the User.Read or User.ReadBasic.All permissions in combination with the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="7b4eb-113">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-113">This is a known bug.</span></span>

|<span data-ttu-id="7b4eb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b4eb-114">Permission type</span></span>      | <span data-ttu-id="7b4eb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b4eb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b4eb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4eb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7b4eb-117">*User.Read 和 Group.Read.All*、*User.ReadBasic.All 和 Group.Read.All*、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b4eb-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b4eb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b4eb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b4eb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-119">Not supported.</span></span>    |
|<span data-ttu-id="7b4eb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b4eb-120">Application</span></span> | <span data-ttu-id="7b4eb-121">*Group.Read.All*、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4eb-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b4eb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b4eb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="7b4eb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b4eb-123">Request headers</span></span>
| <span data-ttu-id="7b4eb-124">标头</span><span class="sxs-lookup"><span data-stu-id="7b4eb-124">Header</span></span>       | <span data-ttu-id="7b4eb-125">值</span><span class="sxs-lookup"><span data-stu-id="7b4eb-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b4eb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b4eb-126">Authorization</span></span>  | <span data-ttu-id="7b4eb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b4eb-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b4eb-129">Content-Type</span></span>  | <span data-ttu-id="7b4eb-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7b4eb-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b4eb-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b4eb-131">Request body</span></span>
<span data-ttu-id="7b4eb-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b4eb-133">参数</span><span class="sxs-lookup"><span data-stu-id="7b4eb-133">Parameter</span></span>    | <span data-ttu-id="7b4eb-134">类型</span><span class="sxs-lookup"><span data-stu-id="7b4eb-134">Type</span></span>   |<span data-ttu-id="7b4eb-135">说明</span><span class="sxs-lookup"><span data-stu-id="7b4eb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b4eb-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7b4eb-136">securityEnabledOnly</span></span>|<span data-ttu-id="7b4eb-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b4eb-137">Boolean</span></span>|<span data-ttu-id="7b4eb-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="7b4eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="7b4eb-140">Response</span></span>

<span data-ttu-id="7b4eb-141">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="7b4eb-142">示例</span><span class="sxs-lookup"><span data-stu-id="7b4eb-142">Example</span></span>
<span data-ttu-id="7b4eb-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b4eb-144">请求</span><span class="sxs-lookup"><span data-stu-id="7b4eb-144">Request</span></span>
<span data-ttu-id="7b4eb-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="7b4eb-146">响应</span><span class="sxs-lookup"><span data-stu-id="7b4eb-146">Response</span></span>
<span data-ttu-id="7b4eb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b4eb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
