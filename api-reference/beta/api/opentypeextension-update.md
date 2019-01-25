---
title: 更新开放扩展
description: 通过请求正文中的属性更新开放扩展（openTypeExtension 对象）：
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: c24714f51a75f17ebe56314ab6dc683701085420
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519995"
---
# <a name="update-open-extension"></a><span data-ttu-id="cbb9b-103">更新开放扩展</span><span class="sxs-lookup"><span data-stu-id="cbb9b-103">Update open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbb9b-104">通过请求正文中的属性更新开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）：</span><span class="sxs-lookup"><span data-stu-id="cbb9b-104">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="cbb9b-105">如果请求正文中的属性与现有属性在扩展中的名称相匹配，则更新扩展中的数据。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-105">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="cbb9b-106">否则，属性及其数据将添加到扩展中。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-106">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="cbb9b-107">扩展中的数据可以是基元类型，也可以是基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-107">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbb9b-108">权限</span><span class="sxs-lookup"><span data-stu-id="cbb9b-108">Permissions</span></span>

<span data-ttu-id="cbb9b-109">根据扩展中创建的资源和权限类型 （委派或应用程序） 请求下, 表中所指定的权限是最小特权需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-109">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="cbb9b-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbb9b-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="cbb9b-111">Supported resource</span></span> | <span data-ttu-id="cbb9b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbb9b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbb9b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbb9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbb9b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbb9b-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="cbb9b-115">设备</span><span class="sxs-lookup"><span data-stu-id="cbb9b-115">device</span></span>](../resources/device.md) | <span data-ttu-id="cbb9b-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="cbb9b-117">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-117">Not supported</span></span> | <span data-ttu-id="cbb9b-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="cbb9b-119">事件</span><span class="sxs-lookup"><span data-stu-id="cbb9b-119">event</span></span>](../resources/event.md) | <span data-ttu-id="cbb9b-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="cbb9b-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="cbb9b-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="cbb9b-123">组</span><span class="sxs-lookup"><span data-stu-id="cbb9b-123">group</span></span>](../resources/group.md) | <span data-ttu-id="cbb9b-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="cbb9b-125">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-125">Not supported</span></span> | <span data-ttu-id="cbb9b-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="cbb9b-127">组事件</span><span class="sxs-lookup"><span data-stu-id="cbb9b-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="cbb9b-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="cbb9b-129">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-129">Not supported</span></span> | <span data-ttu-id="cbb9b-130">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-130">Not supported</span></span> |
| [<span data-ttu-id="cbb9b-131">组帖子</span><span class="sxs-lookup"><span data-stu-id="cbb9b-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="cbb9b-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="cbb9b-133">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-133">Not supported</span></span> | <span data-ttu-id="cbb9b-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="cbb9b-135">邮件</span><span class="sxs-lookup"><span data-stu-id="cbb9b-135">message</span></span>](../resources/message.md) | <span data-ttu-id="cbb9b-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-136">Mail.ReadWrite</span></span> | <span data-ttu-id="cbb9b-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-137">Mail.ReadWrite</span></span> | <span data-ttu-id="cbb9b-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="cbb9b-139">组织</span><span class="sxs-lookup"><span data-stu-id="cbb9b-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="cbb9b-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="cbb9b-141">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-141">Not supported</span></span> | <span data-ttu-id="cbb9b-142">不支持</span><span class="sxs-lookup"><span data-stu-id="cbb9b-142">Not supported</span></span> |
| [<span data-ttu-id="cbb9b-143">个人联系人</span><span class="sxs-lookup"><span data-stu-id="cbb9b-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="cbb9b-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="cbb9b-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="cbb9b-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="cbb9b-147">用户</span><span class="sxs-lookup"><span data-stu-id="cbb9b-147">user</span></span>](../resources/user.md) | <span data-ttu-id="cbb9b-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-148">User.ReadWrite.All</span></span> | <span data-ttu-id="cbb9b-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb9b-149">User.ReadWrite</span></span> | <span data-ttu-id="cbb9b-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb9b-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbb9b-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbb9b-151">HTTP request</span></span>

<span data-ttu-id="cbb9b-152">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `PATCH`。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-152">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

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

><span data-ttu-id="cbb9b-p102">**注意：** 以上语法显示一些标识资源实例的常见方法，以便在其中更新一个扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式在其中更新开放扩展。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="cbb9b-155">若要了解如何在请求正文中添加任意自定义数据来进行更改或添加到扩展插件，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-155">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="cbb9b-156">路径参数</span><span class="sxs-lookup"><span data-stu-id="cbb9b-156">Path parameters</span></span>
|<span data-ttu-id="cbb9b-157">**参数**</span><span class="sxs-lookup"><span data-stu-id="cbb9b-157">**Parameter**</span></span>|<span data-ttu-id="cbb9b-158">**类型**</span><span class="sxs-lookup"><span data-stu-id="cbb9b-158">**Type**</span></span>|<span data-ttu-id="cbb9b-159">**说明**</span><span class="sxs-lookup"><span data-stu-id="cbb9b-159">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cbb9b-160">id</span><span class="sxs-lookup"><span data-stu-id="cbb9b-160">id</span></span>|<span data-ttu-id="cbb9b-161">string</span><span class="sxs-lookup"><span data-stu-id="cbb9b-161">string</span></span>|<span data-ttu-id="cbb9b-p103">相应集合的实例的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="cbb9b-164">extensionId</span><span class="sxs-lookup"><span data-stu-id="cbb9b-164">extensionId</span></span>|<span data-ttu-id="cbb9b-165">string</span><span class="sxs-lookup"><span data-stu-id="cbb9b-165">string</span></span>|<span data-ttu-id="cbb9b-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="cbb9b-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbb9b-169">Request headers</span></span>
| <span data-ttu-id="cbb9b-170">Name</span><span class="sxs-lookup"><span data-stu-id="cbb9b-170">Name</span></span>       | <span data-ttu-id="cbb9b-171">值</span><span class="sxs-lookup"><span data-stu-id="cbb9b-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cbb9b-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbb9b-172">Authorization</span></span> | <span data-ttu-id="cbb9b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbb9b-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbb9b-175">Content-Type</span></span> | <span data-ttu-id="cbb9b-176">application/json</span><span class="sxs-lookup"><span data-stu-id="cbb9b-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbb9b-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbb9b-177">Request body</span></span>

<span data-ttu-id="cbb9b-p106">提供 [openTypeExtension](../resources/opentypeextension.md) 对象的 JSON 正文（具有以下所需的名称-值对）以及要更改或添加到该扩展中的任意定义数据。JSON 负载中的数据可以是基元或基元数组类型。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="cbb9b-180">名称</span><span class="sxs-lookup"><span data-stu-id="cbb9b-180">Name</span></span>       | <span data-ttu-id="cbb9b-181">值</span><span class="sxs-lookup"><span data-stu-id="cbb9b-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cbb9b-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="cbb9b-182">@odata.type</span></span> | <span data-ttu-id="cbb9b-183">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="cbb9b-183">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="cbb9b-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="cbb9b-184">extensionName</span></span> | <span data-ttu-id="cbb9b-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="cbb9b-185">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="cbb9b-186">响应</span><span class="sxs-lookup"><span data-stu-id="cbb9b-186">Response</span></span>

<span data-ttu-id="cbb9b-187">如果成功，此方法返回 `200 OK` 响应代码和更新的 [openTypeExtension](../resources/opentypeextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-187">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="cbb9b-188">示例</span><span class="sxs-lookup"><span data-stu-id="cbb9b-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="cbb9b-189">请求 1</span><span class="sxs-lookup"><span data-stu-id="cbb9b-189">Request 1</span></span>

<span data-ttu-id="cbb9b-p107">第一个示例展示如何在邮件中更新扩展。该扩展最初由以下 JSON 负载表示：</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

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

<span data-ttu-id="cbb9b-192">可以按其名称引用该扩展，</span><span class="sxs-lookup"><span data-stu-id="cbb9b-192">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="cbb9b-193">或者，也可以通过其完全限定的名称引用扩展：</span><span class="sxs-lookup"><span data-stu-id="cbb9b-193">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="cbb9b-194">可以通过以下方法，使用示例请求和以下请求正文更新以上扩展：</span><span class="sxs-lookup"><span data-stu-id="cbb9b-194">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="cbb9b-195">将 `companyName` 从 `Wingtip Toys` 更改为 `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="cbb9b-195">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="cbb9b-196">将 `dealValue` 从 `500050` 更改为 `500100`</span><span class="sxs-lookup"><span data-stu-id="cbb9b-196">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="cbb9b-197">将新数据添加为自定义属性 `updated`</span><span class="sxs-lookup"><span data-stu-id="cbb9b-197">Adding new data as the custom property `updated`</span></span>

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


#### <a name="response-1"></a><span data-ttu-id="cbb9b-198">响应 1</span><span class="sxs-lookup"><span data-stu-id="cbb9b-198">Response 1</span></span>

<span data-ttu-id="cbb9b-199">无论用于引用扩展的方式如何，该响应都相同。</span><span class="sxs-lookup"><span data-stu-id="cbb9b-199">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="cbb9b-200">请求 2</span><span class="sxs-lookup"><span data-stu-id="cbb9b-200">Request 2</span></span>

<span data-ttu-id="cbb9b-p108">第二个示例展示如何在组帖子中更新扩展。该扩展最初由以下 JSON 负载表示，其中的 `2015-07-03T13:04:00Z` 的值为 `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="cbb9b-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

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

<span data-ttu-id="cbb9b-203">以下是要将 `expirationDate` 更改为 `2016-07-30T11:00:00Z` 的请求和请求正文：</span><span class="sxs-lookup"><span data-stu-id="cbb9b-203">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

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

#### <a name="response-2"></a><span data-ttu-id="cbb9b-204">响应 2</span><span class="sxs-lookup"><span data-stu-id="cbb9b-204">Response 2</span></span>

<span data-ttu-id="cbb9b-205">下面是第二个示例的响应，显示了扩展中更新的 `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="cbb9b-205">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
