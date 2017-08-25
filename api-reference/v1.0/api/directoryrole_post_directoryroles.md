# <a name="activate-directoryrole"></a><span data-ttu-id="317ea-101">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="317ea-101">Activate directoryRole</span></span>

<span data-ttu-id="317ea-p101">激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="317ea-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="317ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="317ea-106">Permissions</span></span>
<span data-ttu-id="317ea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="317ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="317ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="317ea-109">Permission type</span></span>      | <span data-ttu-id="317ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="317ea-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="317ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="317ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="317ea-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="317ea-112">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="317ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="317ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="317ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="317ea-114">Not supported.</span></span>    | 
|<span data-ttu-id="317ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="317ea-115">Application</span></span> | <span data-ttu-id="317ea-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="317ea-116">Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="317ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="317ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="317ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="317ea-118">Request headers</span></span>
| <span data-ttu-id="317ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="317ea-119">Name</span></span>       | <span data-ttu-id="317ea-120">类型</span><span class="sxs-lookup"><span data-stu-id="317ea-120">Type</span></span> | <span data-ttu-id="317ea-121">说明</span><span class="sxs-lookup"><span data-stu-id="317ea-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="317ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="317ea-122">Authorization</span></span>  | <span data-ttu-id="317ea-123">string</span><span class="sxs-lookup"><span data-stu-id="317ea-123">string</span></span>  | <span data-ttu-id="317ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="317ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="317ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="317ea-126">Content-Type</span></span>  | <span data-ttu-id="317ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="317ea-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="317ea-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="317ea-128">Request body</span></span>
<span data-ttu-id="317ea-129">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="317ea-129">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="317ea-130">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="317ea-130">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="317ea-131">必需的参数</span><span class="sxs-lookup"><span data-stu-id="317ea-131">Required parameter</span></span> | <span data-ttu-id="317ea-132">类型</span><span class="sxs-lookup"><span data-stu-id="317ea-132">Type</span></span> | <span data-ttu-id="317ea-133">说明</span><span class="sxs-lookup"><span data-stu-id="317ea-133">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="317ea-134">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="317ea-134">roleTemplateId</span></span> | <span data-ttu-id="317ea-135">string</span><span class="sxs-lookup"><span data-stu-id="317ea-135">string</span></span> | <span data-ttu-id="317ea-p104">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="317ea-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="317ea-138">响应</span><span class="sxs-lookup"><span data-stu-id="317ea-138">Response</span></span>

<span data-ttu-id="317ea-139">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="317ea-139">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="317ea-140">示例</span><span class="sxs-lookup"><span data-stu-id="317ea-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="317ea-141">请求</span><span class="sxs-lookup"><span data-stu-id="317ea-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="317ea-142">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="317ea-142">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="317ea-143">响应</span><span class="sxs-lookup"><span data-stu-id="317ea-143">Response</span></span>
<span data-ttu-id="317ea-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="317ea-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
