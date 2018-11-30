---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
ms.openlocfilehash: 9906b0b68711f1bb78d220252366b0c4a56592fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011549"
---
# <a name="delete-open-extension"></a><span data-ttu-id="944a1-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="944a1-103">Delete open extension</span></span>

<span data-ttu-id="944a1-104">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="944a1-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="944a1-105">权限</span><span class="sxs-lookup"><span data-stu-id="944a1-105">Permissions</span></span>

<span data-ttu-id="944a1-106">根据您正在删除扩展名的资源和权限类型 （委派或应用程序） 请求下, 表中所指定的权限是最小特权需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="944a1-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="944a1-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="944a1-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="944a1-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="944a1-108">Supported resource</span></span> | <span data-ttu-id="944a1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="944a1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="944a1-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="944a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="944a1-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="944a1-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="944a1-112">设备</span><span class="sxs-lookup"><span data-stu-id="944a1-112">device</span></span>](../resources/device.md) | <span data-ttu-id="944a1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="944a1-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="944a1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-114">Not supported</span></span> | <span data-ttu-id="944a1-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="944a1-116">事件</span><span class="sxs-lookup"><span data-stu-id="944a1-116">event</span></span>](../resources/event.md) | <span data-ttu-id="944a1-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="944a1-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="944a1-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="944a1-120">组</span><span class="sxs-lookup"><span data-stu-id="944a1-120">group</span></span>](../resources/group.md) | <span data-ttu-id="944a1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="944a1-122">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-122">Not supported</span></span> | <span data-ttu-id="944a1-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="944a1-124">组事件</span><span class="sxs-lookup"><span data-stu-id="944a1-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="944a1-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="944a1-126">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-126">Not supported</span></span> | <span data-ttu-id="944a1-127">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-127">Not supported</span></span> |
| [<span data-ttu-id="944a1-128">组帖子</span><span class="sxs-lookup"><span data-stu-id="944a1-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="944a1-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="944a1-130">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-130">Not supported</span></span> | <span data-ttu-id="944a1-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="944a1-132">邮件</span><span class="sxs-lookup"><span data-stu-id="944a1-132">message</span></span>](../resources/message.md) | <span data-ttu-id="944a1-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-133">Mail.ReadWrite</span></span> | <span data-ttu-id="944a1-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-134">Mail.ReadWrite</span></span> | <span data-ttu-id="944a1-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="944a1-136">组织</span><span class="sxs-lookup"><span data-stu-id="944a1-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="944a1-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="944a1-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="944a1-138">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-138">Not supported</span></span> | <span data-ttu-id="944a1-139">不支持</span><span class="sxs-lookup"><span data-stu-id="944a1-139">Not supported</span></span> |
| [<span data-ttu-id="944a1-140">个人联系人</span><span class="sxs-lookup"><span data-stu-id="944a1-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="944a1-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="944a1-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="944a1-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="944a1-144">用户</span><span class="sxs-lookup"><span data-stu-id="944a1-144">user</span></span>](../resources/user.md) | <span data-ttu-id="944a1-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-145">User.ReadWrite.All</span></span> | <span data-ttu-id="944a1-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="944a1-146">User.ReadWrite</span></span> | <span data-ttu-id="944a1-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="944a1-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="944a1-148">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="944a1-148">HTTP request</span></span>
<span data-ttu-id="944a1-149">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="944a1-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="944a1-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="944a1-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="944a1-152">路径参数</span><span class="sxs-lookup"><span data-stu-id="944a1-152">Path parameters</span></span>
|<span data-ttu-id="944a1-153">参数</span><span class="sxs-lookup"><span data-stu-id="944a1-153">Parameter</span></span>|<span data-ttu-id="944a1-154">类型</span><span class="sxs-lookup"><span data-stu-id="944a1-154">Type</span></span>|<span data-ttu-id="944a1-155">说明</span><span class="sxs-lookup"><span data-stu-id="944a1-155">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="944a1-156">ID</span><span class="sxs-lookup"><span data-stu-id="944a1-156">id</span></span>|<span data-ttu-id="944a1-157">string</span><span class="sxs-lookup"><span data-stu-id="944a1-157">string</span></span>|<span data-ttu-id="944a1-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="944a1-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="944a1-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="944a1-160">extensionId</span></span>|<span data-ttu-id="944a1-161">string</span><span class="sxs-lookup"><span data-stu-id="944a1-161">string</span></span>|<span data-ttu-id="944a1-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="944a1-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="944a1-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="944a1-165">Request headers</span></span>
| <span data-ttu-id="944a1-166">名称</span><span class="sxs-lookup"><span data-stu-id="944a1-166">Name</span></span>       | <span data-ttu-id="944a1-167">值</span><span class="sxs-lookup"><span data-stu-id="944a1-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="944a1-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="944a1-168">Authorization</span></span> | <span data-ttu-id="944a1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="944a1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="944a1-171">请求正文</span><span class="sxs-lookup"><span data-stu-id="944a1-171">Request body</span></span>
<span data-ttu-id="944a1-172">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="944a1-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="944a1-173">响应</span><span class="sxs-lookup"><span data-stu-id="944a1-173">Response</span></span>

<span data-ttu-id="944a1-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="944a1-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="944a1-176">示例</span><span class="sxs-lookup"><span data-stu-id="944a1-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="944a1-177">请求</span><span class="sxs-lookup"><span data-stu-id="944a1-177">Request</span></span>
<span data-ttu-id="944a1-178">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="944a1-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="944a1-179">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="944a1-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="944a1-180">响应</span><span class="sxs-lookup"><span data-stu-id="944a1-180">Response</span></span>
<span data-ttu-id="944a1-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="944a1-181">Here is an example of the response.</span></span>
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