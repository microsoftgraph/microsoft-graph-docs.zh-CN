# <a name="update-permission"></a><span data-ttu-id="47162-101">更新权限</span><span class="sxs-lookup"><span data-stu-id="47162-101">Update permission</span></span>

<span data-ttu-id="47162-102">通过修补该资源更新权限的属性。</span><span class="sxs-lookup"><span data-stu-id="47162-102">Update the properties of a permission by patching the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="47162-103">权限</span><span class="sxs-lookup"><span data-stu-id="47162-103">Permissions</span></span>

<span data-ttu-id="47162-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="47162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47162-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="47162-106">Permission type</span></span>      | <span data-ttu-id="47162-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47162-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="47162-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47162-108">Delegated (work or school account)</span></span> | <span data-ttu-id="47162-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47162-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="47162-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47162-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47162-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47162-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="47162-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="47162-112">Application</span></span> | <span data-ttu-id="47162-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47162-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47162-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47162-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/root:/{path}:/permissions/{perm-id}
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="47162-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="47162-115">Request headers</span></span>

| <span data-ttu-id="47162-116">名称</span><span class="sxs-lookup"><span data-stu-id="47162-116">Name</span></span>          | <span data-ttu-id="47162-117">类型</span><span class="sxs-lookup"><span data-stu-id="47162-117">Type</span></span>   | <span data-ttu-id="47162-118">说明</span><span class="sxs-lookup"><span data-stu-id="47162-118">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="47162-119">if-match</span><span class="sxs-lookup"><span data-stu-id="47162-119">if-match</span></span>      | <span data-ttu-id="47162-120">string</span><span class="sxs-lookup"><span data-stu-id="47162-120">string</span></span> | <span data-ttu-id="47162-121">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="47162-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="request-body"></a><span data-ttu-id="47162-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="47162-122">Request body</span></span>
<span data-ttu-id="47162-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="47162-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="47162-126">属性</span><span class="sxs-lookup"><span data-stu-id="47162-126">Property</span></span>     | <span data-ttu-id="47162-127">类型</span><span class="sxs-lookup"><span data-stu-id="47162-127">Type</span></span>   | <span data-ttu-id="47162-128">说明</span><span class="sxs-lookup"><span data-stu-id="47162-128">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="47162-129">**角色**</span><span class="sxs-lookup"><span data-stu-id="47162-129">**roles**</span></span>    | <span data-ttu-id="47162-130">String</span><span class="sxs-lookup"><span data-stu-id="47162-130">String</span></span> | <span data-ttu-id="47162-131">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="47162-131">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="47162-132">响应</span><span class="sxs-lookup"><span data-stu-id="47162-132">Response</span></span>

<span data-ttu-id="47162-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47162-133">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47162-134">示例</span><span class="sxs-lookup"><span data-stu-id="47162-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="47162-135">请求</span><span class="sxs-lookup"><span data-stu-id="47162-135">Request</span></span>

<span data-ttu-id="47162-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47162-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="47162-137">响应</span><span class="sxs-lookup"><span data-stu-id="47162-137">Response</span></span>

<span data-ttu-id="47162-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="47162-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
