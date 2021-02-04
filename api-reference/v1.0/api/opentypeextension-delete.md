---
title: 删除开放扩展
description: 从指定的资源实例中删除开放扩展（openTypeExtension 对象）。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 803478b334d267c767a0b857b7a13ce8b2f86a56
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092597"
---
# <a name="delete-open-extension"></a><span data-ttu-id="dd6fd-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="dd6fd-103">Delete open extension</span></span>

<span data-ttu-id="dd6fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd6fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd6fd-105">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

<span data-ttu-id="dd6fd-106">有关支持开放扩展的资源[](#permissions)列表，请参阅"权限"部分中的表。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-106">See the table in the [Permissions](#permissions) section for the list of resources that support open extensions.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd6fd-107">权限</span><span class="sxs-lookup"><span data-stu-id="dd6fd-107">Permissions</span></span>

<span data-ttu-id="dd6fd-108">根据从中删除扩展的资源以及请求的权限类型 (委托或应用程序) ，下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dd6fd-109">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请搜索"权限"中的以下 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd6fd-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="dd6fd-110">Supported resource</span></span> | <span data-ttu-id="dd6fd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd6fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd6fd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd6fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd6fd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd6fd-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="dd6fd-114">设备</span><span class="sxs-lookup"><span data-stu-id="dd6fd-114">device</span></span>](../resources/device.md) | <span data-ttu-id="dd6fd-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="dd6fd-116">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-116">Not supported</span></span> | <span data-ttu-id="dd6fd-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-118">事件</span><span class="sxs-lookup"><span data-stu-id="dd6fd-118">event</span></span>](../resources/event.md) | <span data-ttu-id="dd6fd-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="dd6fd-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="dd6fd-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="dd6fd-122">组</span><span class="sxs-lookup"><span data-stu-id="dd6fd-122">group</span></span>](../resources/group.md) | <span data-ttu-id="dd6fd-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd6fd-124">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-124">Not supported</span></span> | <span data-ttu-id="dd6fd-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-126">组事件</span><span class="sxs-lookup"><span data-stu-id="dd6fd-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="dd6fd-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd6fd-128">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-128">Not supported</span></span> | <span data-ttu-id="dd6fd-129">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-129">Not supported</span></span> |
| [<span data-ttu-id="dd6fd-130">组帖子</span><span class="sxs-lookup"><span data-stu-id="dd6fd-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="dd6fd-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="dd6fd-132">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-132">Not supported</span></span> | <span data-ttu-id="dd6fd-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-134">邮件</span><span class="sxs-lookup"><span data-stu-id="dd6fd-134">message</span></span>](../resources/message.md) | <span data-ttu-id="dd6fd-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-135">Mail.ReadWrite</span></span> | <span data-ttu-id="dd6fd-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-136">Mail.ReadWrite</span></span> | <span data-ttu-id="dd6fd-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="dd6fd-138">组织</span><span class="sxs-lookup"><span data-stu-id="dd6fd-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="dd6fd-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="dd6fd-140">不支持</span><span class="sxs-lookup"><span data-stu-id="dd6fd-140">Not supported</span></span> | <span data-ttu-id="dd6fd-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-141">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-142">个人联系人</span><span class="sxs-lookup"><span data-stu-id="dd6fd-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="dd6fd-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="dd6fd-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="dd6fd-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="dd6fd-146">用户</span><span class="sxs-lookup"><span data-stu-id="dd6fd-146">user</span></span>](../resources/user.md) | <span data-ttu-id="dd6fd-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-147">User.ReadWrite</span></span> | <span data-ttu-id="dd6fd-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-148">User.ReadWrite</span></span> | <span data-ttu-id="dd6fd-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-149">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-150">task</span><span class="sxs-lookup"><span data-stu-id="dd6fd-150">task</span></span>](../resources/todotask.md) | <span data-ttu-id="dd6fd-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd6fd-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd6fd-153">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-153">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="dd6fd-154">tasklist</span><span class="sxs-lookup"><span data-stu-id="dd6fd-154">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="dd6fd-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd6fd-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd6fd-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd6fd-157">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd6fd-157">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd6fd-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd6fd-158">HTTP request</span></span>
<span data-ttu-id="dd6fd-159">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-159">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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
DELETE /users/me/todo/lists/{todoTaskListId}/extensions/{extensionId}
DELETE /users/me/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
```

><span data-ttu-id="dd6fd-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="dd6fd-162">路径参数</span><span class="sxs-lookup"><span data-stu-id="dd6fd-162">Path parameters</span></span>
|<span data-ttu-id="dd6fd-163">参数</span><span class="sxs-lookup"><span data-stu-id="dd6fd-163">Parameter</span></span>|<span data-ttu-id="dd6fd-164">类型</span><span class="sxs-lookup"><span data-stu-id="dd6fd-164">Type</span></span>|<span data-ttu-id="dd6fd-165">说明</span><span class="sxs-lookup"><span data-stu-id="dd6fd-165">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dd6fd-166">id</span><span class="sxs-lookup"><span data-stu-id="dd6fd-166">id</span></span>|<span data-ttu-id="dd6fd-167">string</span><span class="sxs-lookup"><span data-stu-id="dd6fd-167">string</span></span>|<span data-ttu-id="dd6fd-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="dd6fd-170">extensionId</span><span class="sxs-lookup"><span data-stu-id="dd6fd-170">extensionId</span></span>|<span data-ttu-id="dd6fd-171">string</span><span class="sxs-lookup"><span data-stu-id="dd6fd-171">string</span></span>|<span data-ttu-id="dd6fd-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dd6fd-175">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd6fd-175">Request headers</span></span>
| <span data-ttu-id="dd6fd-176">名称</span><span class="sxs-lookup"><span data-stu-id="dd6fd-176">Name</span></span>       | <span data-ttu-id="dd6fd-177">值</span><span class="sxs-lookup"><span data-stu-id="dd6fd-177">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="dd6fd-178">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd6fd-178">Authorization</span></span> | <span data-ttu-id="dd6fd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd6fd-181">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd6fd-181">Request body</span></span>
<span data-ttu-id="dd6fd-182">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-182">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd6fd-183">响应</span><span class="sxs-lookup"><span data-stu-id="dd6fd-183">Response</span></span>

<span data-ttu-id="dd6fd-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd6fd-186">示例</span><span class="sxs-lookup"><span data-stu-id="dd6fd-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd6fd-187">请求</span><span class="sxs-lookup"><span data-stu-id="dd6fd-187">Request</span></span>
<span data-ttu-id="dd6fd-188">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-188">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd6fd-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd6fd-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="dd6fd-190">C#</span><span class="sxs-lookup"><span data-stu-id="dd6fd-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd6fd-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd6fd-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd6fd-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd6fd-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd6fd-193">Java</span><span class="sxs-lookup"><span data-stu-id="dd6fd-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="dd6fd-194">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-194">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="dd6fd-195">响应</span><span class="sxs-lookup"><span data-stu-id="dd6fd-195">Response</span></span>
<span data-ttu-id="dd6fd-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd6fd-196">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

