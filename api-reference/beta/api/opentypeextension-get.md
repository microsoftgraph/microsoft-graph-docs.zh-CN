---
title: 获取开放扩展
description: 获取按名称或完全限定的名称标识的开放扩展（openTypeExtension 对象）。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 461cde694e9c9aff3738e5e2a3642b0ae82828b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051121"
---
# <a name="get-open-extension"></a><span data-ttu-id="71897-103">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="71897-103">Get open extension</span></span>

<span data-ttu-id="71897-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71897-105">获取用名称或完全限定的名称标识的开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="71897-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="71897-106">"权限" ["](#permissions) "部分中列出支持打开扩展的资源。</span><span class="sxs-lookup"><span data-stu-id="71897-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

<span data-ttu-id="71897-107">下表列出了可以从受支持的资源实例中获取开放扩展的三种应用场景。</span><span class="sxs-lookup"><span data-stu-id="71897-107">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="71897-108">**GET 应用场景**</span><span class="sxs-lookup"><span data-stu-id="71897-108">**GET scenario**</span></span>|<span data-ttu-id="71897-109">**支持的资源**</span><span class="sxs-lookup"><span data-stu-id="71897-109">**Supported resources**</span></span>|<span data-ttu-id="71897-110">**响应正文**</span><span class="sxs-lookup"><span data-stu-id="71897-110">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="71897-111">从已知资源实例中获取特定扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-111">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="71897-112">[管理单元](../resources/administrativeunit.md)、[设备](../resources/device.md)[、事件](../resources/event.md)、[组](../resources/group.md)、[组事件](../resources/event.md)、[组帖子](../resources/post.md)、[邮件](../resources/message.md)[、组织](../resources/organization.md)[、个人联系人](../resources/contact.md)、[用户、](../resources/user.md)[任务、](../resources/todotask.md)[任务列表](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="71897-112">[Administrative unit](../resources/administrativeunit.md), [device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md), [task](../resources/todotask.md), [tasklist](../resources/todotasklist.md)</span></span>  | <span data-ttu-id="71897-113">仅开放扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-113">Open extension only.</span></span>|
|<span data-ttu-id="71897-114">获取一个通过特定扩展插件扩展的已知资源实例。</span><span class="sxs-lookup"><span data-stu-id="71897-114">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="71897-115">管理单元、设备、事件、组、组事件、组帖子、邮件、组织、个人联系人、用户、任务、任务列表。</span><span class="sxs-lookup"><span data-stu-id="71897-115">Administrative unit, device, event, group, group event, group post, message, organization, personal contact, user, task, task list.</span></span> |<span data-ttu-id="71897-116">一个通过开放扩展插件扩展的资源实例。</span><span class="sxs-lookup"><span data-stu-id="71897-116">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="71897-117">查找并展开具有特定扩展的资源实例。</span><span class="sxs-lookup"><span data-stu-id="71897-117">Find and expand resource instances with a specific extension.</span></span> | <span data-ttu-id="71897-118">事件、组事件、组帖子、邮件、个人联系人、任务、任务列表</span><span class="sxs-lookup"><span data-stu-id="71897-118">Event, group event, group post, message, personal contact, task, task list</span></span> |<span data-ttu-id="71897-119">通过开放扩展展开的资源实例。</span><span class="sxs-lookup"><span data-stu-id="71897-119">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="71897-120">权限</span><span class="sxs-lookup"><span data-stu-id="71897-120">Permissions</span></span>

<span data-ttu-id="71897-121">根据包含扩展的资源和所请求的权限类型（委派或应用程序），下表中指定的权限是指调用此 API 所需的最低限度的特权。</span><span class="sxs-lookup"><span data-stu-id="71897-121">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="71897-122">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71897-122">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71897-123">支持的资源</span><span class="sxs-lookup"><span data-stu-id="71897-123">Supported resource</span></span> | <span data-ttu-id="71897-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71897-124">Delegated (work or school account)</span></span> | <span data-ttu-id="71897-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71897-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71897-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="71897-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="71897-127">设备</span><span class="sxs-lookup"><span data-stu-id="71897-127">device</span></span>](../resources/device.md) | <span data-ttu-id="71897-128">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-128">Directory.Read.All</span></span> | <span data-ttu-id="71897-129">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-129">Not supported</span></span> | <span data-ttu-id="71897-130">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71897-130">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="71897-131">event</span><span class="sxs-lookup"><span data-stu-id="71897-131">event</span></span>](../resources/event.md) | <span data-ttu-id="71897-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="71897-132">Calendars.Read</span></span> | <span data-ttu-id="71897-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="71897-133">Calendars.Read</span></span> | <span data-ttu-id="71897-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="71897-134">Calendars.Read</span></span> |
| [<span data-ttu-id="71897-135">组</span><span class="sxs-lookup"><span data-stu-id="71897-135">group</span></span>](../resources/group.md) | <span data-ttu-id="71897-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-136">Group.Read.All</span></span> | <span data-ttu-id="71897-137">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-137">Not supported</span></span> | <span data-ttu-id="71897-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-138">Group.Read.All</span></span> |
| [<span data-ttu-id="71897-139">组事件</span><span class="sxs-lookup"><span data-stu-id="71897-139">group event</span></span>](../resources/event.md) | <span data-ttu-id="71897-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-140">Group.Read.All</span></span> | <span data-ttu-id="71897-141">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-141">Not supported</span></span> | <span data-ttu-id="71897-142">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-142">Not supported</span></span> |
| [<span data-ttu-id="71897-143">组帖子</span><span class="sxs-lookup"><span data-stu-id="71897-143">group post</span></span>](../resources/post.md) | <span data-ttu-id="71897-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-144">Group.Read.All</span></span> | <span data-ttu-id="71897-145">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-145">Not supported</span></span> | <span data-ttu-id="71897-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-146">Group.Read.All</span></span> |
| [<span data-ttu-id="71897-147">message</span><span class="sxs-lookup"><span data-stu-id="71897-147">message</span></span>](../resources/message.md) | <span data-ttu-id="71897-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="71897-148">Mail.Read</span></span> | <span data-ttu-id="71897-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="71897-149">Mail.Read</span></span> | <span data-ttu-id="71897-150">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="71897-150">Mail.Read</span></span> | 
| [<span data-ttu-id="71897-151">组织</span><span class="sxs-lookup"><span data-stu-id="71897-151">organization</span></span>](../resources/organization.md) | <span data-ttu-id="71897-152">User.Read</span><span class="sxs-lookup"><span data-stu-id="71897-152">User.Read</span></span> | <span data-ttu-id="71897-153">不支持</span><span class="sxs-lookup"><span data-stu-id="71897-153">Not supported</span></span> | <span data-ttu-id="71897-154">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-154">Organization.Read.All</span></span> |
| [<span data-ttu-id="71897-155">个人联系人</span><span class="sxs-lookup"><span data-stu-id="71897-155">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="71897-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="71897-156">Contacts.Read</span></span> | <span data-ttu-id="71897-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="71897-157">Contacts.Read</span></span> | <span data-ttu-id="71897-158">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="71897-158">Contacts.Read</span></span> |
| [<span data-ttu-id="71897-159">用户</span><span class="sxs-lookup"><span data-stu-id="71897-159">user</span></span>](../resources/user.md) | <span data-ttu-id="71897-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="71897-160">User.Read</span></span> | <span data-ttu-id="71897-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="71897-161">User.Read</span></span> | <span data-ttu-id="71897-162">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="71897-162">User.Read.All</span></span> |
| [<span data-ttu-id="71897-163">任务</span><span class="sxs-lookup"><span data-stu-id="71897-163">task</span></span>](../resources/todotask.md) | <span data-ttu-id="71897-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71897-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="71897-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71897-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="71897-166">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71897-166">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="71897-167">任务列表</span><span class="sxs-lookup"><span data-stu-id="71897-167">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="71897-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71897-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="71897-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71897-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="71897-170">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71897-170">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71897-171">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71897-171">HTTP request</span></span>

<span data-ttu-id="71897-172">本部分列出了上述三种 `GET` 应用场景中每一种的语法。</span><span class="sxs-lookup"><span data-stu-id="71897-172">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="71897-173">从已知资源实例中获取特定扩展</span><span class="sxs-lookup"><span data-stu-id="71897-173">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="71897-174">使用与获取资源实例相同的 REST 请求，并使用资源实例的 **extensions** 导航属性标识扩展插件。</span><span class="sxs-lookup"><span data-stu-id="71897-174">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{Id}/extensions/{extensionId}
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/extensions/{extensionId}
```

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="71897-175">获取一个通过匹配的扩展插件扩展的已知资源实例</span><span class="sxs-lookup"><span data-stu-id="71897-175">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="71897-176">对于事件、组事件、组帖子、邮件、个人联系人、任务、任务列表资源类型，可使用与获取资源实例相同的 REST 请求，查找与其 **id** 属性上的筛选器匹配的扩展，然后使用此扩展来扩展实例。</span><span class="sxs-lookup"><span data-stu-id="71897-176">For the event, group event, group post, message, personal contact, task, task list resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="71897-177">该响应包括大部分资源属性。</span><span class="sxs-lookup"><span data-stu-id="71897-177">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="71897-178">对于设备、组、组织和用户资源类型，你必须也使用 `$select` 参数以包括 **id** 属性及你在资源实例中所需的任何其他属性：</span><span class="sxs-lookup"><span data-stu-id="71897-178">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```


### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="71897-179">筛选出多个通过匹配的扩展插件扩展的资源实例</span><span class="sxs-lookup"><span data-stu-id="71897-179">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="71897-180">使用与获取一组受支持的资源相同的 REST 请求，筛选出扩展插件包含匹配的 **id** 属性的一组实例，然后使用此扩展插件扩展这些实例。</span><span class="sxs-lookup"><span data-stu-id="71897-180">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="71897-p103">**注意：** 以上语法显示了一些标识资源实例或集合的常见方法，以便从中获取扩展。可以用来识别这些资源实例或集合的所有其他语法均支持以类似的方式从中获取开放扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="71897-183">路径参数</span><span class="sxs-lookup"><span data-stu-id="71897-183">Path parameters</span></span>
|<span data-ttu-id="71897-184">**参数**</span><span class="sxs-lookup"><span data-stu-id="71897-184">**Parameter**</span></span>|<span data-ttu-id="71897-185">**类型**</span><span class="sxs-lookup"><span data-stu-id="71897-185">**Type**</span></span>|<span data-ttu-id="71897-186">**说明**</span><span class="sxs-lookup"><span data-stu-id="71897-186">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="71897-187">Id</span><span class="sxs-lookup"><span data-stu-id="71897-187">Id</span></span>|<span data-ttu-id="71897-188">string</span><span class="sxs-lookup"><span data-stu-id="71897-188">string</span></span>|<span data-ttu-id="71897-p104">邮件、事件、联系人等相应集合中的对象的唯一标识符的占位符。必需。不要与 **openTypeExtension** 的 **id** 属性混淆。</span><span class="sxs-lookup"><span data-stu-id="71897-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="71897-192">extensionId</span><span class="sxs-lookup"><span data-stu-id="71897-192">extensionId</span></span>|<span data-ttu-id="71897-193">string</span><span class="sxs-lookup"><span data-stu-id="71897-193">string</span></span>|<span data-ttu-id="71897-p105">扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）的占位符。创建扩展时，在 **id** 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="71897-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="71897-197">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71897-197">Optional query parameters</span></span>

<span data-ttu-id="71897-198">请确保对 `$filter` 字符串中的空格字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="71897-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="71897-199">参数</span><span class="sxs-lookup"><span data-stu-id="71897-199">Parameter</span></span>|<span data-ttu-id="71897-200">说明</span><span class="sxs-lookup"><span data-stu-id="71897-200">Description</span></span>|<span data-ttu-id="71897-201">示例</span><span class="sxs-lookup"><span data-stu-id="71897-201">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="71897-202">$filter</span><span class="sxs-lookup"><span data-stu-id="71897-202">$filter</span></span>|<span data-ttu-id="71897-203">返回其 **id** 与 `extensionId` 参数值匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-203">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="71897-204">请求 3</span><span class="sxs-lookup"><span data-stu-id="71897-204">Request 3</span></span>](#request-3)|
|<span data-ttu-id="71897-205">具有 **any** 运算符的 $filter</span><span class="sxs-lookup"><span data-stu-id="71897-205">$filter with **any** operator</span></span>|<span data-ttu-id="71897-206">返回一个资源集合的实例，其中包含其 **id** 与 `extensionId` 参数值匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-206">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="71897-207">请求 5</span><span class="sxs-lookup"><span data-stu-id="71897-207">Request 5</span></span>](#request-5)|
|<span data-ttu-id="71897-208">$expand</span><span class="sxs-lookup"><span data-stu-id="71897-208">$expand</span></span>|<span data-ttu-id="71897-209">展开资源实例以包含扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-209">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="71897-210">[请求 3](#request-3) 和[请求 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="71897-210">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="71897-211">请求标头</span><span class="sxs-lookup"><span data-stu-id="71897-211">Request headers</span></span>
| <span data-ttu-id="71897-212">名称</span><span class="sxs-lookup"><span data-stu-id="71897-212">Name</span></span>       | <span data-ttu-id="71897-213">值</span><span class="sxs-lookup"><span data-stu-id="71897-213">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="71897-214">Authorization</span><span class="sxs-lookup"><span data-stu-id="71897-214">Authorization</span></span> | <span data-ttu-id="71897-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71897-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71897-217">请求正文</span><span class="sxs-lookup"><span data-stu-id="71897-217">Request body</span></span>
<span data-ttu-id="71897-218">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71897-218">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71897-219">响应</span><span class="sxs-lookup"><span data-stu-id="71897-219">Response</span></span>

<span data-ttu-id="71897-p107">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [openTypeExtension](../resources/opentypeextension.md) 对象。根据 GET 查询，准确的响应正文有所不同。</span><span class="sxs-lookup"><span data-stu-id="71897-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="71897-222">示例</span><span class="sxs-lookup"><span data-stu-id="71897-222">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="71897-223">请求 1</span><span class="sxs-lookup"><span data-stu-id="71897-223">Request 1</span></span>

<span data-ttu-id="71897-p108">第一个示例展示引用扩展的两种方式并获取指定邮件中的扩展。无论用于引用扩展的方式为何，该响应都相同。</span><span class="sxs-lookup"><span data-stu-id="71897-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="71897-226">首先，通过它的名称：</span><span class="sxs-lookup"><span data-stu-id="71897-226">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="71897-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="71897-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="71897-228">C#</span><span class="sxs-lookup"><span data-stu-id="71897-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71897-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71897-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71897-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71897-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71897-231">Java</span><span class="sxs-lookup"><span data-stu-id="71897-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="71897-232">其次，通过其 ID（完全限定的名称）：</span><span class="sxs-lookup"><span data-stu-id="71897-232">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="71897-233">响应 1</span><span class="sxs-lookup"><span data-stu-id="71897-233">Response 1</span></span>
<span data-ttu-id="71897-234">下面是第一个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="71897-234">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="71897-235">请求 2</span><span class="sxs-lookup"><span data-stu-id="71897-235">Request 2</span></span>

<span data-ttu-id="71897-236">第二个实例通过其名称引用扩展并获取指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-236">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="71897-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="71897-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal
```
# <a name="c"></a>[<span data-ttu-id="71897-238">C#</span><span class="sxs-lookup"><span data-stu-id="71897-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71897-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71897-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71897-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71897-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71897-241">Java</span><span class="sxs-lookup"><span data-stu-id="71897-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="71897-242">响应 2</span><span class="sxs-lookup"><span data-stu-id="71897-242">Response 2</span></span>

<span data-ttu-id="71897-243">下面是第二个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="71897-243">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl7IsAAA%3D/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="71897-244">请求 3</span><span class="sxs-lookup"><span data-stu-id="71897-244">Request 3</span></span>

<span data-ttu-id="71897-p109">第三个示例通过包括筛选器返回的扩展获取并展开指定的邮件。此筛选器返回其 **id** 与完全限定的名称匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="71897-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="71897-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="71897-248">C#</span><span class="sxs-lookup"><span data-stu-id="71897-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71897-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71897-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71897-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71897-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71897-251">Java</span><span class="sxs-lookup"><span data-stu-id="71897-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="71897-252">响应 3</span><span class="sxs-lookup"><span data-stu-id="71897-252">Response 3</span></span>

<span data-ttu-id="71897-253">下面是第三个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="71897-253">And here is the response from the third example.</span></span> <span data-ttu-id="71897-254">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71897-254">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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

#### <a name="request-4"></a><span data-ttu-id="71897-255">请求 4</span><span class="sxs-lookup"><span data-stu-id="71897-255">Request 4</span></span>

<span data-ttu-id="71897-256">第四个示例通过其完全限定的名称引用扩展并获取指定组帖子中的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-256">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>


# <a name="http"></a>[<span data-ttu-id="71897-257">HTTP</span><span class="sxs-lookup"><span data-stu-id="71897-257">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```
# <a name="c"></a>[<span data-ttu-id="71897-258">C#</span><span class="sxs-lookup"><span data-stu-id="71897-258">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71897-259">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71897-259">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71897-260">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71897-260">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71897-261">Java</span><span class="sxs-lookup"><span data-stu-id="71897-261">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-4"></a><span data-ttu-id="71897-262">响应 4</span><span class="sxs-lookup"><span data-stu-id="71897-262">Response 4</span></span>

<span data-ttu-id="71897-263">下面是第四个示例的响应。</span><span class="sxs-lookup"><span data-stu-id="71897-263">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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


#### <a name="request-5"></a><span data-ttu-id="71897-264">响应 5</span><span class="sxs-lookup"><span data-stu-id="71897-264">Request 5</span></span>

<span data-ttu-id="71897-p111">第五个示例查看已登录用户的邮箱中的所有邮件，并查找包含与筛选器匹配的扩展的邮件，然后通过包括扩展将其展开。此筛选器将返回其 **id** 属性与扩展名 `Com.Contoso.Referral` 匹配的扩展。</span><span class="sxs-lookup"><span data-stu-id="71897-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="71897-267">响应 5</span><span class="sxs-lookup"><span data-stu-id="71897-267">Response 5</span></span>

<span data-ttu-id="71897-268">在第五个示例的响应中，用户邮箱中仅有一封邮件，其 **id** 等于 `Com.Contoso.Referral`。</span><span class="sxs-lookup"><span data-stu-id="71897-268">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="71897-269">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71897-269">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


