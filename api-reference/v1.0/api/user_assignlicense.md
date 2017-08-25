# <a name="assignlicense"></a><span data-ttu-id="7aebe-101">assignLicense</span><span class="sxs-lookup"><span data-stu-id="7aebe-101">assignLicense</span></span>
<span data-ttu-id="7aebe-p101">为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="7aebe-p101">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aebe-104">权限</span><span class="sxs-lookup"><span data-stu-id="7aebe-104">Permissions</span></span>
<span data-ttu-id="7aebe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7aebe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7aebe-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aebe-107">Permission type</span></span>      | <span data-ttu-id="7aebe-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aebe-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="7aebe-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aebe-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7aebe-110">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aebe-110">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    | 
|<span data-ttu-id="7aebe-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aebe-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aebe-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aebe-112">Not supported.</span></span>    | 
|<span data-ttu-id="7aebe-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aebe-113">Application</span></span> | <span data-ttu-id="7aebe-114">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aebe-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7aebe-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aebe-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="7aebe-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aebe-116">Request headers</span></span>
| <span data-ttu-id="7aebe-117">标头</span><span class="sxs-lookup"><span data-stu-id="7aebe-117">Header</span></span>       | <span data-ttu-id="7aebe-118">值</span><span class="sxs-lookup"><span data-stu-id="7aebe-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7aebe-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aebe-119">Authorization</span></span>  | <span data-ttu-id="7aebe-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aebe-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7aebe-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aebe-122">Content-Type</span></span>  | <span data-ttu-id="7aebe-123">application/json</span><span class="sxs-lookup"><span data-stu-id="7aebe-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aebe-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aebe-124">Request body</span></span>
<span data-ttu-id="7aebe-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7aebe-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aebe-126">参数</span><span class="sxs-lookup"><span data-stu-id="7aebe-126">Parameter</span></span>    | <span data-ttu-id="7aebe-127">类型</span><span class="sxs-lookup"><span data-stu-id="7aebe-127">Type</span></span>   |<span data-ttu-id="7aebe-128">说明</span><span class="sxs-lookup"><span data-stu-id="7aebe-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aebe-129">addLicenses</span><span class="sxs-lookup"><span data-stu-id="7aebe-129">addLicenses</span></span>|<span data-ttu-id="7aebe-130">AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="7aebe-130">AssignedLicense</span></span>|<span data-ttu-id="7aebe-p104">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。可以通过设置 [assignedLicense](../resources/assignedlicense.md) 对象中的 **disabledPlans** 属性禁用与许可证相关的计划。</span><span class="sxs-lookup"><span data-stu-id="7aebe-p104">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="7aebe-133">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="7aebe-133">removeLicenses</span></span>|<span data-ttu-id="7aebe-134">Guid</span><span class="sxs-lookup"><span data-stu-id="7aebe-134">Guid</span></span>|<span data-ttu-id="7aebe-135">标识要删除的许可证的 GUID 的集合。</span><span class="sxs-lookup"><span data-stu-id="7aebe-135">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="7aebe-136">响应</span><span class="sxs-lookup"><span data-stu-id="7aebe-136">Response</span></span>

<span data-ttu-id="7aebe-137">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7aebe-137">If successful, this method returns `200, OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aebe-138">示例</span><span class="sxs-lookup"><span data-stu-id="7aebe-138">Example</span></span>
<span data-ttu-id="7aebe-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7aebe-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7aebe-140">请求</span><span class="sxs-lookup"><span data-stu-id="7aebe-140">Request</span></span>
<span data-ttu-id="7aebe-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7aebe-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="7aebe-142">响应</span><span class="sxs-lookup"><span data-stu-id="7aebe-142">Response</span></span>
<span data-ttu-id="7aebe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7aebe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
