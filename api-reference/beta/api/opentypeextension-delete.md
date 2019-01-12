---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 617971d4e31e65a662415c75f4a6cdac330ebcb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983175"
---
# <a name="delete-open-extension"></a><span data-ttu-id="64950-103">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="64950-103">Delete open extension</span></span>

> <span data-ttu-id="64950-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="64950-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64950-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="64950-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64950-106">从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。</span><span class="sxs-lookup"><span data-stu-id="64950-106">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="64950-107">权限</span><span class="sxs-lookup"><span data-stu-id="64950-107">Permissions</span></span>

<span data-ttu-id="64950-108">根据您正在删除扩展名的资源和权限类型 （委派或应用程序） 请求下, 表中所指定的权限是最小特权需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="64950-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="64950-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64950-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64950-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="64950-110">Supported resource</span></span> | <span data-ttu-id="64950-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64950-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64950-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64950-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64950-113">用途</span><span class="sxs-lookup"><span data-stu-id="64950-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="64950-114">设备</span><span class="sxs-lookup"><span data-stu-id="64950-114">device</span></span>](../resources/device.md) | <span data-ttu-id="64950-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64950-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="64950-116">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-116">Not supported</span></span> | <span data-ttu-id="64950-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="64950-118">事件</span><span class="sxs-lookup"><span data-stu-id="64950-118">event</span></span>](../resources/event.md) | <span data-ttu-id="64950-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="64950-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="64950-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="64950-122">组</span><span class="sxs-lookup"><span data-stu-id="64950-122">group</span></span>](../resources/group.md) | <span data-ttu-id="64950-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="64950-124">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-124">Not supported</span></span> | <span data-ttu-id="64950-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="64950-126">组事件</span><span class="sxs-lookup"><span data-stu-id="64950-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="64950-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="64950-128">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-128">Not supported</span></span> | <span data-ttu-id="64950-129">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-129">Not supported</span></span> |
| [<span data-ttu-id="64950-130">组帖子</span><span class="sxs-lookup"><span data-stu-id="64950-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="64950-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="64950-132">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-132">Not supported</span></span> | <span data-ttu-id="64950-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="64950-134">邮件</span><span class="sxs-lookup"><span data-stu-id="64950-134">message</span></span>](../resources/message.md) | <span data-ttu-id="64950-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-135">Mail.ReadWrite</span></span> | <span data-ttu-id="64950-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-136">Mail.ReadWrite</span></span> | <span data-ttu-id="64950-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="64950-138">组织</span><span class="sxs-lookup"><span data-stu-id="64950-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="64950-139">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64950-139">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="64950-140">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-140">Not supported</span></span> | <span data-ttu-id="64950-141">不支持</span><span class="sxs-lookup"><span data-stu-id="64950-141">Not supported</span></span> |
| [<span data-ttu-id="64950-142">个人联系人</span><span class="sxs-lookup"><span data-stu-id="64950-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="64950-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="64950-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="64950-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="64950-146">用户</span><span class="sxs-lookup"><span data-stu-id="64950-146">user</span></span>](../resources/user.md) | <span data-ttu-id="64950-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-147">User.ReadWrite.All</span></span> | <span data-ttu-id="64950-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64950-148">User.ReadWrite</span></span> | <span data-ttu-id="64950-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64950-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64950-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64950-150">HTTP request</span></span>

<span data-ttu-id="64950-151">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。</span><span class="sxs-lookup"><span data-stu-id="64950-151">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="64950-p103">**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。</span><span class="sxs-lookup"><span data-stu-id="64950-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="64950-154">路径参数</span><span class="sxs-lookup"><span data-stu-id="64950-154">Path parameters</span></span>
|<span data-ttu-id="64950-155">**参数**</span><span class="sxs-lookup"><span data-stu-id="64950-155">**Parameter**</span></span>|<span data-ttu-id="64950-156">**类型**</span><span class="sxs-lookup"><span data-stu-id="64950-156">**Type**</span></span>|<span data-ttu-id="64950-157">**说明**</span><span class="sxs-lookup"><span data-stu-id="64950-157">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="64950-158">id</span><span class="sxs-lookup"><span data-stu-id="64950-158">id</span></span>|<span data-ttu-id="64950-159">string</span><span class="sxs-lookup"><span data-stu-id="64950-159">string</span></span>|<span data-ttu-id="64950-p104">实例在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="64950-p104">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="64950-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="64950-162">extensionId</span></span>|<span data-ttu-id="64950-163">string</span><span class="sxs-lookup"><span data-stu-id="64950-163">string</span></span>|<span data-ttu-id="64950-p105">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="64950-p105">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="64950-167">请求标头</span><span class="sxs-lookup"><span data-stu-id="64950-167">Request headers</span></span>
| <span data-ttu-id="64950-168">名称</span><span class="sxs-lookup"><span data-stu-id="64950-168">Name</span></span>       | <span data-ttu-id="64950-169">值</span><span class="sxs-lookup"><span data-stu-id="64950-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="64950-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="64950-170">Authorization</span></span> | <span data-ttu-id="64950-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64950-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64950-173">请求正文</span><span class="sxs-lookup"><span data-stu-id="64950-173">Request body</span></span>
<span data-ttu-id="64950-174">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64950-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64950-175">响应</span><span class="sxs-lookup"><span data-stu-id="64950-175">Response</span></span>

<span data-ttu-id="64950-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="64950-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64950-178">示例</span><span class="sxs-lookup"><span data-stu-id="64950-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64950-179">请求</span><span class="sxs-lookup"><span data-stu-id="64950-179">Request</span></span>
<span data-ttu-id="64950-180">第一个示例按其名称引用扩展并删除指定邮件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="64950-180">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="64950-181">第二个示例删除指定组事件中的扩展。</span><span class="sxs-lookup"><span data-stu-id="64950-181">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="64950-182">响应</span><span class="sxs-lookup"><span data-stu-id="64950-182">Response</span></span>
<span data-ttu-id="64950-183">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="64950-183">Here is an example of the response.</span></span>
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
