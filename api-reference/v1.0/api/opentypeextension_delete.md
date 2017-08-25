# <a name="delete-open-extension"></a><span data-ttu-id="3ad47-101">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="3ad47-101">Delete open extension</span></span>

<span data-ttu-id="3ad47-102">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/openTypeExtension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="3ad47-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3ad47-103">权限</span><span class="sxs-lookup"><span data-stu-id="3ad47-103">Permissions</span></span>

<span data-ttu-id="3ad47-p101">若要调用此 API，必须有以下权限之一，具体视要从中删除扩展的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p101">One of the following permissions is required to call this API, depending on the resource you're deleting the extension from. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ad47-106">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="3ad47-106">**Supported resource**</span></span>|<span data-ttu-id="3ad47-107">**权限**</span><span class="sxs-lookup"><span data-stu-id="3ad47-107">**Permission**</span></span>|<span data-ttu-id="3ad47-108">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="3ad47-108">**Supported resource**</span></span>|<span data-ttu-id="3ad47-109">**权限**</span><span class="sxs-lookup"><span data-stu-id="3ad47-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3ad47-110">设备</span><span class="sxs-lookup"><span data-stu-id="3ad47-110">device</span></span>](../resources/device.md) | <span data-ttu-id="3ad47-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="3ad47-112">事件</span><span class="sxs-lookup"><span data-stu-id="3ad47-112">event</span></span>](../resources/event.md) | <span data-ttu-id="3ad47-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ad47-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="3ad47-114">组</span><span class="sxs-lookup"><span data-stu-id="3ad47-114">group</span></span>](../resources/group.md) | <span data-ttu-id="3ad47-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="3ad47-116">组事件</span><span class="sxs-lookup"><span data-stu-id="3ad47-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="3ad47-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="3ad47-118">组帖子</span><span class="sxs-lookup"><span data-stu-id="3ad47-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="3ad47-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="3ad47-120">邮件</span><span class="sxs-lookup"><span data-stu-id="3ad47-120">message</span></span>](../resources/message.md) | <span data-ttu-id="3ad47-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ad47-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="3ad47-122">组织</span><span class="sxs-lookup"><span data-stu-id="3ad47-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="3ad47-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="3ad47-124">个人联系人</span><span class="sxs-lookup"><span data-stu-id="3ad47-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="3ad47-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ad47-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3ad47-126">用户</span><span class="sxs-lookup"><span data-stu-id="3ad47-126">user</span></span>](../resources/user.md) | <span data-ttu-id="3ad47-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ad47-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="3ad47-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ad47-128">HTTP request</span></span>
<span data-ttu-id="3ad47-129">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="3ad47-129">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="3ad47-p102">**注意：**以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="3ad47-132">参数</span><span class="sxs-lookup"><span data-stu-id="3ad47-132">Parameters</span></span>
|<span data-ttu-id="3ad47-133">**参数**</span><span class="sxs-lookup"><span data-stu-id="3ad47-133">**Parameter**</span></span>|<span data-ttu-id="3ad47-134">**类型**</span><span class="sxs-lookup"><span data-stu-id="3ad47-134">**Type**</span></span>|<span data-ttu-id="3ad47-135">**说明**</span><span class="sxs-lookup"><span data-stu-id="3ad47-135">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3ad47-136">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="3ad47-136">_URL parameters_</span></span>|
|<span data-ttu-id="3ad47-137">id</span><span class="sxs-lookup"><span data-stu-id="3ad47-137">id</span></span>|<span data-ttu-id="3ad47-138">string</span><span class="sxs-lookup"><span data-stu-id="3ad47-138">string</span></span>|<span data-ttu-id="3ad47-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="3ad47-141">extensionId</span><span class="sxs-lookup"><span data-stu-id="3ad47-141">extensionId</span></span>|<span data-ttu-id="3ad47-142">string</span><span class="sxs-lookup"><span data-stu-id="3ad47-142">string</span></span>|<span data-ttu-id="3ad47-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="3ad47-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ad47-146">Request headers</span></span>
| <span data-ttu-id="3ad47-147">名称</span><span class="sxs-lookup"><span data-stu-id="3ad47-147">Name</span></span>       | <span data-ttu-id="3ad47-148">值</span><span class="sxs-lookup"><span data-stu-id="3ad47-148">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3ad47-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ad47-149">Authorization</span></span> | <span data-ttu-id="3ad47-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p105">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3ad47-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ad47-152">Request body</span></span>
<span data-ttu-id="3ad47-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ad47-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ad47-154">响应</span><span class="sxs-lookup"><span data-stu-id="3ad47-154">Response</span></span>

<span data-ttu-id="3ad47-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ad47-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad47-157">示例</span><span class="sxs-lookup"><span data-stu-id="3ad47-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ad47-158">请求</span><span class="sxs-lookup"><span data-stu-id="3ad47-158">Request</span></span>
<span data-ttu-id="3ad47-159">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="3ad47-159">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="3ad47-160">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="3ad47-160">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="3ad47-161">响应</span><span class="sxs-lookup"><span data-stu-id="3ad47-161">Response</span></span>
<span data-ttu-id="3ad47-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ad47-162">Here is an example of the response.</span></span>
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