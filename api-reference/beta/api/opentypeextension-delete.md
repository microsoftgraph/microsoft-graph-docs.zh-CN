---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 374c018e87bf740deb9fffa357d2873dc2503c58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450238"
---
# <a name="delete-open-extension"></a><span data-ttu-id="c6c23-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="c6c23-103">Delete open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6c23-104">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="c6c23-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c6c23-105">权限</span><span class="sxs-lookup"><span data-stu-id="c6c23-105">Permissions</span></span>

<span data-ttu-id="c6c23-106">根据要从中删除扩展的资源以及请求的权限类型 (委派或应用程序), 下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="c6c23-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c6c23-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6c23-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6c23-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="c6c23-108">Supported resource</span></span> | <span data-ttu-id="c6c23-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6c23-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c6c23-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6c23-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6c23-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6c23-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c6c23-112">设备</span><span class="sxs-lookup"><span data-stu-id="c6c23-112">device</span></span>](../resources/device.md) | <span data-ttu-id="c6c23-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="c6c23-114">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-114">Not supported</span></span> | <span data-ttu-id="c6c23-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="c6c23-116">事件</span><span class="sxs-lookup"><span data-stu-id="c6c23-116">event</span></span>](../resources/event.md) | <span data-ttu-id="c6c23-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="c6c23-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="c6c23-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="c6c23-120">组</span><span class="sxs-lookup"><span data-stu-id="c6c23-120">group</span></span>](../resources/group.md) | <span data-ttu-id="c6c23-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="c6c23-122">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-122">Not supported</span></span> | <span data-ttu-id="c6c23-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="c6c23-124">组事件</span><span class="sxs-lookup"><span data-stu-id="c6c23-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="c6c23-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="c6c23-126">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-126">Not supported</span></span> | <span data-ttu-id="c6c23-127">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-127">Not supported</span></span> |
| [<span data-ttu-id="c6c23-128">组帖子</span><span class="sxs-lookup"><span data-stu-id="c6c23-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="c6c23-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="c6c23-130">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-130">Not supported</span></span> | <span data-ttu-id="c6c23-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="c6c23-132">邮件</span><span class="sxs-lookup"><span data-stu-id="c6c23-132">message</span></span>](../resources/message.md) | <span data-ttu-id="c6c23-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-133">Mail.ReadWrite</span></span> | <span data-ttu-id="c6c23-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-134">Mail.ReadWrite</span></span> | <span data-ttu-id="c6c23-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="c6c23-136">组织</span><span class="sxs-lookup"><span data-stu-id="c6c23-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="c6c23-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="c6c23-138">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-138">Not supported</span></span> | <span data-ttu-id="c6c23-139">不支持</span><span class="sxs-lookup"><span data-stu-id="c6c23-139">Not supported</span></span> |
| [<span data-ttu-id="c6c23-140">个人联系人</span><span class="sxs-lookup"><span data-stu-id="c6c23-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="c6c23-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="c6c23-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="c6c23-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c6c23-144">用户</span><span class="sxs-lookup"><span data-stu-id="c6c23-144">user</span></span>](../resources/user.md) | <span data-ttu-id="c6c23-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-145">User.ReadWrite.All</span></span> | <span data-ttu-id="c6c23-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6c23-146">User.ReadWrite</span></span> | <span data-ttu-id="c6c23-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6c23-148">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6c23-148">HTTP request</span></span>

<span data-ttu-id="c6c23-149">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="c6c23-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="c6c23-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="c6c23-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="c6c23-152">路径参数</span><span class="sxs-lookup"><span data-stu-id="c6c23-152">Path parameters</span></span>
|<span data-ttu-id="c6c23-153">**参数**</span><span class="sxs-lookup"><span data-stu-id="c6c23-153">**Parameter**</span></span>|<span data-ttu-id="c6c23-154">**类型**</span><span class="sxs-lookup"><span data-stu-id="c6c23-154">**Type**</span></span>|<span data-ttu-id="c6c23-155">**说明**</span><span class="sxs-lookup"><span data-stu-id="c6c23-155">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c6c23-156">id</span><span class="sxs-lookup"><span data-stu-id="c6c23-156">id</span></span>|<span data-ttu-id="c6c23-157">string</span><span class="sxs-lookup"><span data-stu-id="c6c23-157">string</span></span>|<span data-ttu-id="c6c23-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="c6c23-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="c6c23-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="c6c23-160">extensionId</span></span>|<span data-ttu-id="c6c23-161">string</span><span class="sxs-lookup"><span data-stu-id="c6c23-161">string</span></span>|<span data-ttu-id="c6c23-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="c6c23-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c6c23-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6c23-165">Request headers</span></span>
| <span data-ttu-id="c6c23-166">名称</span><span class="sxs-lookup"><span data-stu-id="c6c23-166">Name</span></span>       | <span data-ttu-id="c6c23-167">值</span><span class="sxs-lookup"><span data-stu-id="c6c23-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c6c23-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6c23-168">Authorization</span></span> | <span data-ttu-id="c6c23-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6c23-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6c23-171">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6c23-171">Request body</span></span>
<span data-ttu-id="c6c23-172">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6c23-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6c23-173">响应</span><span class="sxs-lookup"><span data-stu-id="c6c23-173">Response</span></span>

<span data-ttu-id="c6c23-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c6c23-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6c23-176">示例</span><span class="sxs-lookup"><span data-stu-id="c6c23-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6c23-177">请求</span><span class="sxs-lookup"><span data-stu-id="c6c23-177">Request</span></span>
<span data-ttu-id="c6c23-178">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="c6c23-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c6c23-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c6c23-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6c23-180">C#</span><span class="sxs-lookup"><span data-stu-id="c6c23-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6c23-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6c23-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6c23-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="c6c23-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c6c23-183">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="c6c23-183">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="c6c23-184">响应</span><span class="sxs-lookup"><span data-stu-id="c6c23-184">Response</span></span>
<span data-ttu-id="c6c23-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c6c23-185">Here is an example of the response.</span></span>
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
