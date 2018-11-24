# <a name="list-deleted-items"></a><span data-ttu-id="d367b-101">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="d367b-101">List deleted items</span></span>

<span data-ttu-id="d367b-102">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="d367b-102">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="d367b-103">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d367b-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="d367b-104">权限</span><span class="sxs-lookup"><span data-stu-id="d367b-104">Permissions</span></span>
<span data-ttu-id="d367b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d367b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="d367b-107">对于用户：</span><span class="sxs-lookup"><span data-stu-id="d367b-107">For users:</span></span>

|<span data-ttu-id="d367b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d367b-108">Permission type</span></span>      | <span data-ttu-id="d367b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d367b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d367b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d367b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d367b-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d367b-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d367b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d367b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d367b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d367b-113">Not supported.</span></span> |
|<span data-ttu-id="d367b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d367b-114">Application</span></span> | <span data-ttu-id="d367b-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d367b-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="d367b-116">对于组：</span><span class="sxs-lookup"><span data-stu-id="d367b-116">For groups:</span></span>

|<span data-ttu-id="d367b-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="d367b-117">Permission type</span></span>      | <span data-ttu-id="d367b-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d367b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d367b-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d367b-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d367b-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d367b-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d367b-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d367b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d367b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d367b-122">Not supported.</span></span>    |
|<span data-ttu-id="d367b-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="d367b-123">Application</span></span> | <span data-ttu-id="d367b-124">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d367b-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d367b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d367b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="d367b-126">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="d367b-126">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="d367b-127">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="d367b-127">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="d367b-128">不支持调用 GET/目录/deletedItems 没有类型。</span><span class="sxs-lookup"><span data-stu-id="d367b-128">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d367b-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d367b-129">Optional query parameters</span></span>
<span data-ttu-id="d367b-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d367b-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d367b-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="d367b-131">Request headers</span></span>
| <span data-ttu-id="d367b-132">名称</span><span class="sxs-lookup"><span data-stu-id="d367b-132">Name</span></span>      |<span data-ttu-id="d367b-133">说明</span><span class="sxs-lookup"><span data-stu-id="d367b-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d367b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d367b-134">Authorization</span></span>  | <span data-ttu-id="d367b-135">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="d367b-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="d367b-136">Accept</span><span class="sxs-lookup"><span data-stu-id="d367b-136">Accept</span></span>  | <span data-ttu-id="d367b-137">application/json</span><span class="sxs-lookup"><span data-stu-id="d367b-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d367b-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="d367b-138">Request body</span></span>
<span data-ttu-id="d367b-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d367b-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d367b-140">响应</span><span class="sxs-lookup"><span data-stu-id="d367b-140">Response</span></span>

<span data-ttu-id="d367b-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d367b-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d367b-142">示例</span><span class="sxs-lookup"><span data-stu-id="d367b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d367b-143">请求</span><span class="sxs-lookup"><span data-stu-id="d367b-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="d367b-144">响应</span><span class="sxs-lookup"><span data-stu-id="d367b-144">Response</span></span>
<span data-ttu-id="d367b-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d367b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->