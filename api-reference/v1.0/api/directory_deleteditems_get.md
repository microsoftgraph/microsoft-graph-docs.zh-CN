# <a name="get-deleted-item"></a><span data-ttu-id="bb112-101">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="bb112-101">Get deleted item</span></span>

<span data-ttu-id="bb112-102">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="bb112-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="bb112-103">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="bb112-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb112-104">权限</span><span class="sxs-lookup"><span data-stu-id="bb112-104">Permissions</span></span>
<span data-ttu-id="bb112-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bb112-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="bb112-107">对于用户：</span><span class="sxs-lookup"><span data-stu-id="bb112-107">For users:</span></span>

|<span data-ttu-id="bb112-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb112-108">Permission type</span></span>      | <span data-ttu-id="bb112-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb112-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb112-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb112-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb112-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb112-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="bb112-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb112-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb112-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb112-113">Not supported.</span></span> |
|<span data-ttu-id="bb112-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb112-114">Application</span></span> | <span data-ttu-id="bb112-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb112-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="bb112-116">对于组：</span><span class="sxs-lookup"><span data-stu-id="bb112-116">For groups:</span></span>

|<span data-ttu-id="bb112-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb112-117">Permission type</span></span>      | <span data-ttu-id="bb112-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb112-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb112-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb112-119">Delegated (work or school account)</span></span> | <span data-ttu-id="bb112-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb112-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bb112-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb112-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb112-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb112-122">Not supported.</span></span>    |
|<span data-ttu-id="bb112-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb112-123">Application</span></span> | <span data-ttu-id="bb112-124">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb112-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb112-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb112-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb112-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb112-126">Optional query parameters</span></span>
<span data-ttu-id="bb112-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb112-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb112-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb112-128">Request headers</span></span>
| <span data-ttu-id="bb112-129">名称</span><span class="sxs-lookup"><span data-stu-id="bb112-129">Name</span></span>      |<span data-ttu-id="bb112-130">说明</span><span class="sxs-lookup"><span data-stu-id="bb112-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb112-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb112-131">Authorization</span></span>  | <span data-ttu-id="bb112-132">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="bb112-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="bb112-133">Accept</span><span class="sxs-lookup"><span data-stu-id="bb112-133">Accept</span></span>  | <span data-ttu-id="bb112-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bb112-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb112-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb112-135">Request body</span></span>
<span data-ttu-id="bb112-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb112-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb112-137">响应</span><span class="sxs-lookup"><span data-stu-id="bb112-137">Response</span></span>

<span data-ttu-id="bb112-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb112-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb112-139">示例</span><span class="sxs-lookup"><span data-stu-id="bb112-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb112-140">请求</span><span class="sxs-lookup"><span data-stu-id="bb112-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="bb112-141">响应</span><span class="sxs-lookup"><span data-stu-id="bb112-141">Response</span></span>
<span data-ttu-id="bb112-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb112-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->