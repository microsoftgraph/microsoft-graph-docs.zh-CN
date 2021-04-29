---
title: 创建开放扩展
description: 创建开放扩展（openTypeExtension 对象），并在资源的新实例或现有实例中添加自定义属性。
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: f91a549e13b956d9c0d1fa4d8ca8765e7b7bd89a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052220"
---
# <a name="create-open-extension"></a><span data-ttu-id="933d7-103">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="933d7-103">Create open extension</span></span>

<span data-ttu-id="933d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="933d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="933d7-105">创建开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象），并在资源的新实例或现有实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="933d7-105">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="933d7-106">"权限" ["](#permissions) "部分中列出支持打开扩展的资源。</span><span class="sxs-lookup"><span data-stu-id="933d7-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

> <span data-ttu-id="933d7-107">**请注意：** 如果要在 Outlook 资源上创建开放扩展，请参阅 [openTypeExtension 资源类型](../resources/opentypeextension.md#outlook-specific-considerations)中的 **Outlook 特定注意事项**。</span><span class="sxs-lookup"><span data-stu-id="933d7-107">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="933d7-108">权限</span><span class="sxs-lookup"><span data-stu-id="933d7-108">Permissions</span></span>

<span data-ttu-id="933d7-109">根据要在其中创建扩展的资源和所请求的权限类型（委派或应用程序），下表中指定的权限是指调用此 API 所需的最低限度的特权。</span><span class="sxs-lookup"><span data-stu-id="933d7-109">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="933d7-110">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="933d7-110">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="933d7-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="933d7-111">Supported resource</span></span> | <span data-ttu-id="933d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="933d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="933d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="933d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="933d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="933d7-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="933d7-115">设备</span><span class="sxs-lookup"><span data-stu-id="933d7-115">device</span></span>](../resources/device.md) | <span data-ttu-id="933d7-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="933d7-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="933d7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-117">Not supported</span></span> | <span data-ttu-id="933d7-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-119">事件</span><span class="sxs-lookup"><span data-stu-id="933d7-119">event</span></span>](../resources/event.md) | <span data-ttu-id="933d7-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="933d7-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="933d7-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="933d7-123">组</span><span class="sxs-lookup"><span data-stu-id="933d7-123">group</span></span>](../resources/group.md) | <span data-ttu-id="933d7-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="933d7-125">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-125">Not supported</span></span> | <span data-ttu-id="933d7-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-127">组事件</span><span class="sxs-lookup"><span data-stu-id="933d7-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="933d7-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="933d7-129">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-129">Not supported</span></span> | <span data-ttu-id="933d7-130">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-130">Not supported</span></span> |
| [<span data-ttu-id="933d7-131">组帖子</span><span class="sxs-lookup"><span data-stu-id="933d7-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="933d7-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="933d7-133">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-133">Not supported</span></span> | <span data-ttu-id="933d7-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-135">邮件</span><span class="sxs-lookup"><span data-stu-id="933d7-135">message</span></span>](../resources/message.md) | <span data-ttu-id="933d7-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-136">Mail.ReadWrite</span></span> | <span data-ttu-id="933d7-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-137">Mail.ReadWrite</span></span> | <span data-ttu-id="933d7-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="933d7-139">组织</span><span class="sxs-lookup"><span data-stu-id="933d7-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="933d7-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-140">Organization.ReadWrite.All</span></span> | <span data-ttu-id="933d7-141">不支持</span><span class="sxs-lookup"><span data-stu-id="933d7-141">Not supported</span></span> | <span data-ttu-id="933d7-142">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-142">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-143">个人联系人</span><span class="sxs-lookup"><span data-stu-id="933d7-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="933d7-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="933d7-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="933d7-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="933d7-147">用户</span><span class="sxs-lookup"><span data-stu-id="933d7-147">user</span></span>](../resources/user.md) | <span data-ttu-id="933d7-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-148">User.ReadWrite</span></span> | <span data-ttu-id="933d7-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-149">User.ReadWrite</span></span> | <span data-ttu-id="933d7-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-150">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-151">task</span><span class="sxs-lookup"><span data-stu-id="933d7-151">task</span></span>](../resources/todotask.md) | <span data-ttu-id="933d7-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="933d7-153">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-153">Tasks.ReadWrite</span></span> | <span data-ttu-id="933d7-154">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-154">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="933d7-155">任务列表</span><span class="sxs-lookup"><span data-stu-id="933d7-155">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="933d7-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="933d7-157">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933d7-157">Tasks.ReadWrite</span></span> | <span data-ttu-id="933d7-158">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="933d7-158">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="933d7-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="933d7-159">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="933d7-160">在新资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="933d7-160">Create an extension in a new resource instance</span></span>

<span data-ttu-id="933d7-161">使用创建实例时所用的同一 REST 请求。</span><span class="sxs-lookup"><span data-stu-id="933d7-161">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks
POST /users/{id|userPrincipalName}/todo/lists
```

><span data-ttu-id="933d7-p102">**注意：** 此语法显示了一些创建支持的资源实例的常见方法。可以用来创建这些资源实例的所有其他 POST 语法均支持以类似的方式从中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="933d7-p102">**Note:** This syntax shows some common ways to create the supported resource instances. All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="933d7-164">若要了解如何在请求正文中添加新资源实例和 _扩展_ 的属性，请参阅 [请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="933d7-164">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="933d7-165">在现有资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="933d7-165">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="933d7-166">在请求中标识资源实例，然后对 **extensions** 导航属性执行 `POST`。</span><span class="sxs-lookup"><span data-stu-id="933d7-166">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/tasks/{id}/extensions
POST /users/{id|userPrincipalName}/todo/lists/{id}/extensions
```

><span data-ttu-id="933d7-p103">**注意：** 此语法显示了一些标识资源实例的常见方法，以便在其中创建一个扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="933d7-p103">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="933d7-169">若要了解如何在请求正文中添加 _扩展_，请参阅 [请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="933d7-169">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="933d7-170">路径参数</span><span class="sxs-lookup"><span data-stu-id="933d7-170">Path parameters</span></span>
|<span data-ttu-id="933d7-171">参数</span><span class="sxs-lookup"><span data-stu-id="933d7-171">Parameter</span></span>|<span data-ttu-id="933d7-172">类型</span><span class="sxs-lookup"><span data-stu-id="933d7-172">Type</span></span>|<span data-ttu-id="933d7-173">说明</span><span class="sxs-lookup"><span data-stu-id="933d7-173">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="933d7-174">id</span><span class="sxs-lookup"><span data-stu-id="933d7-174">id</span></span>|<span data-ttu-id="933d7-175">string</span><span class="sxs-lookup"><span data-stu-id="933d7-175">string</span></span>|<span data-ttu-id="933d7-p104">对象在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="933d7-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="933d7-178">请求标头</span><span class="sxs-lookup"><span data-stu-id="933d7-178">Request headers</span></span>

| <span data-ttu-id="933d7-179">名称</span><span class="sxs-lookup"><span data-stu-id="933d7-179">Name</span></span>       | <span data-ttu-id="933d7-180">值</span><span class="sxs-lookup"><span data-stu-id="933d7-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="933d7-181">Authorization</span><span class="sxs-lookup"><span data-stu-id="933d7-181">Authorization</span></span> | <span data-ttu-id="933d7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="933d7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="933d7-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="933d7-184">Content-Type</span></span> | <span data-ttu-id="933d7-185">application/json</span><span class="sxs-lookup"><span data-stu-id="933d7-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="933d7-186">请求正文</span><span class="sxs-lookup"><span data-stu-id="933d7-186">Request body</span></span>

<span data-ttu-id="933d7-p106">提供 [openTypeExtension](../resources/opentypeextension.md) 的 JSON 正文（具有以下所需的名称-值对）以及其他任意自定义数据。JSON 负载中的数据可以是基元类型或基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="933d7-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="933d7-189">名称</span><span class="sxs-lookup"><span data-stu-id="933d7-189">Name</span></span>       | <span data-ttu-id="933d7-190">值</span><span class="sxs-lookup"><span data-stu-id="933d7-190">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="933d7-191">@odata.type</span><span class="sxs-lookup"><span data-stu-id="933d7-191">@odata.type</span></span> | <span data-ttu-id="933d7-192">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="933d7-192">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="933d7-193">extensionName</span><span class="sxs-lookup"><span data-stu-id="933d7-193">extensionName</span></span> | <span data-ttu-id="933d7-194">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="933d7-194">%unique_string%</span></span> |

<span data-ttu-id="933d7-195">在 _新_ 资源实例中创建扩展插件时，除了新的 **openTypeExtension** 对象之外，还要提供 JSON 表示形式的相关属性才能创建此类资源实例。</span><span class="sxs-lookup"><span data-stu-id="933d7-195">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="933d7-196">响应</span><span class="sxs-lookup"><span data-stu-id="933d7-196">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="933d7-197">响应代码</span><span class="sxs-lookup"><span data-stu-id="933d7-197">Response code</span></span>

<span data-ttu-id="933d7-198">响应代码可以是 `201 Created`，也可以是 `202 Accepted`，具体视操作而定。</span><span class="sxs-lookup"><span data-stu-id="933d7-198">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="933d7-p107">使用你用于创建资源实例的相同操作创建扩展时，操作所返回的响应代码与通过该操作创建不带扩展的资源实例时返回的代码相同。请参阅有关创建实例的相应主题，如[上](#create-an-extension-in-a-new-resource-instance)所列。</span><span class="sxs-lookup"><span data-stu-id="933d7-p107">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="933d7-201">响应正文</span><span class="sxs-lookup"><span data-stu-id="933d7-201">Response body</span></span>

| <span data-ttu-id="933d7-202">应用场景</span><span class="sxs-lookup"><span data-stu-id="933d7-202">Scenario</span></span>       | <span data-ttu-id="933d7-203">资源</span><span class="sxs-lookup"><span data-stu-id="933d7-203">Resource</span></span>  | <span data-ttu-id="933d7-204">响应正文</span><span class="sxs-lookup"><span data-stu-id="933d7-204">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="933d7-205">在显式创建 _新_ 资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="933d7-205">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="933d7-206">[联系人](../resources/contact.md)、[事件](../resources/event.md)、[邮件](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="933d7-206">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="933d7-207">包括使用 [openTypeExtension](../resources/opentypeextension.md) 对象扩展的新实例。</span><span class="sxs-lookup"><span data-stu-id="933d7-207">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="933d7-208">在隐式创建资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="933d7-208">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="933d7-209">帖子</span><span class="sxs-lookup"><span data-stu-id="933d7-209">post</span></span>](../resources/post.md) | <span data-ttu-id="933d7-210">响应只包括响应代码，不包括响应正文。</span><span class="sxs-lookup"><span data-stu-id="933d7-210">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="933d7-211">在 _现有_ 资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="933d7-211">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="933d7-212">所有支持的资源</span><span class="sxs-lookup"><span data-stu-id="933d7-212">All supported resources</span></span> | <span data-ttu-id="933d7-213">包括 **openTypeExtension** 对象。</span><span class="sxs-lookup"><span data-stu-id="933d7-213">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="933d7-214">示例</span><span class="sxs-lookup"><span data-stu-id="933d7-214">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="933d7-215">请求 1</span><span class="sxs-lookup"><span data-stu-id="933d7-215">Request 1</span></span>

<span data-ttu-id="933d7-p108">第一个示例在同一个调用中创建一个邮件和一个扩展。请求正文包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="933d7-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="933d7-218">新邮件的典型 **subject**、**body** 和 **toRecipients** 属性。</span><span class="sxs-lookup"><span data-stu-id="933d7-218">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="933d7-219">对于扩展：</span><span class="sxs-lookup"><span data-stu-id="933d7-219">And for the extension:</span></span>

  - <span data-ttu-id="933d7-220">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="933d7-220">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="933d7-221">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="933d7-221">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="933d7-222">存储为 JSON 有效负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `dealValue`。</span><span class="sxs-lookup"><span data-stu-id="933d7-222">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>


# <a name="http"></a>[<span data-ttu-id="933d7-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="933d7-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

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
# <a name="c"></a>[<span data-ttu-id="933d7-224">C#</span><span class="sxs-lookup"><span data-stu-id="933d7-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="933d7-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="933d7-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="933d7-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="933d7-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-1"></a><span data-ttu-id="933d7-227">响应 1</span><span class="sxs-lookup"><span data-stu-id="933d7-227">Response 1</span></span>

<span data-ttu-id="933d7-p109">下面是第一个示例的响应。响应正文包括新邮件的属性以及新扩展的以下属性：</span><span class="sxs-lookup"><span data-stu-id="933d7-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="933d7-230">具有完全限定的名称 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="933d7-230">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="933d7-231">请求中指定的默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="933d7-231">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="933d7-232">请求中指定的作为 3 个自定义属性存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="933d7-232">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="933d7-233">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="933d7-233">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
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
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
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

### <a name="request-2"></a><span data-ttu-id="933d7-234">请求 2</span><span class="sxs-lookup"><span data-stu-id="933d7-234">Request 2</span></span>

<span data-ttu-id="933d7-p110">第二个示例在指定邮件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="933d7-p110">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="933d7-237">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="933d7-237">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="933d7-238">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="933d7-238">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="933d7-239">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="933d7-239">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="933d7-240">HTTP</span><span class="sxs-lookup"><span data-stu-id="933d7-240">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="933d7-241">C#</span><span class="sxs-lookup"><span data-stu-id="933d7-241">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="933d7-242">JavaScript</span><span class="sxs-lookup"><span data-stu-id="933d7-242">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="933d7-243">Objective-C</span><span class="sxs-lookup"><span data-stu-id="933d7-243">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-2"></a><span data-ttu-id="933d7-244">响应 2</span><span class="sxs-lookup"><span data-stu-id="933d7-244">Response 2</span></span>

<span data-ttu-id="933d7-p111">下面是第二个示例的响应。请求正文包括新扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="933d7-p111">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="933d7-247">默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="933d7-247">The default property **extensionName**.</span></span>
- <span data-ttu-id="933d7-248">具有完全限定的名称 `microsoft.graph.openTypeExtension.Com.Contoso.Referral` 的 **Id** 属性。</span><span class="sxs-lookup"><span data-stu-id="933d7-248">The **id** property with the fully qualified name of `microsoft.graph.openTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="933d7-249">要存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="933d7-249">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('microsoft.graph.openTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="933d7-250">请求 3</span><span class="sxs-lookup"><span data-stu-id="933d7-250">Request 3</span></span>

<span data-ttu-id="933d7-p112">第三个示例在指定组事件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="933d7-p112">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="933d7-253">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="933d7-253">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="933d7-254">扩展名“Com.Contoso.Deal”。</span><span class="sxs-lookup"><span data-stu-id="933d7-254">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="933d7-255">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="933d7-255">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>


# <a name="http"></a>[<span data-ttu-id="933d7-256">HTTP</span><span class="sxs-lookup"><span data-stu-id="933d7-256">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="933d7-257">C#</span><span class="sxs-lookup"><span data-stu-id="933d7-257">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="933d7-258">JavaScript</span><span class="sxs-lookup"><span data-stu-id="933d7-258">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="933d7-259">Objective-C</span><span class="sxs-lookup"><span data-stu-id="933d7-259">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-3"></a><span data-ttu-id="933d7-260">响应 3</span><span class="sxs-lookup"><span data-stu-id="933d7-260">Response 3</span></span>

<span data-ttu-id="933d7-261">下面是第三个示例请求的响应。</span><span class="sxs-lookup"><span data-stu-id="933d7-261">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "microsoft.graph.openTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="933d7-262">请求 4</span><span class="sxs-lookup"><span data-stu-id="933d7-262">Request 4</span></span>

<span data-ttu-id="933d7-p113">第四个示例对现有的组帖子使用相同的 **reply** 操作调用，在新的组帖子中创建扩展。**reply** 操作创建新帖子和嵌入帖子中的新扩展。请求正文包括 **post** 属性，此属性又包含新帖子的 **body** 以及新扩展的以下数据：</span><span class="sxs-lookup"><span data-stu-id="933d7-p113">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="933d7-266">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="933d7-266">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="933d7-267">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="933d7-267">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="933d7-268">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="933d7-268">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="933d7-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="933d7-269">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

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
# <a name="c"></a>[<span data-ttu-id="933d7-270">C#</span><span class="sxs-lookup"><span data-stu-id="933d7-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="933d7-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="933d7-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="933d7-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="933d7-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-4"></a><span data-ttu-id="933d7-273">响应 4</span><span class="sxs-lookup"><span data-stu-id="933d7-273">Response 4</span></span>

<span data-ttu-id="933d7-p114">下面是第四个示例的响应。新的组帖子中成功创建扩展仅会产生 HTTP 202 响应代码。</span><span class="sxs-lookup"><span data-stu-id="933d7-p114">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="933d7-276">响应 5</span><span class="sxs-lookup"><span data-stu-id="933d7-276">Request 5</span></span>

<span data-ttu-id="933d7-p115">第五个示例使用 POST 操作创建对话，在新的组帖子中创建扩展。POST 操作创建新对话、线程和帖子以及嵌入帖子中的新扩展。请求正文包括 **Topic** 和 **Threads** 属性以及新对话的子 **post** 对象。**post** 对象又包含新帖子的 **body** 和以下扩展数据：</span><span class="sxs-lookup"><span data-stu-id="933d7-p115">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="933d7-281">`microsoft.graph.openTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="933d7-281">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="933d7-282">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="933d7-282">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="933d7-283">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="933d7-283">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>


# <a name="http"></a>[<span data-ttu-id="933d7-284">HTTP</span><span class="sxs-lookup"><span data-stu-id="933d7-284">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

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
# <a name="c"></a>[<span data-ttu-id="933d7-285">C#</span><span class="sxs-lookup"><span data-stu-id="933d7-285">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-opentypeextension-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="933d7-286">JavaScript</span><span class="sxs-lookup"><span data-stu-id="933d7-286">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-opentypeextension-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="933d7-287">Objective-C</span><span class="sxs-lookup"><span data-stu-id="933d7-287">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-opentypeextension-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response-5"></a><span data-ttu-id="933d7-288">响应 5</span><span class="sxs-lookup"><span data-stu-id="933d7-288">Response 5</span></span>

<span data-ttu-id="933d7-p116">下面是第五个示例的响应，其中包含新对话和线程 ID。这个新线程包含自动创建的帖子，帖子又包含新扩展。</span><span class="sxs-lookup"><span data-stu-id="933d7-p116">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="933d7-291">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="933d7-291">Note: The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="933d7-p117">若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread-list-posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension-get.md)。</span><span class="sxs-lookup"><span data-stu-id="933d7-p117">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

