---
title: 创建开放扩展
description: 创建开放扩展 (openTypeExtension 对象) 并添加自定义属性
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a654d0bc48bc5f4f83be4adaf258fa3186914745
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539951"
---
# <a name="create-open-extension"></a><span data-ttu-id="efba1-103">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="efba1-103">Create open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efba1-104">创建开放扩展 ([openTypeExtension](../resources/opentypeextension.md)对象), 并在新的或现有的受支持的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-104">Create an open extension ([openTypeExtension](../resources/opentypeextension.md) object) and add custom properties in a new or existing instance of a supported resource.</span></span>

> <span data-ttu-id="efba1-105">**注意:** 如果要创建 outlook 资源的开放扩展, 请参阅[openTypeExtension 资源类型](../resources/opentypeextension.md#outlook-specific-considerations)中的**Outlook 特定注意事项**。</span><span class="sxs-lookup"><span data-stu-id="efba1-105">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="efba1-106">权限</span><span class="sxs-lookup"><span data-stu-id="efba1-106">Permissions</span></span>

<span data-ttu-id="efba1-107">根据要在其中创建扩展的资源以及请求的权限类型 (委派或应用程序), 下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="efba1-107">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="efba1-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efba1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efba1-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="efba1-109">Supported resource</span></span> | <span data-ttu-id="efba1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efba1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efba1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efba1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efba1-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="efba1-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="efba1-113">设备</span><span class="sxs-lookup"><span data-stu-id="efba1-113">device</span></span>](../resources/device.md) | <span data-ttu-id="efba1-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="efba1-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="efba1-115">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-115">Not supported</span></span> | <span data-ttu-id="efba1-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="efba1-117">event</span><span class="sxs-lookup"><span data-stu-id="efba1-117">event</span></span>](../resources/event.md) | <span data-ttu-id="efba1-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="efba1-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="efba1-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="efba1-121">组</span><span class="sxs-lookup"><span data-stu-id="efba1-121">group</span></span>](../resources/group.md) | <span data-ttu-id="efba1-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="efba1-123">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-123">Not supported</span></span> | <span data-ttu-id="efba1-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="efba1-125">组事件</span><span class="sxs-lookup"><span data-stu-id="efba1-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="efba1-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="efba1-127">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-127">Not supported</span></span> | <span data-ttu-id="efba1-128">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-128">Not supported</span></span> |
| [<span data-ttu-id="efba1-129">组帖子</span><span class="sxs-lookup"><span data-stu-id="efba1-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="efba1-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="efba1-131">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-131">Not supported</span></span> | <span data-ttu-id="efba1-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="efba1-133">邮件</span><span class="sxs-lookup"><span data-stu-id="efba1-133">message</span></span>](../resources/message.md) | <span data-ttu-id="efba1-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-134">Mail.ReadWrite</span></span> | <span data-ttu-id="efba1-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-135">Mail.ReadWrite</span></span> | <span data-ttu-id="efba1-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="efba1-137">组织</span><span class="sxs-lookup"><span data-stu-id="efba1-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="efba1-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="efba1-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="efba1-139">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-139">Not supported</span></span> | <span data-ttu-id="efba1-140">不支持</span><span class="sxs-lookup"><span data-stu-id="efba1-140">Not supported</span></span> |
| [<span data-ttu-id="efba1-141">个人联系人</span><span class="sxs-lookup"><span data-stu-id="efba1-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="efba1-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="efba1-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="efba1-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="efba1-145">用户</span><span class="sxs-lookup"><span data-stu-id="efba1-145">user</span></span>](../resources/user.md) | <span data-ttu-id="efba1-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-146">User.ReadWrite.All</span></span> | <span data-ttu-id="efba1-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efba1-147">User.ReadWrite</span></span> | <span data-ttu-id="efba1-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efba1-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efba1-149">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efba1-149">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="efba1-150">在新资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="efba1-150">Create an extension in a new resource instance</span></span>

<span data-ttu-id="efba1-151">使用您用于创建实例的相同 REST 请求。</span><span class="sxs-lookup"><span data-stu-id="efba1-151">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="efba1-152">**注意:** 此语法展示了创建受支持的资源实例的一些常见方法。</span><span class="sxs-lookup"><span data-stu-id="efba1-152">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="efba1-153">所有其他允许您创建这些资源实例的 POST 语法都支持以类似方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="efba1-153">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="efba1-154">若要了解如何在请求正文中添加新资源实例[和扩展插件](#request-body)的属性，请参阅_请求正文_部分。</span><span class="sxs-lookup"><span data-stu-id="efba1-154">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="efba1-155">在现有资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="efba1-155">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="efba1-156">在请求中标识资源实例，然后对 `POST` 导航属性执行 \*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="efba1-156">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="efba1-157">**注意:** 此语法显示了一些用于标识资源实例的常见方法, 以便在其中创建扩展。</span><span class="sxs-lookup"><span data-stu-id="efba1-157">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="efba1-158">允许您标识这些资源实例的所有其他语法都支持以类似方式在其中创建开放扩展。</span><span class="sxs-lookup"><span data-stu-id="efba1-158">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="efba1-159">若要了解如何在请求正文中添加[扩展插件](#request-body)，请参阅_请求正文_部分。</span><span class="sxs-lookup"><span data-stu-id="efba1-159">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="efba1-160">路径参数</span><span class="sxs-lookup"><span data-stu-id="efba1-160">Path parameters</span></span>

|<span data-ttu-id="efba1-161">**参数**</span><span class="sxs-lookup"><span data-stu-id="efba1-161">**Parameter**</span></span>|<span data-ttu-id="efba1-162">**类型**</span><span class="sxs-lookup"><span data-stu-id="efba1-162">**Type**</span></span>|<span data-ttu-id="efba1-163">**说明**</span><span class="sxs-lookup"><span data-stu-id="efba1-163">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="efba1-164">id</span><span class="sxs-lookup"><span data-stu-id="efba1-164">id</span></span>|<span data-ttu-id="efba1-165">string</span><span class="sxs-lookup"><span data-stu-id="efba1-165">string</span></span>|<span data-ttu-id="efba1-p104">对象在相应集合中的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="efba1-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="efba1-168">请求标头</span><span class="sxs-lookup"><span data-stu-id="efba1-168">Request headers</span></span>

| <span data-ttu-id="efba1-169">名称</span><span class="sxs-lookup"><span data-stu-id="efba1-169">Name</span></span>       | <span data-ttu-id="efba1-170">值</span><span class="sxs-lookup"><span data-stu-id="efba1-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="efba1-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="efba1-171">Authorization</span></span> | <span data-ttu-id="efba1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efba1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efba1-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="efba1-174">Content-Type</span></span> | <span data-ttu-id="efba1-175">application/json</span><span class="sxs-lookup"><span data-stu-id="efba1-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="efba1-176">请求正文</span><span class="sxs-lookup"><span data-stu-id="efba1-176">Request body</span></span>

<span data-ttu-id="efba1-177">提供具有以下必需的名称-值对和任何其他自定义数据的[openTypeExtension](../resources/opentypeextension.md)的 JSON 正文。</span><span class="sxs-lookup"><span data-stu-id="efba1-177">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md), with the following required name-value pairs and any additional custom data.</span></span> <span data-ttu-id="efba1-178">JSON 负载中的数据可以是基元类型或基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="efba1-178">The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="efba1-179">名称</span><span class="sxs-lookup"><span data-stu-id="efba1-179">Name</span></span>       | <span data-ttu-id="efba1-180">值</span><span class="sxs-lookup"><span data-stu-id="efba1-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="efba1-181">@odata.type</span><span class="sxs-lookup"><span data-stu-id="efba1-181">@odata.type</span></span> | <span data-ttu-id="efba1-182">OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="efba1-182">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="efba1-183">extensionName</span><span class="sxs-lookup"><span data-stu-id="efba1-183">extensionName</span></span> | <span data-ttu-id="efba1-184">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="efba1-184">%unique_string%</span></span> |

<span data-ttu-id="efba1-185">在_新_资源实例中创建扩展插件时，除了新的 **openTypeExtension** 对象之外，还要提供 JSON 表示形式的相关属性才能创建此类资源实例。</span><span class="sxs-lookup"><span data-stu-id="efba1-185">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="efba1-186">响应</span><span class="sxs-lookup"><span data-stu-id="efba1-186">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="efba1-187">响应代码</span><span class="sxs-lookup"><span data-stu-id="efba1-187">Response code</span></span>

<span data-ttu-id="efba1-188">响应代码可以是 `201 Created`，也可以是 `202 Accepted`，具体视操作而定。</span><span class="sxs-lookup"><span data-stu-id="efba1-188">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="efba1-189">使用与创建资源实例相同的操作创建扩展时, 该操作将返回在使用操作创建资源实例而不带扩展时返回的响应代码。</span><span class="sxs-lookup"><span data-stu-id="efba1-189">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="efba1-190">请参阅有关创建实例的相应主题，如[上 ](#create-an-extension-in-a-new-resource-instance)所列。</span><span class="sxs-lookup"><span data-stu-id="efba1-190">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="efba1-191">响应正文</span><span class="sxs-lookup"><span data-stu-id="efba1-191">Response body</span></span>

| <span data-ttu-id="efba1-192">应用场景</span><span class="sxs-lookup"><span data-stu-id="efba1-192">Scenario</span></span>       | <span data-ttu-id="efba1-193">资源</span><span class="sxs-lookup"><span data-stu-id="efba1-193">Resource</span></span>  | <span data-ttu-id="efba1-194">响应正文</span><span class="sxs-lookup"><span data-stu-id="efba1-194">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="efba1-195">在显式创建_新_资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="efba1-195">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="efba1-196">[联系人](../resources/contact.md)、[事件](../resources/event.md)、[邮件](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="efba1-196">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="efba1-197">包括使用 [openTypeExtension](../resources/opentypeextension.md) 对象扩展的新实例。</span><span class="sxs-lookup"><span data-stu-id="efba1-197">Includes the new instance expanded with the [openTypeExtension](../resources/opentypeextension.md) object.</span></span> |
| <span data-ttu-id="efba1-198">在隐式创建资源实例的同时创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="efba1-198">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="efba1-199">帖子</span><span class="sxs-lookup"><span data-stu-id="efba1-199">post</span></span>](../resources/post.md) | <span data-ttu-id="efba1-200">响应只包括响应代码，不包括响应正文。</span><span class="sxs-lookup"><span data-stu-id="efba1-200">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="efba1-201">在_现有_资源实例中创建扩展插件</span><span class="sxs-lookup"><span data-stu-id="efba1-201">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="efba1-202">所有支持的资源</span><span class="sxs-lookup"><span data-stu-id="efba1-202">All supported resources</span></span> | <span data-ttu-id="efba1-203">包括 **openTypeExtension** 对象。</span><span class="sxs-lookup"><span data-stu-id="efba1-203">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="efba1-204">示例</span><span class="sxs-lookup"><span data-stu-id="efba1-204">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="efba1-205">请求 1</span><span class="sxs-lookup"><span data-stu-id="efba1-205">Request 1</span></span>

<span data-ttu-id="efba1-p108">第一个示例在同一个调用中创建一个邮件和一个扩展。请求正文包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="efba1-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="efba1-208">新邮件的典型 **subject**、**body** 和 **toRecipients** 属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-208">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="efba1-209">对于扩展：</span><span class="sxs-lookup"><span data-stu-id="efba1-209">And for the extension:</span></span>

  - <span data-ttu-id="efba1-210">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="efba1-210">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
  - <span data-ttu-id="efba1-211">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="efba1-211">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="efba1-212">要存储为 JSON 有效负载中的三个自定义属性的`companyName`其他`expirationDate`数据: `dealValue`、和。</span><span class="sxs-lookup"><span data-stu-id="efba1-212">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

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
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="efba1-213">响应 1</span><span class="sxs-lookup"><span data-stu-id="efba1-213">Response 1</span></span>

<span data-ttu-id="efba1-p109">下面是第一个示例的响应。响应正文包括新邮件的属性以及新扩展的以下属性：</span><span class="sxs-lookup"><span data-stu-id="efba1-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="efba1-216">具有完全限定的名称 \*\*\*\* 的 `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` 属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-216">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="efba1-217">请求中指定的默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="efba1-217">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="efba1-218">请求中指定的作为 3 个自定义属性存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="efba1-218">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="efba1-p110">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="efba1-221">请求 2</span><span class="sxs-lookup"><span data-stu-id="efba1-221">Request 2</span></span>

<span data-ttu-id="efba1-p111">第二个示例在指定邮件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="efba1-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="efba1-224">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="efba1-224">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="efba1-225">扩展名“Com.Contoso.Referral”。</span><span class="sxs-lookup"><span data-stu-id="efba1-225">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="efba1-226">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="efba1-226">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="efba1-227">响应 2</span><span class="sxs-lookup"><span data-stu-id="efba1-227">Response 2</span></span>

<span data-ttu-id="efba1-p112">下面是第二个示例的响应。请求正文包括新扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="efba1-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="efba1-230">默认属性 **extensionName**。</span><span class="sxs-lookup"><span data-stu-id="efba1-230">The default property **extensionName**.</span></span>
- <span data-ttu-id="efba1-231">具有完全限定的名称 \*\*\*\* 的 `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral` 属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-231">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="efba1-232">要存储的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="efba1-232">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="efba1-233">请求 3</span><span class="sxs-lookup"><span data-stu-id="efba1-233">Request 3</span></span>

<span data-ttu-id="efba1-p113">第三个示例在指定组事件中创建扩展。请求正文包括扩展的如下内容：</span><span class="sxs-lookup"><span data-stu-id="efba1-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="efba1-236">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="efba1-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="efba1-237">扩展名“Com.Contoso.Deal”。</span><span class="sxs-lookup"><span data-stu-id="efba1-237">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="efba1-238">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`dealValue` 和 `expirationDate`。</span><span class="sxs-lookup"><span data-stu-id="efba1-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="efba1-239">响应 3</span><span class="sxs-lookup"><span data-stu-id="efba1-239">Response 3</span></span>

<span data-ttu-id="efba1-240">下面是第三个示例请求的响应。</span><span class="sxs-lookup"><span data-stu-id="efba1-240">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="efba1-241">请求 4</span><span class="sxs-lookup"><span data-stu-id="efba1-241">Request 4</span></span>

<span data-ttu-id="efba1-p114">第四个示例对现有的组帖子使用相同的 **reply** 操作调用，在新的组帖子中创建扩展。**reply** 操作创建新帖子和嵌入帖子中的新扩展。请求正文包括 **post** 属性，此属性又包含新帖子的 **body** 以及新扩展的以下数据：</span><span class="sxs-lookup"><span data-stu-id="efba1-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="efba1-245">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="efba1-245">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="efba1-246">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="efba1-246">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="efba1-247">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="efba1-247">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-4"></a><span data-ttu-id="efba1-248">响应 4</span><span class="sxs-lookup"><span data-stu-id="efba1-248">Response 4</span></span>

<span data-ttu-id="efba1-p115">下面是第四个示例的响应。新的组帖子中成功创建扩展仅会产生 HTTP 202 响应代码。</span><span class="sxs-lookup"><span data-stu-id="efba1-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="efba1-251">响应 5</span><span class="sxs-lookup"><span data-stu-id="efba1-251">Request 5</span></span>

<span data-ttu-id="efba1-p116">第五个示例使用 POST 操作创建对话，在新的组帖子中创建扩展。POST 操作创建新对话、线程和帖子以及嵌入帖子中的新扩展。请求正文包括 **Topic** 和 **Threads** 属性以及新对话的子 **post** 对象。**post** 对象又包含新帖子的 **body** 和以下扩展数据：</span><span class="sxs-lookup"><span data-stu-id="efba1-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="efba1-256">`Microsoft.Graph.OpenTypeExtension` 类型。</span><span class="sxs-lookup"><span data-stu-id="efba1-256">The type `Microsoft.Graph.OpenTypeExtension`.</span></span>
- <span data-ttu-id="efba1-257">扩展名“Com.Contoso.HR”。</span><span class="sxs-lookup"><span data-stu-id="efba1-257">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="efba1-258">存储为 JSON 负载中的 3 个自定义属性的其他数据：`companyName`、`expirationDate` 和 `topPicks` 字符串数组。</span><span class="sxs-lookup"><span data-stu-id="efba1-258">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

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
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
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

### <a name="response-5"></a><span data-ttu-id="efba1-259">响应 5</span><span class="sxs-lookup"><span data-stu-id="efba1-259">Response 5</span></span>

<span data-ttu-id="efba1-p117">下面是第五个示例的响应，其中包含新对话和线程 ID。这个新线程包含自动创建的帖子，帖子又包含新扩展。</span><span class="sxs-lookup"><span data-stu-id="efba1-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="efba1-p118">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efba1-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="efba1-p119">若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread-list-posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension-get.md)。</span><span class="sxs-lookup"><span data-stu-id="efba1-p119">To get the new extension, first [get all the posts](../api/conversationthread-list-posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension-get.md).</span></span>

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
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
