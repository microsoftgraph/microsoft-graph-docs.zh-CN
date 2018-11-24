# <a name="delete-open-extension"></a><span data-ttu-id="b4f19-101">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="b4f19-101">Delete open extension</span></span>

<span data-ttu-id="b4f19-102">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/openTypeExtension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="b4f19-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b4f19-103">权限</span><span class="sxs-lookup"><span data-stu-id="b4f19-103">Permissions</span></span>

<span data-ttu-id="b4f19-104">根据您正在删除扩展名的资源和权限类型 （委派或应用程序） 请求下, 表中所指定的权限是最小特权需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b4f19-104">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b4f19-105">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b4f19-105">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b4f19-106">支持的资源</span><span class="sxs-lookup"><span data-stu-id="b4f19-106">Supported resource</span></span> | <span data-ttu-id="b4f19-107">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f19-107">Delegated (work or school account)</span></span> | <span data-ttu-id="b4f19-108">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4f19-108">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4f19-109">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4f19-109">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="b4f19-110">设备</span><span class="sxs-lookup"><span data-stu-id="b4f19-110">device</span></span>](../resources/device.md) | <span data-ttu-id="b4f19-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-111">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="b4f19-112">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-112">Not supported</span></span> | <span data-ttu-id="b4f19-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-113">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="b4f19-114">事件</span><span class="sxs-lookup"><span data-stu-id="b4f19-114">event</span></span>](../resources/event.md) | <span data-ttu-id="b4f19-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="b4f19-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="b4f19-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-117">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="b4f19-118">组</span><span class="sxs-lookup"><span data-stu-id="b4f19-118">group</span></span>](../resources/group.md) | <span data-ttu-id="b4f19-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="b4f19-120">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-120">Not supported</span></span> | <span data-ttu-id="b4f19-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-121">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b4f19-122">组事件</span><span class="sxs-lookup"><span data-stu-id="b4f19-122">group event</span></span>](../resources/event.md) | <span data-ttu-id="b4f19-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="b4f19-124">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-124">Not supported</span></span> | <span data-ttu-id="b4f19-125">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-125">Not supported</span></span> |
| [<span data-ttu-id="b4f19-126">组帖子</span><span class="sxs-lookup"><span data-stu-id="b4f19-126">group post</span></span>](../resources/post.md) | <span data-ttu-id="b4f19-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="b4f19-128">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-128">Not supported</span></span> | <span data-ttu-id="b4f19-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-129">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b4f19-130">邮件</span><span class="sxs-lookup"><span data-stu-id="b4f19-130">message</span></span>](../resources/message.md) | <span data-ttu-id="b4f19-131">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-131">Mail.ReadWrite</span></span> | <span data-ttu-id="b4f19-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-132">Mail.ReadWrite</span></span> | <span data-ttu-id="b4f19-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-133">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="b4f19-134">组织</span><span class="sxs-lookup"><span data-stu-id="b4f19-134">organization</span></span>](../resources/organization.md) | <span data-ttu-id="b4f19-135">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-135">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="b4f19-136">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-136">Not supported</span></span> | <span data-ttu-id="b4f19-137">不支持</span><span class="sxs-lookup"><span data-stu-id="b4f19-137">Not supported</span></span> |
| [<span data-ttu-id="b4f19-138">个人联系人</span><span class="sxs-lookup"><span data-stu-id="b4f19-138">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="b4f19-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-139">Contacts.ReadWrite</span></span> | <span data-ttu-id="b4f19-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="b4f19-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-141">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="b4f19-142">用户</span><span class="sxs-lookup"><span data-stu-id="b4f19-142">user</span></span>](../resources/user.md) | <span data-ttu-id="b4f19-143">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-143">User.ReadWrite.All</span></span> | <span data-ttu-id="b4f19-144">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4f19-144">User.ReadWrite</span></span> | <span data-ttu-id="b4f19-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f19-145">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4f19-146">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4f19-146">HTTP request</span></span>
<span data-ttu-id="b4f19-147">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="b4f19-147">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="b4f19-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="b4f19-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="b4f19-150">路径参数</span><span class="sxs-lookup"><span data-stu-id="b4f19-150">Path parameters</span></span>
|<span data-ttu-id="b4f19-151">参数</span><span class="sxs-lookup"><span data-stu-id="b4f19-151">Parameter</span></span>|<span data-ttu-id="b4f19-152">类型</span><span class="sxs-lookup"><span data-stu-id="b4f19-152">Type</span></span>|<span data-ttu-id="b4f19-153">说明</span><span class="sxs-lookup"><span data-stu-id="b4f19-153">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b4f19-154">ID</span><span class="sxs-lookup"><span data-stu-id="b4f19-154">id</span></span>|<span data-ttu-id="b4f19-155">string</span><span class="sxs-lookup"><span data-stu-id="b4f19-155">string</span></span>|<span data-ttu-id="b4f19-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="b4f19-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="b4f19-158">extensionId</span><span class="sxs-lookup"><span data-stu-id="b4f19-158">extensionId</span></span>|<span data-ttu-id="b4f19-159">string</span><span class="sxs-lookup"><span data-stu-id="b4f19-159">string</span></span>|<span data-ttu-id="b4f19-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="b4f19-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b4f19-163">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4f19-163">Request headers</span></span>
| <span data-ttu-id="b4f19-164">名称</span><span class="sxs-lookup"><span data-stu-id="b4f19-164">Name</span></span>       | <span data-ttu-id="b4f19-165">值</span><span class="sxs-lookup"><span data-stu-id="b4f19-165">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b4f19-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4f19-166">Authorization</span></span> | <span data-ttu-id="b4f19-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4f19-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4f19-169">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4f19-169">Request body</span></span>
<span data-ttu-id="b4f19-170">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4f19-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4f19-171">响应</span><span class="sxs-lookup"><span data-stu-id="b4f19-171">Response</span></span>

<span data-ttu-id="b4f19-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4f19-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4f19-174">示例</span><span class="sxs-lookup"><span data-stu-id="b4f19-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4f19-175">请求</span><span class="sxs-lookup"><span data-stu-id="b4f19-175">Request</span></span>
<span data-ttu-id="b4f19-176">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="b4f19-176">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="b4f19-177">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="b4f19-177">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="b4f19-178">响应</span><span class="sxs-lookup"><span data-stu-id="b4f19-178">Response</span></span>
<span data-ttu-id="b4f19-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4f19-179">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->