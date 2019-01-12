---
title: 更新开放扩展
description: 通过请求正文中的属性更新开放扩展（openTypeExtension 对象）：
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 9aa2d69b4d285eb2ee290ed18a7da3d5e199859a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953208"
---
# <a name="update-open-extension"></a><span data-ttu-id="456f5-103">更新开放扩展</span><span class="sxs-lookup"><span data-stu-id="456f5-103">Update open extension</span></span>

> <span data-ttu-id="456f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="456f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="456f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="456f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="456f5-106">通过请求正文中的属性更新开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）：</span><span class="sxs-lookup"><span data-stu-id="456f5-106">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="456f5-107">如果请求正文中的属性与现有属性在扩展中的名称相匹配，则更新扩展中的数据。</span><span class="sxs-lookup"><span data-stu-id="456f5-107">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="456f5-108">否则，属性及其数据将添加到扩展中。</span><span class="sxs-lookup"><span data-stu-id="456f5-108">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="456f5-109">扩展中的数据可以是基元类型，也可以是基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="456f5-109">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="456f5-110">权限</span><span class="sxs-lookup"><span data-stu-id="456f5-110">Permissions</span></span>

<span data-ttu-id="456f5-111">根据扩展中创建的资源和权限类型 （委派或应用程序） 请求下, 表中所指定的权限是最小特权需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="456f5-111">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="456f5-112">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="456f5-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="456f5-113">支持的资源</span><span class="sxs-lookup"><span data-stu-id="456f5-113">Supported resource</span></span> | <span data-ttu-id="456f5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="456f5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="456f5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="456f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="456f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="456f5-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="456f5-117">设备</span><span class="sxs-lookup"><span data-stu-id="456f5-117">device</span></span>](../resources/device.md) | <span data-ttu-id="456f5-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="456f5-118">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="456f5-119">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-119">Not supported</span></span> | <span data-ttu-id="456f5-120">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-120">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="456f5-121">事件</span><span class="sxs-lookup"><span data-stu-id="456f5-121">event</span></span>](../resources/event.md) | <span data-ttu-id="456f5-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="456f5-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="456f5-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-124">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="456f5-125">组</span><span class="sxs-lookup"><span data-stu-id="456f5-125">group</span></span>](../resources/group.md) | <span data-ttu-id="456f5-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="456f5-127">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-127">Not supported</span></span> | <span data-ttu-id="456f5-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-128">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="456f5-129">组事件</span><span class="sxs-lookup"><span data-stu-id="456f5-129">group event</span></span>](../resources/event.md) | <span data-ttu-id="456f5-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="456f5-131">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-131">Not supported</span></span> | <span data-ttu-id="456f5-132">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-132">Not supported</span></span> |
| [<span data-ttu-id="456f5-133">组帖子</span><span class="sxs-lookup"><span data-stu-id="456f5-133">group post</span></span>](../resources/post.md) | <span data-ttu-id="456f5-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-134">Group.ReadWrite.All</span></span> | <span data-ttu-id="456f5-135">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-135">Not supported</span></span> | <span data-ttu-id="456f5-136">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-136">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="456f5-137">邮件</span><span class="sxs-lookup"><span data-stu-id="456f5-137">message</span></span>](../resources/message.md) | <span data-ttu-id="456f5-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-138">Mail.ReadWrite</span></span> | <span data-ttu-id="456f5-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-139">Mail.ReadWrite</span></span> | <span data-ttu-id="456f5-140">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-140">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="456f5-141">组织</span><span class="sxs-lookup"><span data-stu-id="456f5-141">organization</span></span>](../resources/organization.md) | <span data-ttu-id="456f5-142">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="456f5-142">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="456f5-143">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-143">Not supported</span></span> | <span data-ttu-id="456f5-144">不支持</span><span class="sxs-lookup"><span data-stu-id="456f5-144">Not supported</span></span> |
| [<span data-ttu-id="456f5-145">个人联系人</span><span class="sxs-lookup"><span data-stu-id="456f5-145">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="456f5-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="456f5-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-147">Contacts.ReadWrite</span></span> | <span data-ttu-id="456f5-148">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-148">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="456f5-149">用户</span><span class="sxs-lookup"><span data-stu-id="456f5-149">user</span></span>](../resources/user.md) | <span data-ttu-id="456f5-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-150">User.ReadWrite.All</span></span> | <span data-ttu-id="456f5-151">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456f5-151">User.ReadWrite</span></span> | <span data-ttu-id="456f5-152">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456f5-152">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="456f5-153">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="456f5-153">HTTP request</span></span>

<span data-ttu-id="456f5-154">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `PATCH`。</span><span class="sxs-lookup"><span data-stu-id="456f5-154">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{Id}/extensions/{extensionId}
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="456f5-p103">**注意：** 以上语法显示一些标识资源实例的常见方法，以便在其中更新一个扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式在其中更新开放扩展。</span><span class="sxs-lookup"><span data-stu-id="456f5-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="456f5-157">若要了解如何在请求正文中添加任意自定义数据来进行更改或添加到扩展插件，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="456f5-157">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="456f5-158">路径参数</span><span class="sxs-lookup"><span data-stu-id="456f5-158">Path parameters</span></span>
|<span data-ttu-id="456f5-159">**参数**</span><span class="sxs-lookup"><span data-stu-id="456f5-159">**Parameter**</span></span>|<span data-ttu-id="456f5-160">**类型**</span><span class="sxs-lookup"><span data-stu-id="456f5-160">**Type**</span></span>|<span data-ttu-id="456f5-161">**说明**</span><span class="sxs-lookup"><span data-stu-id="456f5-161">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="456f5-162">id</span><span class="sxs-lookup"><span data-stu-id="456f5-162">id</span></span>|<span data-ttu-id="456f5-163">string</span><span class="sxs-lookup"><span data-stu-id="456f5-163">string</span></span>|<span data-ttu-id="456f5-p104">相应集合的实例的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="456f5-p104">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="456f5-166">extensionId</span><span class="sxs-lookup"><span data-stu-id="456f5-166">extensionId</span></span>|<span data-ttu-id="456f5-167">string</span><span class="sxs-lookup"><span data-stu-id="456f5-167">string</span></span>|<span data-ttu-id="456f5-p105">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="456f5-p105">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="456f5-171">请求标头</span><span class="sxs-lookup"><span data-stu-id="456f5-171">Request headers</span></span>
| <span data-ttu-id="456f5-172">名称</span><span class="sxs-lookup"><span data-stu-id="456f5-172">Name</span></span>       | <span data-ttu-id="456f5-173">值</span><span class="sxs-lookup"><span data-stu-id="456f5-173">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="456f5-174">Authorization</span><span class="sxs-lookup"><span data-stu-id="456f5-174">Authorization</span></span> | <span data-ttu-id="456f5-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="456f5-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="456f5-177">Content-Type</span><span class="sxs-lookup"><span data-stu-id="456f5-177">Content-Type</span></span> | <span data-ttu-id="456f5-178">application/json</span><span class="sxs-lookup"><span data-stu-id="456f5-178">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="456f5-179">请求正文</span><span class="sxs-lookup"><span data-stu-id="456f5-179">Request body</span></span>

<span data-ttu-id="456f5-p107">提供 [openTypeExtension](../resources/opentypeextension.md) 对象的 JSON 正文（具有以下所需的名称-值对）以及要更改或添加到该扩展中的任意定义数据。JSON 负载中的数据可以是基元或基元数组类型。</span><span class="sxs-lookup"><span data-stu-id="456f5-p107">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="456f5-182">名称</span><span class="sxs-lookup"><span data-stu-id="456f5-182">Name</span></span>       | <span data-ttu-id="456f5-183">值</span><span class="sxs-lookup"><span data-stu-id="456f5-183">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="456f5-184">@odata.type</span><span class="sxs-lookup"><span data-stu-id="456f5-184">@odata.type</span></span> | <span data-ttu-id="456f5-185">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="456f5-185">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="456f5-186">extensionName</span><span class="sxs-lookup"><span data-stu-id="456f5-186">extensionName</span></span> | <span data-ttu-id="456f5-187">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="456f5-187">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="456f5-188">响应</span><span class="sxs-lookup"><span data-stu-id="456f5-188">Response</span></span>

<span data-ttu-id="456f5-189">如果成功，此方法返回 `200 OK` 响应代码和更新的 [openTypeExtension](../resources/opentypeextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="456f5-189">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="456f5-190">示例</span><span class="sxs-lookup"><span data-stu-id="456f5-190">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="456f5-191">请求 1</span><span class="sxs-lookup"><span data-stu-id="456f5-191">Request 1</span></span>

<span data-ttu-id="456f5-p108">第一个示例展示如何在邮件中更新扩展。该扩展最初由以下 JSON 负载表示：</span><span class="sxs-lookup"><span data-stu-id="456f5-p108">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="456f5-194">可以按其名称引用该扩展，</span><span class="sxs-lookup"><span data-stu-id="456f5-194">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="456f5-195">或者，也可以通过其完全限定的名称引用扩展：</span><span class="sxs-lookup"><span data-stu-id="456f5-195">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="456f5-196">可以通过以下方法，使用示例请求和以下请求正文更新以上扩展：</span><span class="sxs-lookup"><span data-stu-id="456f5-196">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="456f5-197">将 `companyName` 从 `Wingtip Toys` 更改为 `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="456f5-197">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="456f5-198">将 `dealValue` 从 `500050` 更改为 `500100`</span><span class="sxs-lookup"><span data-stu-id="456f5-198">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="456f5-199">将新数据添加为自定义属性 `updated`</span><span class="sxs-lookup"><span data-stu-id="456f5-199">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="456f5-200">响应 1</span><span class="sxs-lookup"><span data-stu-id="456f5-200">Response 1</span></span>

<span data-ttu-id="456f5-201">无论用于引用扩展的方式如何，该响应都相同。</span><span class="sxs-lookup"><span data-stu-id="456f5-201">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="456f5-202">请求 2</span><span class="sxs-lookup"><span data-stu-id="456f5-202">Request 2</span></span>

<span data-ttu-id="456f5-p109">第二个示例展示如何在组帖子中更新扩展。该扩展最初由以下 JSON 负载表示，其中的 `2015-07-03T13:04:00Z` 的值为 `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="456f5-p109">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="456f5-205">以下是要将 `expirationDate` 更改为 `2016-07-30T11:00:00Z` 的请求和请求正文：</span><span class="sxs-lookup"><span data-stu-id="456f5-205">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="456f5-206">响应 2</span><span class="sxs-lookup"><span data-stu-id="456f5-206">Response 2</span></span>

<span data-ttu-id="456f5-207">下面是第二个示例的响应，显示了扩展中更新的 `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="456f5-207">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.opentypeextension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
