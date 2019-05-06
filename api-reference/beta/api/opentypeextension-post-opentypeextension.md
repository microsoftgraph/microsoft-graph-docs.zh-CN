---
title: 创建开放扩展
description: 创建开放扩展 (openTypeExtension 对象) 并添加自定义属性
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 104f29d9026d385403d272d71fc5acf77ad6fd3d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597075"
---
# <a name="create-open-extension"></a><span data-ttu-id="e9ee0-103">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="e9ee0-103">Create open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9ee0-104">创建开放扩展 ([openTypeExtension](../resources/opentypeextension.md)对象), 并在新的或现有的受支持的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-104">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="e9ee0-105">**请注意：** 如果要在 Outlook 资源上创建开放扩展，请参阅 [openTypeExtension 资源类型](../resources/opentypeextension.md#outlook-specific-considerations)中的 **Outlook 特定注意事项**。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-105">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9ee0-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9ee0-106">Permissions</span></span>

<span data-ttu-id="e9ee0-107">根据要在其中创建扩展的资源和所请求的权限类型（委派或应用程序），下表中指定的权限是指调用此 API 所需的最低限度的特权。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-107">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e9ee0-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9ee0-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="e9ee0-109">Supported resource</span></span> | <span data-ttu-id="e9ee0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9ee0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9ee0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9ee0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9ee0-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9ee0-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e9ee0-113">设备</span><span class="sxs-lookup"><span data-stu-id="e9ee0-113">device</span></span>](../resources/device.md) | <span data-ttu-id="e9ee0-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e9ee0-115">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-115">Not supported</span></span> | <span data-ttu-id="e9ee0-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="e9ee0-117">事件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-117">event</span></span>](../resources/event.md) | <span data-ttu-id="e9ee0-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="e9ee0-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="e9ee0-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e9ee0-121">组</span><span class="sxs-lookup"><span data-stu-id="e9ee0-121">group</span></span>](../resources/group.md) | <span data-ttu-id="e9ee0-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="e9ee0-123">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-123">Not supported</span></span> | <span data-ttu-id="e9ee0-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e9ee0-125">组事件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="e9ee0-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="e9ee0-127">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-127">Not supported</span></span> | <span data-ttu-id="e9ee0-128">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-128">Not supported</span></span> |
| [<span data-ttu-id="e9ee0-129">组帖子</span><span class="sxs-lookup"><span data-stu-id="e9ee0-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="e9ee0-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="e9ee0-131">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-131">Not supported</span></span> | <span data-ttu-id="e9ee0-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e9ee0-133">邮件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-133">message</span></span>](../resources/message.md) | <span data-ttu-id="e9ee0-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-134">Mail.ReadWrite</span></span> | <span data-ttu-id="e9ee0-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-135">Mail.ReadWrite</span></span> | <span data-ttu-id="e9ee0-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="e9ee0-137">组织</span><span class="sxs-lookup"><span data-stu-id="e9ee0-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="e9ee0-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e9ee0-139">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-139">Not supported</span></span> | <span data-ttu-id="e9ee0-140">不支持</span><span class="sxs-lookup"><span data-stu-id="e9ee0-140">Not supported</span></span> |
| [<span data-ttu-id="e9ee0-141">个人联系人</span><span class="sxs-lookup"><span data-stu-id="e9ee0-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="e9ee0-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="e9ee0-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="e9ee0-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e9ee0-145">用户</span><span class="sxs-lookup"><span data-stu-id="e9ee0-145">user</span></span>](../resources/user.md) | <span data-ttu-id="e9ee0-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-146">User.ReadWrite.All</span></span> | <span data-ttu-id="e9ee0-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9ee0-147">User.ReadWrite</span></span> | <span data-ttu-id="e9ee0-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ee0-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9ee0-149">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9ee0-149">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="e9ee0-150">在新资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-150">Create an extension in a new resource instance</span></span>

<span data-ttu-id="e9ee0-151">使用创建实例时所用的同一 REST 请求。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-151">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="e9ee0-152">**请注意：** 此语法显示了一些创建受支持资源实例的常用方式。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-152">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="e9ee0-153">可用来创建这些资源实例的所有其他 POST 语法均支持以类似的方式从中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-153">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e9ee0-154">若要了解如何在请求正文中添加新资源实例和_扩展_的属性，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-154">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="e9ee0-155">在现有资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-155">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="e9ee0-156">在请求中标识资源实例，然后对 **extensions** 导航属性执行 `POST`。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-156">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="e9ee0-157">**请注意：** 以上语法显示一些标识资源实例的常见方法，以便在其中创建一个扩展。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-157">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="e9ee0-158">可用来标识这些资源实例的所有其他语法均支持以类似的方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-158">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e9ee0-159">若要了解如何在请求正文中添加_扩展_，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-159">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="e9ee0-160">路径参数</span><span class="sxs-lookup"><span data-stu-id="e9ee0-160">Path parameters</span></span>

|<span data-ttu-id="e9ee0-161">**参数**</span><span class="sxs-lookup"><span data-stu-id="e9ee0-161">**Parameter**</span></span>|<span data-ttu-id="e9ee0-162">**类型**</span><span class="sxs-lookup"><span data-stu-id="e9ee0-162">**Type**</span></span>|<span data-ttu-id="e9ee0-163">**说明**</span><span class="sxs-lookup"><span data-stu-id="e9ee0-163">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e9ee0-164">id</span><span class="sxs-lookup"><span data-stu-id="e9ee0-164">id</span></span>|<span data-ttu-id="e9ee0-165">string</span><span class="sxs-lookup"><span data-stu-id="e9ee0-165">string</span></span>|<span data-ttu-id="e9ee0-p104">对象在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e9ee0-168">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9ee0-168">Request headers</span></span>

| <span data-ttu-id="e9ee0-169">名称</span><span class="sxs-lookup"><span data-stu-id="e9ee0-169">Name</span></span>       | <span data-ttu-id="e9ee0-170">值</span><span class="sxs-lookup"><span data-stu-id="e9ee0-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e9ee0-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9ee0-171">Authorization</span></span> | <span data-ttu-id="e9ee0-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9ee0-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9ee0-174">Content-Type</span></span> | <span data-ttu-id="e9ee0-175">application/json</span><span class="sxs-lookup"><span data-stu-id="e9ee0-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9ee0-176">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9ee0-176">Request body</span></span>

<span data-ttu-id="e9ee0-p106">提供具有以下必需的名称-值对和任何其他自定义数据的[openTypeExtension](../resources/opentypeextension.md)的 JSON 正文。JSON 有效负载中的数据可以是基元类型, 也可以是基元类型的数组。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="e9ee0-179">名称</span><span class="sxs-lookup"><span data-stu-id="e9ee0-179">Name</span></span>       | <span data-ttu-id="e9ee0-180">值</span><span class="sxs-lookup"><span data-stu-id="e9ee0-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e9ee0-181">@odata.type</span><span class="sxs-lookup"><span data-stu-id="e9ee0-181">@odata.type</span></span> | <span data-ttu-id="e9ee0-182">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e9ee0-182">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="e9ee0-183">extensionName</span><span class="sxs-lookup"><span data-stu-id="e9ee0-183">extensionName</span></span> | <span data-ttu-id="e9ee0-184">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="e9ee0-184">%unique_string%</span></span> |

<span data-ttu-id="e9ee0-185">在_新_资源实例中创建扩展插件时，除了新的 **openTypeExtension** 对象之外，还要提供 JSON 表示形式的相关属性才能创建此类资源实例。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-185">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="e9ee0-186">响应</span><span class="sxs-lookup"><span data-stu-id="e9ee0-186">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="e9ee0-187">响应代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-187">Response code</span></span>

<span data-ttu-id="e9ee0-188">响应代码可以是 `201 Created`，也可以是 `202 Accepted`，具体视操作而定。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-188">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="e9ee0-189">使用创建资源实例时所用的操作创建扩展时，操作所返回的响应代码与通过该操作创建不带扩展的资源实例时返回的代码相同。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-189">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="e9ee0-190">请参阅有关创建实例的相应主题，如[上 ](#create-an-extension-in-a-new-resource-instance)所列。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-190">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="e9ee0-191">响应正文</span><span class="sxs-lookup"><span data-stu-id="e9ee0-191">Response body</span></span>

| <span data-ttu-id="e9ee0-192">应用场景</span><span class="sxs-lookup"><span data-stu-id="e9ee0-192">Scenario</span></span>       | <span data-ttu-id="e9ee0-193">资源</span><span class="sxs-lookup"><span data-stu-id="e9ee0-193">Resource</span></span>  | <span data-ttu-id="e9ee0-194">响应正文</span><span class="sxs-lookup"><span data-stu-id="e9ee0-194">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="e9ee0-195">在显式创建_新_资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-195">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="e9ee0-196">[联系人](../resources/contact.md)、[事件](../resources/event.md)、[邮件](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="e9ee0-196">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="e9ee0-197">包括使用 [openTypeExtension](../resources/opentypeextension.md) 对象扩展的新实例。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-197">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="e9ee0-198">在隐式创建资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-198">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="e9ee0-199">帖子</span><span class="sxs-lookup"><span data-stu-id="e9ee0-199">post</span></span>](../resources/post.md) | <span data-ttu-id="e9ee0-200">响应只包括响应代码，不包括响应正文。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-200">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="e9ee0-201">在_现有_资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e9ee0-201">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="e9ee0-202">所有支持的资源</span><span class="sxs-lookup"><span data-stu-id="e9ee0-202">All supported resources</span></span> | <span data-ttu-id="e9ee0-203">包括 **openTypeExtension** 对象。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-203">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="e9ee0-204">示例</span><span class="sxs-lookup"><span data-stu-id="e9ee0-204">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="e9ee0-205">请求 1</span><span class="sxs-lookup"><span data-stu-id="e9ee0-205">Request 1</span></span>

<span data-ttu-id="e9ee0-p108">第一个示例在同一个调用中创建一个邮件和一个扩展。请求正文包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="e9ee0-208">新邮件的典型 **subject**、**body** 和 **toRecipients** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-208">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="e9ee0-209">对于扩展：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-209">And for the extension:</span></span>

  - <span data-ttu-id="e9ee0-210">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-210">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="e9ee0-211">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-211">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="e9ee0-212">存储为 JSON 有效负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `dealValue`。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-212">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-Type: application/json

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="e9ee0-213">响应 1</span><span class="sxs-lookup"><span data-stu-id="e9ee0-213">Response 1</span></span>

<span data-ttu-id="e9ee0-p109">下面是第一个示例的响应。响应正文包括新邮件的属性以及新扩展的以下属性：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="e9ee0-216">具有完全限定的名称 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-216">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e9ee0-217">请求中指定的默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-217">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="e9ee0-218">请求中指定的作为 3 个自定义属性存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-218">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="e9ee0-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
      "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ee0-221">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-221">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ee0-222">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9ee0-222">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_opentypeextension_1-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

****

### <a name="request-2"></a><span data-ttu-id="e9ee0-223">请求 2</span><span class="sxs-lookup"><span data-stu-id="e9ee0-223">Request 2</span></span>

<span data-ttu-id="e9ee0-p111">第二个示例在指定邮件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e9ee0-226">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-226">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e9ee0-227">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-227">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="e9ee0-228">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-228">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions
Content-Type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="e9ee0-229">响应 2</span><span class="sxs-lookup"><span data-stu-id="e9ee0-229">Response 2</span></span>

<span data-ttu-id="e9ee0-p112">下面是第二个示例的响应。请求正文包括新扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="e9ee0-232">默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-232">The default property **extensionName**.</span></span>
- <span data-ttu-id="e9ee0-233">具有完全限定的名称 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-233">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e9ee0-234">要存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-234">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ee0-235">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-235">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ee0-236">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9ee0-236">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_opentypeextension_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

****

### <a name="request-3"></a><span data-ttu-id="e9ee0-237">请求 3</span><span class="sxs-lookup"><span data-stu-id="e9ee0-237">Request 3</span></span>

<span data-ttu-id="e9ee0-p113">第三个示例在指定组事件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e9ee0-240">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-240">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e9ee0-241">扩展名“Com.Contoso.Deal”。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-241">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="e9ee0-242">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-242">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions
Content-type: application/json

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="e9ee0-243">响应 3</span><span class="sxs-lookup"><span data-stu-id="e9ee0-243">Response 3</span></span>

<span data-ttu-id="e9ee0-244">下面是第三个示例请求的响应。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-244">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ee0-245">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-245">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ee0-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9ee0-246">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_opentypeextension_3-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

****

### <a name="request-4"></a><span data-ttu-id="e9ee0-247">请求 4</span><span class="sxs-lookup"><span data-stu-id="e9ee0-247">Request 4</span></span>

<span data-ttu-id="e9ee0-p114">第四个示例对现有的组帖子使用相同的 **reply** 操作调用，在新的组帖子中创建扩展。**reply** 操作创建新帖子和嵌入帖子中的新扩展。请求正文包括 **post** 属性，此属性又包含新帖子的 **body** 以及新扩展的以下数据：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="e9ee0-251">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-251">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e9ee0-252">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-252">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e9ee0-253">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-253">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply
Content-type: application/json

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a><span data-ttu-id="e9ee0-254">响应 4</span><span class="sxs-lookup"><span data-stu-id="e9ee0-254">Response 4</span></span>

<span data-ttu-id="e9ee0-p115">下面是第四个示例的响应。新的组帖子中成功创建扩展仅会产生 HTTP 202 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ee0-257">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-257">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ee0-258">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9ee0-258">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_opentypeextension_4-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

****

### <a name="request-5"></a><span data-ttu-id="e9ee0-259">响应 5</span><span class="sxs-lookup"><span data-stu-id="e9ee0-259">Request 5</span></span>

<span data-ttu-id="e9ee0-p116">第五个示例使用 POST 操作创建对话，在新的组帖子中创建扩展。POST 操作创建新对话、线程和帖子以及嵌入帖子中的新扩展。请求正文包括 **Topic** 和 **Threads** 属性以及新对话的子 **post** 对象。**post** 对象又包含新帖子的 **body** 和以下扩展数据：</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="e9ee0-264">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-264">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e9ee0-265">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-265">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e9ee0-266">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-266">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations
Content-type: application/json

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "microsoft.graph.openTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a><span data-ttu-id="e9ee0-267">响应 5</span><span class="sxs-lookup"><span data-stu-id="e9ee0-267">Response 5</span></span>

<span data-ttu-id="e9ee0-p117">下面是第五个示例的响应，其中包含新对话和线程 ID。这个新线程包含自动创建的帖子，帖子又包含新扩展。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="e9ee0-p118">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="e9ee0-p119">若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread-list-posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension-get.md)。</span><span class="sxs-lookup"><span data-stu-id="e9ee0-p119">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9ee0-274">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e9ee0-274">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ee0-275">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9ee0-275">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_opentypeextension_5-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
