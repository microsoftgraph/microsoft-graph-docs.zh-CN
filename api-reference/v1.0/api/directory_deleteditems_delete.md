# <a name="permanently-delete-item"></a><span data-ttu-id="fc610-101">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="fc610-101">Permanently delete item</span></span>

<span data-ttu-id="fc610-102">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="fc610-102">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="fc610-103">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="fc610-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="fc610-104">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="fc610-104">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="fc610-105">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="fc610-105">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc610-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc610-106">Permissions</span></span>
<span data-ttu-id="fc610-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fc610-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="fc610-109">对于用户：</span><span class="sxs-lookup"><span data-stu-id="fc610-109">For users:</span></span>

|<span data-ttu-id="fc610-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc610-110">Permission type</span></span>      | <span data-ttu-id="fc610-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc610-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc610-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc610-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc610-113">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc610-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fc610-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc610-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc610-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc610-115">Not supported.</span></span> |
|<span data-ttu-id="fc610-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc610-116">Application</span></span> | <span data-ttu-id="fc610-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc610-117">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="fc610-118">对于组：</span><span class="sxs-lookup"><span data-stu-id="fc610-118">For groups:</span></span>

|<span data-ttu-id="fc610-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc610-119">Permission type</span></span>      | <span data-ttu-id="fc610-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc610-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc610-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc610-121">Delegated (work or school account)</span></span> | <span data-ttu-id="fc610-122">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc610-122">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fc610-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc610-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc610-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc610-124">Not supported.</span></span>    |
|<span data-ttu-id="fc610-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc610-125">Application</span></span> | <span data-ttu-id="fc610-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc610-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc610-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc610-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc610-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc610-128">Request headers</span></span>
| <span data-ttu-id="fc610-129">名称</span><span class="sxs-lookup"><span data-stu-id="fc610-129">Name</span></span>       | <span data-ttu-id="fc610-130">说明</span><span class="sxs-lookup"><span data-stu-id="fc610-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc610-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc610-131">Authorization</span></span>  | <span data-ttu-id="fc610-132">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="fc610-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="fc610-133">Accept</span><span class="sxs-lookup"><span data-stu-id="fc610-133">Accept</span></span>  | <span data-ttu-id="fc610-134">application/json</span><span class="sxs-lookup"><span data-stu-id="fc610-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc610-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc610-135">Request body</span></span>
<span data-ttu-id="fc610-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc610-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc610-137">响应</span><span class="sxs-lookup"><span data-stu-id="fc610-137">Response</span></span>

<span data-ttu-id="fc610-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc610-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc610-140">示例</span><span class="sxs-lookup"><span data-stu-id="fc610-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc610-141">请求</span><span class="sxs-lookup"><span data-stu-id="fc610-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="fc610-142">响应</span><span class="sxs-lookup"><span data-stu-id="fc610-142">Response</span></span>
<span data-ttu-id="fc610-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc610-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->