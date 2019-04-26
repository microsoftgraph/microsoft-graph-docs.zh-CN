---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 157fe63cf76273e9e968cac890a336e33f5124d0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338122"
---
# <a name="delete-open-extension"></a><span data-ttu-id="1fe9d-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="1fe9d-103">Delete open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fe9d-104">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1fe9d-105">权限</span><span class="sxs-lookup"><span data-stu-id="1fe9d-105">Permissions</span></span>

<span data-ttu-id="1fe9d-106">根据要从中删除扩展的资源以及请求的权限类型 (委派或应用程序), 下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1fe9d-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fe9d-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="1fe9d-108">Supported resource</span></span> | <span data-ttu-id="1fe9d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fe9d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1fe9d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fe9d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fe9d-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fe9d-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="1fe9d-112">设备</span><span class="sxs-lookup"><span data-stu-id="1fe9d-112">device</span></span>](../resources/device.md) | <span data-ttu-id="1fe9d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="1fe9d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-114">Not supported</span></span> | <span data-ttu-id="1fe9d-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="1fe9d-116">event</span><span class="sxs-lookup"><span data-stu-id="1fe9d-116">event</span></span>](../resources/event.md) | <span data-ttu-id="1fe9d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="1fe9d-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="1fe9d-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="1fe9d-120">组</span><span class="sxs-lookup"><span data-stu-id="1fe9d-120">group</span></span>](../resources/group.md) | <span data-ttu-id="1fe9d-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="1fe9d-122">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-122">Not supported</span></span> | <span data-ttu-id="1fe9d-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="1fe9d-124">组事件</span><span class="sxs-lookup"><span data-stu-id="1fe9d-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="1fe9d-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="1fe9d-126">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-126">Not supported</span></span> | <span data-ttu-id="1fe9d-127">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-127">Not supported</span></span> |
| [<span data-ttu-id="1fe9d-128">组帖子</span><span class="sxs-lookup"><span data-stu-id="1fe9d-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="1fe9d-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="1fe9d-130">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-130">Not supported</span></span> | <span data-ttu-id="1fe9d-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="1fe9d-132">邮件</span><span class="sxs-lookup"><span data-stu-id="1fe9d-132">message</span></span>](../resources/message.md) | <span data-ttu-id="1fe9d-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-133">Mail.ReadWrite</span></span> | <span data-ttu-id="1fe9d-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-134">Mail.ReadWrite</span></span> | <span data-ttu-id="1fe9d-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="1fe9d-136">组织</span><span class="sxs-lookup"><span data-stu-id="1fe9d-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="1fe9d-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="1fe9d-138">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-138">Not supported</span></span> | <span data-ttu-id="1fe9d-139">不支持</span><span class="sxs-lookup"><span data-stu-id="1fe9d-139">Not supported</span></span> |
| [<span data-ttu-id="1fe9d-140">个人联系人</span><span class="sxs-lookup"><span data-stu-id="1fe9d-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="1fe9d-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="1fe9d-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="1fe9d-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="1fe9d-144">用户</span><span class="sxs-lookup"><span data-stu-id="1fe9d-144">user</span></span>](../resources/user.md) | <span data-ttu-id="1fe9d-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-145">User.ReadWrite.All</span></span> | <span data-ttu-id="1fe9d-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe9d-146">User.ReadWrite</span></span> | <span data-ttu-id="1fe9d-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fe9d-148">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fe9d-148">HTTP request</span></span>

<span data-ttu-id="1fe9d-149">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="1fe9d-p102">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="1fe9d-152">路径参数</span><span class="sxs-lookup"><span data-stu-id="1fe9d-152">Path parameters</span></span>
|<span data-ttu-id="1fe9d-153">**参数**</span><span class="sxs-lookup"><span data-stu-id="1fe9d-153">**Parameter**</span></span>|<span data-ttu-id="1fe9d-154">**类型**</span><span class="sxs-lookup"><span data-stu-id="1fe9d-154">**Type**</span></span>|<span data-ttu-id="1fe9d-155">**说明**</span><span class="sxs-lookup"><span data-stu-id="1fe9d-155">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1fe9d-156">id</span><span class="sxs-lookup"><span data-stu-id="1fe9d-156">id</span></span>|<span data-ttu-id="1fe9d-157">string</span><span class="sxs-lookup"><span data-stu-id="1fe9d-157">string</span></span>|<span data-ttu-id="1fe9d-p103">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="1fe9d-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="1fe9d-160">extensionId</span></span>|<span data-ttu-id="1fe9d-161">string</span><span class="sxs-lookup"><span data-stu-id="1fe9d-161">string</span></span>|<span data-ttu-id="1fe9d-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1fe9d-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fe9d-165">Request headers</span></span>
| <span data-ttu-id="1fe9d-166">名称</span><span class="sxs-lookup"><span data-stu-id="1fe9d-166">Name</span></span>       | <span data-ttu-id="1fe9d-167">值</span><span class="sxs-lookup"><span data-stu-id="1fe9d-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1fe9d-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fe9d-168">Authorization</span></span> | <span data-ttu-id="1fe9d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fe9d-171">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fe9d-171">Request body</span></span>
<span data-ttu-id="1fe9d-172">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fe9d-173">响应</span><span class="sxs-lookup"><span data-stu-id="1fe9d-173">Response</span></span>

<span data-ttu-id="1fe9d-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe9d-176">示例</span><span class="sxs-lookup"><span data-stu-id="1fe9d-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fe9d-177">请求</span><span class="sxs-lookup"><span data-stu-id="1fe9d-177">Request</span></span>
<span data-ttu-id="1fe9d-178">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```

<span data-ttu-id="1fe9d-179">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="1fe9d-180">响应</span><span class="sxs-lookup"><span data-stu-id="1fe9d-180">Response</span></span>
<span data-ttu-id="1fe9d-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1fe9d-181">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
