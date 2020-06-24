---
title: 创建开放扩展
description: 创建开放扩展（openTypeExtension 对象）并添加自定义属性
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: d6c06370494e9e89fa77d40a0889819f47f21d2c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863367"
---
# <a name="create-open-extension"></a><span data-ttu-id="e6677-103">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="e6677-103">Create open extension</span></span>

<span data-ttu-id="e6677-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6677-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6677-105">创建开放扩展（[openTypeExtension](../resources/opentypeextension.md)对象），并在新的或现有的受支持的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e6677-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="e6677-106">**请注意：** 如果要在 Outlook 资源上创建开放扩展，请参阅 [openTypeExtension 资源类型](../resources/opentypeextension.md#outlook-specific-considerations)中的 **Outlook 特定注意事项**。</span><span class="sxs-lookup"><span data-stu-id="e6677-106">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6677-107">权限</span><span class="sxs-lookup"><span data-stu-id="e6677-107">Permissions</span></span>

<span data-ttu-id="e6677-108">根据要在其中创建扩展的资源和所请求的权限类型（委派或应用程序），下表中指定的权限是指调用此 API 所需的最低限度的特权。</span><span class="sxs-lookup"><span data-stu-id="e6677-108">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e6677-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6677-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6677-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="e6677-110">Supported resource</span></span> | <span data-ttu-id="e6677-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6677-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e6677-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6677-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6677-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6677-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e6677-114">设备</span><span class="sxs-lookup"><span data-stu-id="e6677-114">device</span></span>](../resources/device.md) | <span data-ttu-id="e6677-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6677-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e6677-116">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-116">Not supported</span></span> | <span data-ttu-id="e6677-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="e6677-118">事件</span><span class="sxs-lookup"><span data-stu-id="e6677-118">event</span></span>](../resources/event.md) | <span data-ttu-id="e6677-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="e6677-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="e6677-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e6677-122">组</span><span class="sxs-lookup"><span data-stu-id="e6677-122">group</span></span>](../resources/group.md) | <span data-ttu-id="e6677-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="e6677-124">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-124">Not supported</span></span> | <span data-ttu-id="e6677-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e6677-126">组事件</span><span class="sxs-lookup"><span data-stu-id="e6677-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="e6677-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="e6677-128">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-128">Not supported</span></span> | <span data-ttu-id="e6677-129">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-129">Not supported</span></span> |
| [<span data-ttu-id="e6677-130">组帖子</span><span class="sxs-lookup"><span data-stu-id="e6677-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="e6677-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="e6677-132">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-132">Not supported</span></span> | <span data-ttu-id="e6677-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e6677-134">邮件</span><span class="sxs-lookup"><span data-stu-id="e6677-134">message</span></span>](../resources/message.md) | <span data-ttu-id="e6677-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-135">Mail.ReadWrite</span></span> | <span data-ttu-id="e6677-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-136">Mail.ReadWrite</span></span> | <span data-ttu-id="e6677-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="e6677-138">组织</span><span class="sxs-lookup"><span data-stu-id="e6677-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="e6677-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="e6677-140">不支持</span><span class="sxs-lookup"><span data-stu-id="e6677-140">Not supported</span></span> | <span data-ttu-id="e6677-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-141">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="e6677-142">个人联系人</span><span class="sxs-lookup"><span data-stu-id="e6677-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="e6677-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="e6677-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="e6677-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e6677-146">用户</span><span class="sxs-lookup"><span data-stu-id="e6677-146">user</span></span>](../resources/user.md) | <span data-ttu-id="e6677-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-147">User.ReadWrite</span></span> | <span data-ttu-id="e6677-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6677-148">User.ReadWrite</span></span> | <span data-ttu-id="e6677-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6677-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6677-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6677-150">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="e6677-151">在新资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e6677-151">Create an extension in a new resource instance</span></span>

<span data-ttu-id="e6677-152">使用创建实例时所用的同一 REST 请求。</span><span class="sxs-lookup"><span data-stu-id="e6677-152">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="e6677-153">**请注意：** 此语法显示了一些创建受支持资源实例的常用方式。</span><span class="sxs-lookup"><span data-stu-id="e6677-153">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="e6677-154">可用来创建这些资源实例的所有其他 POST 语法均支持以类似的方式从中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e6677-154">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e6677-155">若要了解如何在请求正文中添加新资源实例和_扩展_的属性，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="e6677-155">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="e6677-156">在现有资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e6677-156">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="e6677-157">在请求中标识资源实例，然后对 **extensions** 导航属性执行 `POST`。</span><span class="sxs-lookup"><span data-stu-id="e6677-157">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="e6677-158">**请注意：** 以上语法显示一些标识资源实例的常见方法，以便在其中创建一个扩展。</span><span class="sxs-lookup"><span data-stu-id="e6677-158">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="e6677-159">可用来标识这些资源实例的所有其他语法均支持以类似的方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e6677-159">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="e6677-160">若要了解如何在请求正文中添加_扩展_，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="e6677-160">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="e6677-161">路径参数</span><span class="sxs-lookup"><span data-stu-id="e6677-161">Path parameters</span></span>

|<span data-ttu-id="e6677-162">**参数**</span><span class="sxs-lookup"><span data-stu-id="e6677-162">**Parameter**</span></span>|<span data-ttu-id="e6677-163">**类型**</span><span class="sxs-lookup"><span data-stu-id="e6677-163">**Type**</span></span>|<span data-ttu-id="e6677-164">**说明**</span><span class="sxs-lookup"><span data-stu-id="e6677-164">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e6677-165">id</span><span class="sxs-lookup"><span data-stu-id="e6677-165">id</span></span>|<span data-ttu-id="e6677-166">string</span><span class="sxs-lookup"><span data-stu-id="e6677-166">string</span></span>|<span data-ttu-id="e6677-167">A unique identifier for an object in the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="e6677-167">A unique identifier for an object in the corresponding collection.</span></span> <span data-ttu-id="e6677-168">Required.</span><span class="sxs-lookup"><span data-stu-id="e6677-168">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e6677-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6677-169">Request headers</span></span>

| <span data-ttu-id="e6677-170">名称</span><span class="sxs-lookup"><span data-stu-id="e6677-170">Name</span></span>       | <span data-ttu-id="e6677-171">值</span><span class="sxs-lookup"><span data-stu-id="e6677-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e6677-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6677-172">Authorization</span></span> | <span data-ttu-id="e6677-173">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e6677-173">Bearer {token}.</span></span> <span data-ttu-id="e6677-174">Required.</span><span class="sxs-lookup"><span data-stu-id="e6677-174">Required.</span></span> |
| <span data-ttu-id="e6677-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6677-175">Content-Type</span></span> | <span data-ttu-id="e6677-176">application/json</span><span class="sxs-lookup"><span data-stu-id="e6677-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6677-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6677-177">Request body</span></span>

<span data-ttu-id="e6677-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span><span class="sxs-lookup"><span data-stu-id="e6677-178">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="e6677-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span><span class="sxs-lookup"><span data-stu-id="e6677-179">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="e6677-180">名称</span><span class="sxs-lookup"><span data-stu-id="e6677-180">Name</span></span>       | <span data-ttu-id="e6677-181">值</span><span class="sxs-lookup"><span data-stu-id="e6677-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e6677-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="e6677-182">@odata.type</span></span> | <span data-ttu-id="e6677-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e6677-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="e6677-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="e6677-184">extensionName</span></span> | <span data-ttu-id="e6677-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="e6677-185">%unique_string%</span></span> |

<span data-ttu-id="e6677-186">在_新_资源实例中创建扩展插件时，除了新的 **openTypeExtension** 对象之外，还要提供 JSON 表示形式的相关属性才能创建此类资源实例。</span><span class="sxs-lookup"><span data-stu-id="e6677-186">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="e6677-187">响应</span><span class="sxs-lookup"><span data-stu-id="e6677-187">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="e6677-188">响应代码</span><span class="sxs-lookup"><span data-stu-id="e6677-188">Response code</span></span>

<span data-ttu-id="e6677-189">响应代码可以是 `201 Created`，也可以是 `202 Accepted`，具体视操作而定。</span><span class="sxs-lookup"><span data-stu-id="e6677-189">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="e6677-190">使用创建资源实例时所用的操作创建扩展时，操作所返回的响应代码与通过该操作创建不带扩展的资源实例时返回的代码相同。</span><span class="sxs-lookup"><span data-stu-id="e6677-190">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="e6677-191">请参阅有关创建实例的相应主题，如[上 ](#create-an-extension-in-a-new-resource-instance)所列。</span><span class="sxs-lookup"><span data-stu-id="e6677-191">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="e6677-192">响应正文</span><span class="sxs-lookup"><span data-stu-id="e6677-192">Response body</span></span>

| <span data-ttu-id="e6677-193">应用场景</span><span class="sxs-lookup"><span data-stu-id="e6677-193">Scenario</span></span>       | <span data-ttu-id="e6677-194">资源</span><span class="sxs-lookup"><span data-stu-id="e6677-194">Resource</span></span>  | <span data-ttu-id="e6677-195">响应正文</span><span class="sxs-lookup"><span data-stu-id="e6677-195">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="e6677-196">在显式创建_新_资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e6677-196">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="e6677-197">[联系人](../resources/contact.md)、[事件](../resources/event.md)、[邮件](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="e6677-197">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="e6677-198">包括使用 [openTypeExtension](../resources/opentypeextension.md) 对象扩展的新实例。</span><span class="sxs-lookup"><span data-stu-id="e6677-198">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="e6677-199">在隐式创建资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e6677-199">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="e6677-200">帖子</span><span class="sxs-lookup"><span data-stu-id="e6677-200">post</span></span>](../resources/post.md) | <span data-ttu-id="e6677-201">响应只包括响应代码，不包括响应正文。</span><span class="sxs-lookup"><span data-stu-id="e6677-201">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="e6677-202">在_现有_资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="e6677-202">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="e6677-203">所有支持的资源</span><span class="sxs-lookup"><span data-stu-id="e6677-203">All supported resources</span></span> | <span data-ttu-id="e6677-204">包括 **openTypeExtension** 对象。</span><span class="sxs-lookup"><span data-stu-id="e6677-204">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="e6677-205">示例</span><span class="sxs-lookup"><span data-stu-id="e6677-205">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="e6677-206">请求 1</span><span class="sxs-lookup"><span data-stu-id="e6677-206">Request 1</span></span>

<span data-ttu-id="e6677-207">The first example creates a message and an extension in the same call.</span><span class="sxs-lookup"><span data-stu-id="e6677-207">The first example creates a message and an extension in the same call.</span></span> <span data-ttu-id="e6677-208">The request body includes the following:</span><span class="sxs-lookup"><span data-stu-id="e6677-208">The request body includes the following:</span></span>

- <span data-ttu-id="e6677-209">新邮件的典型 **subject**、**body** 和 **toRecipients** 属性。</span><span class="sxs-lookup"><span data-stu-id="e6677-209">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="e6677-210">对于扩展：</span><span class="sxs-lookup"><span data-stu-id="e6677-210">And for the extension:</span></span>

  - <span data-ttu-id="e6677-211">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e6677-211">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="e6677-212">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="e6677-212">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="e6677-213">存储为 JSON 有效负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `dealValue`。</span><span class="sxs-lookup"><span data-stu-id="e6677-213">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6677-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6677-214">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6677-215">C#</span><span class="sxs-lookup"><span data-stu-id="e6677-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6677-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6677-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6677-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6677-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="e6677-218">响应 1</span><span class="sxs-lookup"><span data-stu-id="e6677-218">Response 1</span></span>

<span data-ttu-id="e6677-219">Here is the response for the first example.</span><span class="sxs-lookup"><span data-stu-id="e6677-219">Here is the response for the first example.</span></span> <span data-ttu-id="e6677-220">The response body includes properties of the new message, and the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-220">The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="e6677-221">具有完全限定的名称 \*\*\*\* 的 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 属性。</span><span class="sxs-lookup"><span data-stu-id="e6677-221">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e6677-222">请求中指定的默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="e6677-222">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="e6677-223">请求中指定的作为 3 个自定义属性存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="e6677-223">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="e6677-224">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e6677-224">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e6677-225">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e6677-225">All of the properties will be returned from an actual call.</span></span>

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

****

### <a name="request-2"></a><span data-ttu-id="e6677-226">请求 2</span><span class="sxs-lookup"><span data-stu-id="e6677-226">Request 2</span></span>

<span data-ttu-id="e6677-227">The second example creates an extension in the specified message.</span><span class="sxs-lookup"><span data-stu-id="e6677-227">The second example creates an extension in the specified message.</span></span> <span data-ttu-id="e6677-228">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-228">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e6677-229">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e6677-229">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e6677-230">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="e6677-230">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="e6677-231">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="e6677-231">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6677-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6677-232">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6677-233">C#</span><span class="sxs-lookup"><span data-stu-id="e6677-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6677-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6677-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6677-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6677-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="e6677-236">响应 2</span><span class="sxs-lookup"><span data-stu-id="e6677-236">Response 2</span></span>

<span data-ttu-id="e6677-237">Here is the response for the second example.</span><span class="sxs-lookup"><span data-stu-id="e6677-237">Here is the response for the second example.</span></span> <span data-ttu-id="e6677-238">The response body includes the following for the new extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-238">The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="e6677-239">默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="e6677-239">The default property **extensionName**.</span></span>
- <span data-ttu-id="e6677-240">具有完全限定的名称 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="e6677-240">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="e6677-241">要存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="e6677-241">The custom data to be stored.</span></span>

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

****

### <a name="request-3"></a><span data-ttu-id="e6677-242">请求 3</span><span class="sxs-lookup"><span data-stu-id="e6677-242">Request 3</span></span>

<span data-ttu-id="e6677-243">The third example creates an extension in the specified group event.</span><span class="sxs-lookup"><span data-stu-id="e6677-243">The third example creates an extension in the specified group event.</span></span> <span data-ttu-id="e6677-244">The request body includes the following for the extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-244">The request body includes the following for the extension:</span></span>

- <span data-ttu-id="e6677-245">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e6677-245">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e6677-246">扩展名“Com.Contoso.Deal”。</span><span class="sxs-lookup"><span data-stu-id="e6677-246">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="e6677-247">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="e6677-247">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6677-248">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6677-248">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6677-249">C#</span><span class="sxs-lookup"><span data-stu-id="e6677-249">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6677-250">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6677-250">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6677-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6677-251">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="e6677-252">响应 3</span><span class="sxs-lookup"><span data-stu-id="e6677-252">Response 3</span></span>

<span data-ttu-id="e6677-253">下面是第三个示例请求的响应。</span><span class="sxs-lookup"><span data-stu-id="e6677-253">Here is the response from the third example request.</span></span>

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

****

### <a name="request-4"></a><span data-ttu-id="e6677-254">请求 4</span><span class="sxs-lookup"><span data-stu-id="e6677-254">Request 4</span></span>

<span data-ttu-id="e6677-255">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span><span class="sxs-lookup"><span data-stu-id="e6677-255">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post.</span></span> <span data-ttu-id="e6677-256">The **reply** action creates a new post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="e6677-256">The **reply** action creates a new post, and a new extension embedded in the post.</span></span> <span data-ttu-id="e6677-257">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-257">The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="e6677-258">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e6677-258">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e6677-259">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="e6677-259">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e6677-260">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="e6677-260">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6677-261">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6677-261">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6677-262">C#</span><span class="sxs-lookup"><span data-stu-id="e6677-262">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6677-263">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6677-263">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6677-264">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6677-264">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="e6677-265">响应 4</span><span class="sxs-lookup"><span data-stu-id="e6677-265">Response 4</span></span>

<span data-ttu-id="e6677-266">Here is the response from the fourth example.</span><span class="sxs-lookup"><span data-stu-id="e6677-266">Here is the response from the fourth example.</span></span> <span data-ttu-id="e6677-267">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span><span class="sxs-lookup"><span data-stu-id="e6677-267">Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="e6677-268">响应 5</span><span class="sxs-lookup"><span data-stu-id="e6677-268">Request 5</span></span>

<span data-ttu-id="e6677-269">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span><span class="sxs-lookup"><span data-stu-id="e6677-269">The fifth example creates an extension in a new group post using the same POST operation to create a conversation.</span></span> <span data-ttu-id="e6677-270">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span><span class="sxs-lookup"><span data-stu-id="e6677-270">The POST operation creates a new conversation, thread and post, and a new extension embedded in the post.</span></span> <span data-ttu-id="e6677-271">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span><span class="sxs-lookup"><span data-stu-id="e6677-271">The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation.</span></span> <span data-ttu-id="e6677-272">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span><span class="sxs-lookup"><span data-stu-id="e6677-272">The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="e6677-273">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="e6677-273">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="e6677-274">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="e6677-274">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="e6677-275">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="e6677-275">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6677-276">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6677-276">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6677-277">C#</span><span class="sxs-lookup"><span data-stu-id="e6677-277">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6677-278">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6677-278">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6677-279">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6677-279">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="e6677-280">响应 5</span><span class="sxs-lookup"><span data-stu-id="e6677-280">Response 5</span></span>

<span data-ttu-id="e6677-281">Here is the response from the fifth example which contains the new conversation and a thread ID.</span><span class="sxs-lookup"><span data-stu-id="e6677-281">Here is the response from the fifth example which contains the new conversation and a thread ID.</span></span> <span data-ttu-id="e6677-282">This new thread contains an automatically created post, which in turn contains the new extension.</span><span class="sxs-lookup"><span data-stu-id="e6677-282">This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="e6677-283">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e6677-283">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e6677-284">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e6677-284">All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="e6677-285">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span><span class="sxs-lookup"><span data-stu-id="e6677-285">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one.</span></span> <span data-ttu-id="e6677-286">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span><span class="sxs-lookup"><span data-stu-id="e6677-286">Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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
  ]
}
-->
