# <a name="checkmembergroups"></a><span data-ttu-id="45b26-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="45b26-101">checkMemberGroups</span></span>
<span data-ttu-id="45b26-p101">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="45b26-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="45b26-p102">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="45b26-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="45b26-108">权限</span><span class="sxs-lookup"><span data-stu-id="45b26-108">Permissions</span></span>
<span data-ttu-id="45b26-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="45b26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45b26-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="45b26-111">Permission type</span></span>      | <span data-ttu-id="45b26-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45b26-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="45b26-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45b26-113">Delegated (work or school account)</span></span> | <span data-ttu-id="45b26-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45b26-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="45b26-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45b26-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45b26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45b26-116">Not supported.</span></span>    | 
|<span data-ttu-id="45b26-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="45b26-117">Application</span></span> | <span data-ttu-id="45b26-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b26-118">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="45b26-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45b26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="45b26-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="45b26-120">Request headers</span></span>
| <span data-ttu-id="45b26-121">标头</span><span class="sxs-lookup"><span data-stu-id="45b26-121">Header</span></span>       | <span data-ttu-id="45b26-122">值</span><span class="sxs-lookup"><span data-stu-id="45b26-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45b26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45b26-123">Authorization</span></span>  | <span data-ttu-id="45b26-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45b26-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="45b26-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45b26-126">Content-Type</span></span>  | <span data-ttu-id="45b26-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45b26-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45b26-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="45b26-128">Request body</span></span>
<span data-ttu-id="45b26-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="45b26-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="45b26-130">参数</span><span class="sxs-lookup"><span data-stu-id="45b26-130">Parameter</span></span>    | <span data-ttu-id="45b26-131">类型</span><span class="sxs-lookup"><span data-stu-id="45b26-131">Type</span></span>   |<span data-ttu-id="45b26-132">说明</span><span class="sxs-lookup"><span data-stu-id="45b26-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45b26-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="45b26-133">groupIds</span></span>|<span data-ttu-id="45b26-134">String</span><span class="sxs-lookup"><span data-stu-id="45b26-134">String</span></span>|<span data-ttu-id="45b26-135">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="45b26-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="45b26-136">响应</span><span class="sxs-lookup"><span data-stu-id="45b26-136">Response</span></span>

<span data-ttu-id="45b26-137">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="45b26-137">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45b26-138">示例</span><span class="sxs-lookup"><span data-stu-id="45b26-138">Example</span></span>
<span data-ttu-id="45b26-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="45b26-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45b26-140">请求</span><span class="sxs-lookup"><span data-stu-id="45b26-140">Request</span></span>
<span data-ttu-id="45b26-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45b26-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="45b26-142">响应</span><span class="sxs-lookup"><span data-stu-id="45b26-142">Response</span></span>
<span data-ttu-id="45b26-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45b26-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
