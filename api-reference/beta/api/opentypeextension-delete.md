---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: bd19d5ca1da444171201c7dbe4cd5c016aad5352
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863381"
---
# <a name="delete-open-extension"></a><span data-ttu-id="48729-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="48729-103">Delete open extension</span></span>

<span data-ttu-id="48729-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48729-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48729-105">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="48729-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="48729-106">权限</span><span class="sxs-lookup"><span data-stu-id="48729-106">Permissions</span></span>

<span data-ttu-id="48729-107">根据要从中删除扩展的资源以及请求的权限类型（委派或应用程序），下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="48729-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="48729-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48729-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48729-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="48729-109">Supported resource</span></span> | <span data-ttu-id="48729-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48729-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48729-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48729-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48729-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="48729-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="48729-113">设备</span><span class="sxs-lookup"><span data-stu-id="48729-113">device</span></span>](../resources/device.md) | <span data-ttu-id="48729-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48729-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="48729-115">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-115">Not supported</span></span> | <span data-ttu-id="48729-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="48729-117">事件</span><span class="sxs-lookup"><span data-stu-id="48729-117">event</span></span>](../resources/event.md) | <span data-ttu-id="48729-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="48729-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="48729-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="48729-121">组</span><span class="sxs-lookup"><span data-stu-id="48729-121">group</span></span>](../resources/group.md) | <span data-ttu-id="48729-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="48729-123">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-123">Not supported</span></span> | <span data-ttu-id="48729-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="48729-125">组事件</span><span class="sxs-lookup"><span data-stu-id="48729-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="48729-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="48729-127">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-127">Not supported</span></span> | <span data-ttu-id="48729-128">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-128">Not supported</span></span> |
| [<span data-ttu-id="48729-129">组帖子</span><span class="sxs-lookup"><span data-stu-id="48729-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="48729-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="48729-131">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-131">Not supported</span></span> | <span data-ttu-id="48729-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="48729-133">邮件</span><span class="sxs-lookup"><span data-stu-id="48729-133">message</span></span>](../resources/message.md) | <span data-ttu-id="48729-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-134">Mail.ReadWrite</span></span> | <span data-ttu-id="48729-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-135">Mail.ReadWrite</span></span> | <span data-ttu-id="48729-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="48729-137">组织</span><span class="sxs-lookup"><span data-stu-id="48729-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="48729-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="48729-139">不支持</span><span class="sxs-lookup"><span data-stu-id="48729-139">Not supported</span></span> | <span data-ttu-id="48729-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-140">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="48729-141">个人联系人</span><span class="sxs-lookup"><span data-stu-id="48729-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="48729-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="48729-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="48729-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="48729-145">用户</span><span class="sxs-lookup"><span data-stu-id="48729-145">user</span></span>](../resources/user.md) | <span data-ttu-id="48729-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-146">User.ReadWrite</span></span> | <span data-ttu-id="48729-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48729-147">User.ReadWrite</span></span> | <span data-ttu-id="48729-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48729-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48729-149">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48729-149">HTTP request</span></span>

<span data-ttu-id="48729-150">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="48729-150">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
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

><span data-ttu-id="48729-151">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it.</span><span class="sxs-lookup"><span data-stu-id="48729-151">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it.</span></span> <span data-ttu-id="48729-152">All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span><span class="sxs-lookup"><span data-stu-id="48729-152">All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="48729-153">路径参数</span><span class="sxs-lookup"><span data-stu-id="48729-153">Path parameters</span></span>
|<span data-ttu-id="48729-154">**参数**</span><span class="sxs-lookup"><span data-stu-id="48729-154">**Parameter**</span></span>|<span data-ttu-id="48729-155">**类型**</span><span class="sxs-lookup"><span data-stu-id="48729-155">**Type**</span></span>|<span data-ttu-id="48729-156">**说明**</span><span class="sxs-lookup"><span data-stu-id="48729-156">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="48729-157">id</span><span class="sxs-lookup"><span data-stu-id="48729-157">id</span></span>|<span data-ttu-id="48729-158">string</span><span class="sxs-lookup"><span data-stu-id="48729-158">string</span></span>|<span data-ttu-id="48729-159">A unique identifier for an instance in the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="48729-159">A unique identifier for an instance in the corresponding collection.</span></span> <span data-ttu-id="48729-160">Required.</span><span class="sxs-lookup"><span data-stu-id="48729-160">Required.</span></span>|
|<span data-ttu-id="48729-161">extensionId</span><span class="sxs-lookup"><span data-stu-id="48729-161">extensionId</span></span>|<span data-ttu-id="48729-162">string</span><span class="sxs-lookup"><span data-stu-id="48729-162">string</span></span>|<span data-ttu-id="48729-163">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span><span class="sxs-lookup"><span data-stu-id="48729-163">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span></span> <span data-ttu-id="48729-164">The fully qualified name is returned in the `id` property when you create the extension.</span><span class="sxs-lookup"><span data-stu-id="48729-164">The fully qualified name is returned in the `id` property when you create the extension.</span></span> <span data-ttu-id="48729-165">Required.</span><span class="sxs-lookup"><span data-stu-id="48729-165">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="48729-166">请求标头</span><span class="sxs-lookup"><span data-stu-id="48729-166">Request headers</span></span>
| <span data-ttu-id="48729-167">名称</span><span class="sxs-lookup"><span data-stu-id="48729-167">Name</span></span>       | <span data-ttu-id="48729-168">值</span><span class="sxs-lookup"><span data-stu-id="48729-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="48729-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="48729-169">Authorization</span></span> | <span data-ttu-id="48729-170">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="48729-170">Bearer {token}.</span></span> <span data-ttu-id="48729-171">Required.</span><span class="sxs-lookup"><span data-stu-id="48729-171">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48729-172">请求正文</span><span class="sxs-lookup"><span data-stu-id="48729-172">Request body</span></span>
<span data-ttu-id="48729-173">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48729-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48729-174">响应</span><span class="sxs-lookup"><span data-stu-id="48729-174">Response</span></span>

<span data-ttu-id="48729-175">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="48729-175">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="48729-176">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="48729-176">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48729-177">示例</span><span class="sxs-lookup"><span data-stu-id="48729-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48729-178">请求</span><span class="sxs-lookup"><span data-stu-id="48729-178">Request</span></span>
<span data-ttu-id="48729-179">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="48729-179">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="48729-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="48729-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="48729-181">C#</span><span class="sxs-lookup"><span data-stu-id="48729-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48729-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48729-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48729-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48729-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="48729-184">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="48729-184">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="48729-185">响应</span><span class="sxs-lookup"><span data-stu-id="48729-185">Response</span></span>
<span data-ttu-id="48729-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="48729-186">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
