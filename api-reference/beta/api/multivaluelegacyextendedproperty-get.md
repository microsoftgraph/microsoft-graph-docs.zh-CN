---
title: 获取 multiValueLegacyExtendedProperty
description: 展开。
localization_priority: Normal
ms.openlocfilehash: 7a649020bf326d4ec1ed3a83ae0c759a012378d4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641083"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="49134-103">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="49134-103">Get multiValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49134-104">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="49134-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="49134-105">使用查询参数 `$expand`，可以获取使用指明的扩展属性扩展的指定实例。</span><span class="sxs-lookup"><span data-stu-id="49134-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="49134-106">这是当前获取 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="49134-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="49134-107">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="49134-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="49134-108">日历</span><span class="sxs-lookup"><span data-stu-id="49134-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="49134-109">联系人</span><span class="sxs-lookup"><span data-stu-id="49134-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="49134-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="49134-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="49134-111">事件</span><span class="sxs-lookup"><span data-stu-id="49134-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="49134-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="49134-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="49134-113">message</span><span class="sxs-lookup"><span data-stu-id="49134-113">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="49134-114">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="49134-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="49134-115">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="49134-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="49134-116">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="49134-116">As well as the following group resources:</span></span>

- <span data-ttu-id="49134-117">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="49134-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="49134-118">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="49134-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="49134-119">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="49134-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="49134-120">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="49134-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="49134-121">权限</span><span class="sxs-lookup"><span data-stu-id="49134-121">Permissions</span></span>
<span data-ttu-id="49134-122">根据资源获得的扩展的属性和权限键入 （委派或应用程序） 您请求，若要调用此 API 至少是下表中所指定的权限。</span><span class="sxs-lookup"><span data-stu-id="49134-122">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="49134-123">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49134-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49134-124">支持的资源</span><span class="sxs-lookup"><span data-stu-id="49134-124">Supported resource</span></span> | <span data-ttu-id="49134-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49134-125">Delegated (work or school account)</span></span> | <span data-ttu-id="49134-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49134-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49134-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="49134-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="49134-128">calendar</span><span class="sxs-lookup"><span data-stu-id="49134-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="49134-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-129">Calendars.Read</span></span> | <span data-ttu-id="49134-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-130">Calendars.Read</span></span> | <span data-ttu-id="49134-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-131">Calendars.Read</span></span> |
| [<span data-ttu-id="49134-132">联系人</span><span class="sxs-lookup"><span data-stu-id="49134-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="49134-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-133">Contacts.Read</span></span> | <span data-ttu-id="49134-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-134">Contacts.Read</span></span> | <span data-ttu-id="49134-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-135">Contacts.Read</span></span> |
| [<span data-ttu-id="49134-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="49134-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="49134-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-137">Contacts.Read</span></span> | <span data-ttu-id="49134-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-138">Contacts.Read</span></span> | <span data-ttu-id="49134-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49134-139">Contacts.Read</span></span> |
| [<span data-ttu-id="49134-140">事件</span><span class="sxs-lookup"><span data-stu-id="49134-140">event</span></span>](../resources/event.md) | <span data-ttu-id="49134-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-141">Calendars.Read</span></span> | <span data-ttu-id="49134-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-142">Calendars.Read</span></span> |  <span data-ttu-id="49134-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49134-143">Calendars.Read</span></span>|
| <span data-ttu-id="49134-144">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="49134-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="49134-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49134-145">Group.Read.All</span></span> | <span data-ttu-id="49134-146">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-146">Not supported</span></span> | <span data-ttu-id="49134-147">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-147">Not supported</span></span> |
| <span data-ttu-id="49134-148">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="49134-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="49134-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49134-149">Group.Read.All</span></span> | <span data-ttu-id="49134-150">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-150">Not supported</span></span> | <span data-ttu-id="49134-151">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-151">Not supported</span></span> |
| <span data-ttu-id="49134-152">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="49134-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="49134-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49134-153">Group.Read.All</span></span> | <span data-ttu-id="49134-154">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-154">Not supported</span></span> | <span data-ttu-id="49134-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49134-155">Group.Read.All</span></span> |
| [<span data-ttu-id="49134-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="49134-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="49134-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-157">Mail.Read</span></span> | <span data-ttu-id="49134-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-158">Mail.Read</span></span> | <span data-ttu-id="49134-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-159">Mail.Read</span></span> |
| [<span data-ttu-id="49134-160">message</span><span class="sxs-lookup"><span data-stu-id="49134-160">message</span></span>](../resources/message.md) | <span data-ttu-id="49134-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-161">Mail.Read</span></span> | <span data-ttu-id="49134-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-162">Mail.Read</span></span> | <span data-ttu-id="49134-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49134-163">Mail.Read</span></span> |
| [<span data-ttu-id="49134-164">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="49134-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="49134-165">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49134-165">Tasks.Read</span></span> | <span data-ttu-id="49134-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49134-166">Tasks.Read</span></span> | <span data-ttu-id="49134-167">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-167">Not supported</span></span> |
| [<span data-ttu-id="49134-168">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="49134-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="49134-169">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49134-169">Tasks.Read</span></span> | <span data-ttu-id="49134-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49134-170">Tasks.Read</span></span> | <span data-ttu-id="49134-171">不支持</span><span class="sxs-lookup"><span data-stu-id="49134-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="49134-172">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49134-172">HTTP request</span></span>

<span data-ttu-id="49134-p103">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="49134-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="49134-175">获取**邮件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-175">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="49134-176">获取一个**mailFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-176">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="49134-177">获取**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-177">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="49134-178">获取**日历**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-178">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="49134-179">获取**联系人**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-179">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="49134-180">获取一个**contactFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-180">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="49134-181">获取**outlookTask**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-181">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="49134-182">获取**outlookTaskFolder**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-182">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="49134-183">获取组**事件**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-183">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="49134-184">获取一个组**发布**实例：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="49134-184">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="49134-185">路径参数</span><span class="sxs-lookup"><span data-stu-id="49134-185">Path parameters</span></span>
|<span data-ttu-id="49134-186">**参数**</span><span class="sxs-lookup"><span data-stu-id="49134-186">**Parameter**</span></span>|<span data-ttu-id="49134-187">**类型**</span><span class="sxs-lookup"><span data-stu-id="49134-187">**Type**</span></span>|<span data-ttu-id="49134-188">**说明**</span><span class="sxs-lookup"><span data-stu-id="49134-188">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="49134-189">id_value</span><span class="sxs-lookup"><span data-stu-id="49134-189">id_value</span></span>|<span data-ttu-id="49134-190">String</span><span class="sxs-lookup"><span data-stu-id="49134-190">String</span></span>|<span data-ttu-id="49134-p104">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="49134-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="49134-195">请求标头</span><span class="sxs-lookup"><span data-stu-id="49134-195">Request headers</span></span>
| <span data-ttu-id="49134-196">名称</span><span class="sxs-lookup"><span data-stu-id="49134-196">Name</span></span>      |<span data-ttu-id="49134-197">说明</span><span class="sxs-lookup"><span data-stu-id="49134-197">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49134-198">Authorization</span><span class="sxs-lookup"><span data-stu-id="49134-198">Authorization</span></span>  | <span data-ttu-id="49134-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49134-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49134-201">请求正文</span><span class="sxs-lookup"><span data-stu-id="49134-201">Request body</span></span>
<span data-ttu-id="49134-202">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49134-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49134-203">响应</span><span class="sxs-lookup"><span data-stu-id="49134-203">Response</span></span>

<span data-ttu-id="49134-204">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="49134-204">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="49134-205">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="49134-205">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="49134-206">示例</span><span class="sxs-lookup"><span data-stu-id="49134-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49134-207">请求</span><span class="sxs-lookup"><span data-stu-id="49134-207">Request</span></span>
<span data-ttu-id="49134-p106">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="49134-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="49134-210">响应</span><span class="sxs-lookup"><span data-stu-id="49134-210">Response</span></span>

<span data-ttu-id="49134-211">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="49134-211">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="49134-p107">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49134-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
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
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
