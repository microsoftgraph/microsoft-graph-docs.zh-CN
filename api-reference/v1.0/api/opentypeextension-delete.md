---
title: 删除开放扩展
description: 从指定的资源实例中删除开放扩展（openTypeExtension 对象）。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 9430f4480cc6d18979c9b395ecc4fc7c9bda72c4
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797150"
---
# <a name="delete-open-extension"></a><span data-ttu-id="66011-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="66011-103">Delete open extension</span></span>

<span data-ttu-id="66011-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66011-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66011-105">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="66011-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="66011-106">权限</span><span class="sxs-lookup"><span data-stu-id="66011-106">Permissions</span></span>

<span data-ttu-id="66011-107">根据要从中删除扩展的资源和权限类型 (委派或应用程序) 请求的权限，下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="66011-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="66011-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66011-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66011-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="66011-109">Supported resource</span></span> | <span data-ttu-id="66011-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66011-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66011-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66011-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66011-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="66011-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="66011-113">设备</span><span class="sxs-lookup"><span data-stu-id="66011-113">device</span></span>](../resources/device.md) | <span data-ttu-id="66011-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66011-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="66011-115">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-115">Not supported</span></span> | <span data-ttu-id="66011-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-117">事件</span><span class="sxs-lookup"><span data-stu-id="66011-117">event</span></span>](../resources/event.md) | <span data-ttu-id="66011-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="66011-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="66011-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="66011-121">组</span><span class="sxs-lookup"><span data-stu-id="66011-121">group</span></span>](../resources/group.md) | <span data-ttu-id="66011-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="66011-123">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-123">Not supported</span></span> | <span data-ttu-id="66011-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-125">组事件</span><span class="sxs-lookup"><span data-stu-id="66011-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="66011-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="66011-127">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-127">Not supported</span></span> | <span data-ttu-id="66011-128">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-128">Not supported</span></span> |
| [<span data-ttu-id="66011-129">组帖子</span><span class="sxs-lookup"><span data-stu-id="66011-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="66011-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="66011-131">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-131">Not supported</span></span> | <span data-ttu-id="66011-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-133">邮件</span><span class="sxs-lookup"><span data-stu-id="66011-133">message</span></span>](../resources/message.md) | <span data-ttu-id="66011-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-134">Mail.ReadWrite</span></span> | <span data-ttu-id="66011-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-135">Mail.ReadWrite</span></span> | <span data-ttu-id="66011-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="66011-137">组织</span><span class="sxs-lookup"><span data-stu-id="66011-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="66011-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="66011-139">不支持</span><span class="sxs-lookup"><span data-stu-id="66011-139">Not supported</span></span> | <span data-ttu-id="66011-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-140">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-141">个人联系人</span><span class="sxs-lookup"><span data-stu-id="66011-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="66011-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="66011-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="66011-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="66011-145">用户</span><span class="sxs-lookup"><span data-stu-id="66011-145">user</span></span>](../resources/user.md) | <span data-ttu-id="66011-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-146">User.ReadWrite</span></span> | <span data-ttu-id="66011-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-147">User.ReadWrite</span></span> | <span data-ttu-id="66011-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66011-148">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-149">task</span><span class="sxs-lookup"><span data-stu-id="66011-149">task</span></span>](../resources/todotask.md) | <span data-ttu-id="66011-150">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-150">Tasks.ReadWrite</span></span> | <span data-ttu-id="66011-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="66011-152">全部写读。</span><span class="sxs-lookup"><span data-stu-id="66011-152">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="66011-153">tasklist</span><span class="sxs-lookup"><span data-stu-id="66011-153">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="66011-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="66011-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66011-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="66011-156">全部写读。</span><span class="sxs-lookup"><span data-stu-id="66011-156">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66011-157">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66011-157">HTTP request</span></span>
<span data-ttu-id="66011-158">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="66011-158">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="66011-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="66011-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="66011-161">路径参数</span><span class="sxs-lookup"><span data-stu-id="66011-161">Path parameters</span></span>
|<span data-ttu-id="66011-162">参数</span><span class="sxs-lookup"><span data-stu-id="66011-162">Parameter</span></span>|<span data-ttu-id="66011-163">类型</span><span class="sxs-lookup"><span data-stu-id="66011-163">Type</span></span>|<span data-ttu-id="66011-164">说明</span><span class="sxs-lookup"><span data-stu-id="66011-164">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66011-165">id</span><span class="sxs-lookup"><span data-stu-id="66011-165">id</span></span>|<span data-ttu-id="66011-166">string</span><span class="sxs-lookup"><span data-stu-id="66011-166">string</span></span>|<span data-ttu-id="66011-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="66011-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="66011-169">extensionId</span><span class="sxs-lookup"><span data-stu-id="66011-169">extensionId</span></span>|<span data-ttu-id="66011-170">string</span><span class="sxs-lookup"><span data-stu-id="66011-170">string</span></span>|<span data-ttu-id="66011-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="66011-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="66011-174">请求标头</span><span class="sxs-lookup"><span data-stu-id="66011-174">Request headers</span></span>
| <span data-ttu-id="66011-175">名称</span><span class="sxs-lookup"><span data-stu-id="66011-175">Name</span></span>       | <span data-ttu-id="66011-176">值</span><span class="sxs-lookup"><span data-stu-id="66011-176">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="66011-177">Authorization</span><span class="sxs-lookup"><span data-stu-id="66011-177">Authorization</span></span> | <span data-ttu-id="66011-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66011-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66011-180">请求正文</span><span class="sxs-lookup"><span data-stu-id="66011-180">Request body</span></span>
<span data-ttu-id="66011-181">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66011-181">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66011-182">响应</span><span class="sxs-lookup"><span data-stu-id="66011-182">Response</span></span>

<span data-ttu-id="66011-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="66011-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66011-185">示例</span><span class="sxs-lookup"><span data-stu-id="66011-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66011-186">请求</span><span class="sxs-lookup"><span data-stu-id="66011-186">Request</span></span>
<span data-ttu-id="66011-187">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="66011-187">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="66011-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="66011-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="66011-189">C#</span><span class="sxs-lookup"><span data-stu-id="66011-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66011-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66011-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66011-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66011-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66011-192">Java</span><span class="sxs-lookup"><span data-stu-id="66011-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="66011-193">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="66011-193">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="66011-194">响应</span><span class="sxs-lookup"><span data-stu-id="66011-194">Response</span></span>
<span data-ttu-id="66011-195">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66011-195">Here is an example of the response.</span></span>
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

