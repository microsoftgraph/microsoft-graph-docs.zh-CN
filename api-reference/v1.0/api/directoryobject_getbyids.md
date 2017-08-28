# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="2bb07-101">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="2bb07-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="2bb07-p101">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="2bb07-105">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="2bb07-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="2bb07-106">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject_getmemberobjects.md) 或 [getMemberGroups](directoryobject_getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="2bb07-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="2bb07-107">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="2bb07-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bb07-108">权限</span><span class="sxs-lookup"><span data-stu-id="2bb07-108">Permissions</span></span>

<span data-ttu-id="2bb07-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2bb07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bb07-111">Permission type</span></span>      | <span data-ttu-id="2bb07-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bb07-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bb07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb07-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2bb07-114">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bb07-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bb07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb07-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bb07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bb07-116">Not supported.</span></span>    |
|<span data-ttu-id="2bb07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bb07-117">Application</span></span> | <span data-ttu-id="2bb07-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bb07-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bb07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bb07-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="2bb07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bb07-120">Request headers</span></span>

| <span data-ttu-id="2bb07-121">名称</span><span class="sxs-lookup"><span data-stu-id="2bb07-121">Name</span></span>       | <span data-ttu-id="2bb07-122">类型</span><span class="sxs-lookup"><span data-stu-id="2bb07-122">Type</span></span> | <span data-ttu-id="2bb07-123">说明</span><span class="sxs-lookup"><span data-stu-id="2bb07-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2bb07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb07-124">Authorization</span></span>  | <span data-ttu-id="2bb07-125">string</span><span class="sxs-lookup"><span data-stu-id="2bb07-125">string</span></span>  | <span data-ttu-id="2bb07-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2bb07-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2bb07-128">Content-Type</span></span>  | <span data-ttu-id="2bb07-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2bb07-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bb07-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bb07-130">Request body</span></span>

<span data-ttu-id="2bb07-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2bb07-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2bb07-132">参数</span><span class="sxs-lookup"><span data-stu-id="2bb07-132">Parameter</span></span>   | <span data-ttu-id="2bb07-133">类型</span><span class="sxs-lookup"><span data-stu-id="2bb07-133">Type</span></span> |<span data-ttu-id="2bb07-134">说明</span><span class="sxs-lookup"><span data-stu-id="2bb07-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bb07-135">ids</span><span class="sxs-lookup"><span data-stu-id="2bb07-135">ids</span></span>|<span data-ttu-id="2bb07-136">String collection</span><span class="sxs-lookup"><span data-stu-id="2bb07-136">String collection</span></span>| <span data-ttu-id="2bb07-p104">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="2bb07-139">types</span><span class="sxs-lookup"><span data-stu-id="2bb07-139">types</span></span>|<span data-ttu-id="2bb07-140">String collection</span><span class="sxs-lookup"><span data-stu-id="2bb07-140">String collection</span></span>| <span data-ttu-id="2bb07-p105">指定要搜索的资源集合集的资源类型集合。如果未指定，则默认为 [directoryObject](../resources/directoryobject.md)，其包含目录中定义的所有资源类型。可以在该集合中指定派生自 `directoryObject` 的所有对象，例如：[用户](../resources/user.md)、[组](../resources/group.md)、[设备](../resources/device.md)等。这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p105">A collection of resource types that specifies the set of resource collections to search. If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory. Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on. The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="2bb07-145">响应</span><span class="sxs-lookup"><span data-stu-id="2bb07-145">Response</span></span>

<span data-ttu-id="2bb07-146">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2bb07-146">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb07-147">示例</span><span class="sxs-lookup"><span data-stu-id="2bb07-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2bb07-148">请求</span><span class="sxs-lookup"><span data-stu-id="2bb07-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="2bb07-149">响应</span><span class="sxs-lookup"><span data-stu-id="2bb07-149">Response</span></span>

<span data-ttu-id="2bb07-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bb07-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
