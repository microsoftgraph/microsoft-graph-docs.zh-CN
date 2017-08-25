# <a name="get-open-extension"></a><span data-ttu-id="be612-101">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="be612-101">Get open extension</span></span>

<span data-ttu-id="be612-102">获取用名称或完全限定的名称标识的开放扩展（[openTypeExtension](../resources/openTypeExtension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="be612-102">Get an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="be612-103">下表列出了可以从受支持的资源实例中获取开放扩展的三种应用场景。</span><span class="sxs-lookup"><span data-stu-id="be612-103">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="be612-104">**GET 应用场景**</span><span class="sxs-lookup"><span data-stu-id="be612-104">**GET scenario**</span></span>|<span data-ttu-id="be612-105">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="be612-105">**Supported resources**</span></span>|<span data-ttu-id="be612-106">**响应正文**</span><span class="sxs-lookup"><span data-stu-id="be612-106">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="be612-107">从已知资源实例中获取特定扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-107">Get a specific extension from a known resource instance.</span></span>| [<span data-ttu-id="be612-108">设备](../resources/device.md)、[事件](../resources/event.md)、[组](../resources/group.md)、[组事件](../resources/event.md)、[组帖子](../resources/post.md)、[邮件](../resources/message.md)、[组织](../resources/organization.md)、[个人联系人](../resources/contact.md)、[用户</span><span class="sxs-lookup"><span data-stu-id="be612-108">Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user</span></span>](../resources/user.md) | <span data-ttu-id="be612-109">仅开放扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-109">Open extension only.</span></span>|
|<span data-ttu-id="be612-110">获取一个通过特定扩展插件扩展的已知资源实例。</span><span class="sxs-lookup"><span data-stu-id="be612-110">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="be612-111">设备、事件、组、组事件、组帖子、邮件、组织、个人联系人、用户</span><span class="sxs-lookup"><span data-stu-id="be612-111">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="be612-112">一个通过开放扩展插件扩展的资源实例。</span><span class="sxs-lookup"><span data-stu-id="be612-112">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="be612-113">查找并展开具有特定扩展的资源实例。</span><span class="sxs-lookup"><span data-stu-id="be612-113">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="be612-114">事件、组事件、组帖子、邮件、个人联系人</span><span class="sxs-lookup"><span data-stu-id="be612-114">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="be612-115">通过开放扩展展开的资源实例。</span><span class="sxs-lookup"><span data-stu-id="be612-115">Resource instances expanded with the open extension.</span></span>|


## <a name="permissions"></a><span data-ttu-id="be612-116">权限</span><span class="sxs-lookup"><span data-stu-id="be612-116">Permissions</span></span>

<span data-ttu-id="be612-p101">要调用此 API，必须有以下权限之一，具体视包含扩展的资源而定。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="be612-p101">One of the following permissions is required to call this API, depending on the resource that contains the extension. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be612-119">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="be612-119">**Supported resource**</span></span>|<span data-ttu-id="be612-120">**权限**</span><span class="sxs-lookup"><span data-stu-id="be612-120">**Permission**</span></span>|<span data-ttu-id="be612-121">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="be612-121">**Supported resource**</span></span>|<span data-ttu-id="be612-122">**权限**</span><span class="sxs-lookup"><span data-stu-id="be612-122">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="be612-123">设备</span><span class="sxs-lookup"><span data-stu-id="be612-123">Device</span></span>](../resources/device.md) | <span data-ttu-id="be612-124">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-124">Directory.Read.All</span></span> | [<span data-ttu-id="be612-125">事件</span><span class="sxs-lookup"><span data-stu-id="be612-125">Event</span></span>](../resources/event.md) | <span data-ttu-id="be612-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="be612-126">Calendars.Read</span></span> | 
| [<span data-ttu-id="be612-127">组</span><span class="sxs-lookup"><span data-stu-id="be612-127">Group</span></span>](../resources/group.md) | <span data-ttu-id="be612-128">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-128">Group.Read.All</span></span> | [<span data-ttu-id="be612-129">组事件</span><span class="sxs-lookup"><span data-stu-id="be612-129">Group event</span></span>](../resources/event.md) | <span data-ttu-id="be612-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-130">Group.Read.All</span></span> | 
| [<span data-ttu-id="be612-131">组帖子</span><span class="sxs-lookup"><span data-stu-id="be612-131">Group post</span></span>](../resources/post.md) | <span data-ttu-id="be612-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-132">Group.Read.All</span></span> | [<span data-ttu-id="be612-133">邮件</span><span class="sxs-lookup"><span data-stu-id="be612-133">Message</span></span>](../resources/message.md) | <span data-ttu-id="be612-134">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="be612-134">Mail.Read</span></span> | 
| [<span data-ttu-id="be612-135">组织</span><span class="sxs-lookup"><span data-stu-id="be612-135">Organization</span></span>](../resources/organization.md) | <span data-ttu-id="be612-136">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-136">Directory.Read.All</span></span> | [<span data-ttu-id="be612-137">个人联系人</span><span class="sxs-lookup"><span data-stu-id="be612-137">Personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="be612-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="be612-138">Contacts.Read</span></span> |
| [<span data-ttu-id="be612-139">用户</span><span class="sxs-lookup"><span data-stu-id="be612-139">User</span></span>](../resources/user.md) | <span data-ttu-id="be612-140">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="be612-140">User.Read.All</span></span> | | |



## <a name="http-request"></a><span data-ttu-id="be612-141">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be612-141">HTTP request</span></span>

<span data-ttu-id="be612-142">本部分列出了上述三种 `GET` 应用场景中每一种的语法。</span><span class="sxs-lookup"><span data-stu-id="be612-142">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="be612-143">从已知资源实例中获取特定扩展</span><span class="sxs-lookup"><span data-stu-id="be612-143">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="be612-144">使用与获取资源实例相同的 REST 请求，并使用资源实例的 **extensions** 导航属性标识扩展插件。</span><span class="sxs-lookup"><span data-stu-id="be612-144">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="be612-145">获取一个通过匹配的扩展插件扩展的已知资源实例</span><span class="sxs-lookup"><span data-stu-id="be612-145">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="be612-p102">对于事件、组事件、组帖子、邮件、个人联系人资源类型，可使用与获取资源实例相同的 REST 请求，查找 **id** 属性与筛选器匹配的扩展插件，然后使用此扩展插件扩展这个资源实例。该响应包括大部分资源属性。</span><span class="sxs-lookup"><span data-stu-id="be612-p102">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="be612-148">对于设备、组、组织和用户资源类型，你必须也使用 `$select` 参数以包括 **id** 属性及你在资源实例中所需的任何其他属性：</span><span class="sxs-lookup"><span data-stu-id="be612-148">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="be612-149">筛选出多个通过匹配的扩展插件扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="be612-149">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="be612-150">使用与获取一组受支持的资源相同的 REST 请求，筛选出扩展插件包含匹配的 **id** 属性的一组实例，然后使用此扩展插件扩展这些实例。</span><span class="sxs-lookup"><span data-stu-id="be612-150">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="be612-p103">**注意：**以上语法显示了一些标识资源实例或集合的常见方法，以便从中获取扩展。可以用来识别这些资源实例或集合的所有其他语法均支持以类似的方式从中获取开放扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="be612-153">参数</span><span class="sxs-lookup"><span data-stu-id="be612-153">Parameters</span></span>
|<span data-ttu-id="be612-154">**参数**</span><span class="sxs-lookup"><span data-stu-id="be612-154">**Parameter**</span></span>|<span data-ttu-id="be612-155">**类型**</span><span class="sxs-lookup"><span data-stu-id="be612-155">**Type**</span></span>|<span data-ttu-id="be612-156">**说明**</span><span class="sxs-lookup"><span data-stu-id="be612-156">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="be612-157">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="be612-157">_URL parameters_</span></span>|
|<span data-ttu-id="be612-158">Id</span><span class="sxs-lookup"><span data-stu-id="be612-158">Id</span></span>|<span data-ttu-id="be612-159">string</span><span class="sxs-lookup"><span data-stu-id="be612-159">string</span></span>|<span data-ttu-id="be612-p104">邮件、事件、联系人等相应集合中的对象的唯一标识符的占位符。必需。不要与 **openTypeExtension** 的 **id** 属性混淆。</span><span class="sxs-lookup"><span data-stu-id="be612-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="be612-163">extensionId</span><span class="sxs-lookup"><span data-stu-id="be612-163">extensionId</span></span>|<span data-ttu-id="be612-164">string</span><span class="sxs-lookup"><span data-stu-id="be612-164">string</span></span>|<span data-ttu-id="be612-p105">扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）的占位符。创建扩展时，在 **id** 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="be612-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|


## <a name="optional-query-parameters"></a><span data-ttu-id="be612-168">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be612-168">Optional query parameters</span></span>

<span data-ttu-id="be612-169">请确保对 `$filter` 字符串中的空格字符应用 [URL 编码](http://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="be612-169">Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="be612-170">**名称**</span><span class="sxs-lookup"><span data-stu-id="be612-170">**Name**</span></span>|<span data-ttu-id="be612-171">**值**</span><span class="sxs-lookup"><span data-stu-id="be612-171">**Value**</span></span>|<span data-ttu-id="be612-172">**说明**</span><span class="sxs-lookup"><span data-stu-id="be612-172">**Description**</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="be612-173">$filter</span><span class="sxs-lookup"><span data-stu-id="be612-173">$filter</span></span>|<span data-ttu-id="be612-174">string</span><span class="sxs-lookup"><span data-stu-id="be612-174">string</span></span>|<span data-ttu-id="be612-175">返回其 **id** 与 `extensionId` 参数值匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-175">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="be612-176">具有 **any** 运算符的 $filter</span><span class="sxs-lookup"><span data-stu-id="be612-176">$filter with **any** operator</span></span>|<span data-ttu-id="be612-177">string</span><span class="sxs-lookup"><span data-stu-id="be612-177">string</span></span>|<span data-ttu-id="be612-178">返回特定资源集合的实例，其中包含其 **id** 与 `extensionId` 参数值匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-178">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>| 
|<span data-ttu-id="be612-179">$expand</span><span class="sxs-lookup"><span data-stu-id="be612-179">$expand</span></span>|<span data-ttu-id="be612-180">string</span><span class="sxs-lookup"><span data-stu-id="be612-180">string</span></span>|<span data-ttu-id="be612-181">展开资源实例以包含扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-181">Expands a resource instance to include an extension.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="be612-182">请求标头</span><span class="sxs-lookup"><span data-stu-id="be612-182">Request headers</span></span>
| <span data-ttu-id="be612-183">名称</span><span class="sxs-lookup"><span data-stu-id="be612-183">Name</span></span>       | <span data-ttu-id="be612-184">值</span><span class="sxs-lookup"><span data-stu-id="be612-184">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="be612-185">Authorization</span><span class="sxs-lookup"><span data-stu-id="be612-185">Authorization</span></span> | <span data-ttu-id="be612-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be612-p106">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="be612-188">请求正文</span><span class="sxs-lookup"><span data-stu-id="be612-188">Request body</span></span>
<span data-ttu-id="be612-189">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be612-189">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be612-190">响应</span><span class="sxs-lookup"><span data-stu-id="be612-190">Response</span></span>

<span data-ttu-id="be612-p107">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [openTypeExtension](../resources/opentypeextension.md) 对象。根据 GET 查询，准确的响应正文有所不同。</span><span class="sxs-lookup"><span data-stu-id="be612-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="be612-193">示例</span><span class="sxs-lookup"><span data-stu-id="be612-193">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="be612-194">请求 1</span><span class="sxs-lookup"><span data-stu-id="be612-194">Request 1</span></span>

<span data-ttu-id="be612-p108">第一个示例展示引用扩展的两种方式并获取指定邮件中的扩展。无论用于引用扩展的方式为何，该响应都相同。</span><span class="sxs-lookup"><span data-stu-id="be612-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="be612-197">首先，通过它的名称：</span><span class="sxs-lookup"><span data-stu-id="be612-197">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="be612-198">其次，通过其 ID（完全限定的名称）：</span><span class="sxs-lookup"><span data-stu-id="be612-198">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="be612-199">响应 1</span><span class="sxs-lookup"><span data-stu-id="be612-199">Response 1</span></span>
<span data-ttu-id="be612-200">下面是第一个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="be612-200">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="be612-201">请求 2</span><span class="sxs-lookup"><span data-stu-id="be612-201">Request 2</span></span>

<span data-ttu-id="be612-202">第二个实例通过其名称引用扩展并获取指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-202">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions('Com.Contoso.Deal') 
```

#### <a name="response-2"></a><span data-ttu-id="be612-203">响应 2</span><span class="sxs-lookup"><span data-stu-id="be612-203">Response 2</span></span>

<span data-ttu-id="be612-204">下面是第二个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="be612-204">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="be612-205">请求 3</span><span class="sxs-lookup"><span data-stu-id="be612-205">Request 3</span></span>

<span data-ttu-id="be612-p109">第三个示例通过包括筛选器返回的扩展获取并展开指定的邮件。此筛选器返回其 **id** 与完全限定的名称匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="be612-208">响应 3</span><span class="sxs-lookup"><span data-stu-id="be612-208">Response 3</span></span>

<span data-ttu-id="be612-p110">下面是第三个示例的响应。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be612-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="be612-212">请求 4</span><span class="sxs-lookup"><span data-stu-id="be612-212">Request 4</span></span>

<span data-ttu-id="be612-213">第四个示例通过其完全限定的名称引用扩展并获取指定组帖子中的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-213">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate') 
```

#### <a name="response-4"></a><span data-ttu-id="be612-214">响应 4</span><span class="sxs-lookup"><span data-stu-id="be612-214">Response 4</span></span>

<span data-ttu-id="be612-215">下面是第四个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="be612-215">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="be612-216">响应 5</span><span class="sxs-lookup"><span data-stu-id="be612-216">Request 5</span></span>

<span data-ttu-id="be612-p111">第五个示例查看已登录用户的邮箱中的所有邮件，并查找包含与筛选器匹配的扩展的邮件，然后通过包括扩展将其展开。此筛选器将返回其 **id** 属性与扩展名 `Com.Contoso.Referral` 匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="be612-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="be612-219">响应 5</span><span class="sxs-lookup"><span data-stu-id="be612-219">Response 5</span></span>

<span data-ttu-id="be612-220">在第五个示例的响应中，用户邮箱中仅有一封邮件，其 **id** 等于 `Com.Contoso.Referral`。</span><span class="sxs-lookup"><span data-stu-id="be612-220">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="be612-p112">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be612-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
