---
title: 更新开放扩展
description: 通过请求正文中的属性更新开放扩展（openTypeExtension 对象）：
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 89804b1259f3832b2b69e2f62d25ac1fa8856809
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863689"
---
# <a name="update-open-extension"></a><span data-ttu-id="05536-103">更新开放扩展</span><span class="sxs-lookup"><span data-stu-id="05536-103">Update open extension</span></span>

<span data-ttu-id="05536-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05536-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05536-105">通过请求正文中的属性更新开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）：</span><span class="sxs-lookup"><span data-stu-id="05536-105">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="05536-106">如果请求正文中的属性与现有属性在扩展中的名称相匹配，则更新扩展中的数据。</span><span class="sxs-lookup"><span data-stu-id="05536-106">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="05536-107">否则，属性及其数据将添加到扩展中。</span><span class="sxs-lookup"><span data-stu-id="05536-107">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="05536-108">扩展插件中的数据可以是基元类型，也可以是基元类型数组。</span><span class="sxs-lookup"><span data-stu-id="05536-108">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="05536-109">权限</span><span class="sxs-lookup"><span data-stu-id="05536-109">Permissions</span></span>

<span data-ttu-id="05536-110">根据在其中创建扩展的资源以及请求的权限类型（委派或应用程序），下表中指定的权限是调用此 API 所需的最低特权。</span><span class="sxs-lookup"><span data-stu-id="05536-110">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="05536-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05536-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05536-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="05536-112">Supported resource</span></span> | <span data-ttu-id="05536-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05536-113">Delegated (work or school account)</span></span> | <span data-ttu-id="05536-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05536-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05536-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05536-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="05536-116">设备</span><span class="sxs-lookup"><span data-stu-id="05536-116">device</span></span>](../resources/device.md) | <span data-ttu-id="05536-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05536-117">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="05536-118">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-118">Not supported</span></span> | <span data-ttu-id="05536-119">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-119">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="05536-120">事件</span><span class="sxs-lookup"><span data-stu-id="05536-120">event</span></span>](../resources/event.md) | <span data-ttu-id="05536-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="05536-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-122">Calendars.ReadWrite</span></span> | <span data-ttu-id="05536-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-123">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="05536-124">组</span><span class="sxs-lookup"><span data-stu-id="05536-124">group</span></span>](../resources/group.md) | <span data-ttu-id="05536-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="05536-126">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-126">Not supported</span></span> | <span data-ttu-id="05536-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-127">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="05536-128">组事件</span><span class="sxs-lookup"><span data-stu-id="05536-128">group event</span></span>](../resources/event.md) | <span data-ttu-id="05536-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="05536-130">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-130">Not supported</span></span> | <span data-ttu-id="05536-131">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-131">Not supported</span></span> |
| [<span data-ttu-id="05536-132">组帖子</span><span class="sxs-lookup"><span data-stu-id="05536-132">group post</span></span>](../resources/post.md) | <span data-ttu-id="05536-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-133">Group.ReadWrite.All</span></span> | <span data-ttu-id="05536-134">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-134">Not supported</span></span> | <span data-ttu-id="05536-135">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-135">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="05536-136">邮件</span><span class="sxs-lookup"><span data-stu-id="05536-136">message</span></span>](../resources/message.md) | <span data-ttu-id="05536-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-137">Mail.ReadWrite</span></span> | <span data-ttu-id="05536-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-138">Mail.ReadWrite</span></span> | <span data-ttu-id="05536-139">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-139">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="05536-140">组织</span><span class="sxs-lookup"><span data-stu-id="05536-140">organization</span></span>](../resources/organization.md) | <span data-ttu-id="05536-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-141">Organization.ReadWrite.All</span></span> | <span data-ttu-id="05536-142">不支持</span><span class="sxs-lookup"><span data-stu-id="05536-142">Not supported</span></span> | <span data-ttu-id="05536-143">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-143">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="05536-144">个人联系人</span><span class="sxs-lookup"><span data-stu-id="05536-144">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="05536-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="05536-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-146">Contacts.ReadWrite</span></span> | <span data-ttu-id="05536-147">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-147">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="05536-148">用户</span><span class="sxs-lookup"><span data-stu-id="05536-148">user</span></span>](../resources/user.md) | <span data-ttu-id="05536-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-149">User.ReadWrite</span></span> | <span data-ttu-id="05536-150">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05536-150">User.ReadWrite</span></span> | <span data-ttu-id="05536-151">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05536-151">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05536-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05536-152">HTTP request</span></span>
<span data-ttu-id="05536-153">在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `PATCH`。</span><span class="sxs-lookup"><span data-stu-id="05536-153">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
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

><span data-ttu-id="05536-p102">**注意：** 以上语法显示一些标识资源实例的常见方法，以便在其中更新一个扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式在其中更新开放扩展。</span><span class="sxs-lookup"><span data-stu-id="05536-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="05536-156">若要了解如何在请求正文中添加任意自定义数据来进行更改或添加到扩展插件，请参阅[请求正文](#request-body)部分。</span><span class="sxs-lookup"><span data-stu-id="05536-156">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="05536-157">路径参数</span><span class="sxs-lookup"><span data-stu-id="05536-157">Path parameters</span></span>
|<span data-ttu-id="05536-158">参数</span><span class="sxs-lookup"><span data-stu-id="05536-158">Parameter</span></span>|<span data-ttu-id="05536-159">类型</span><span class="sxs-lookup"><span data-stu-id="05536-159">Type</span></span>|<span data-ttu-id="05536-160">说明</span><span class="sxs-lookup"><span data-stu-id="05536-160">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="05536-161">id</span><span class="sxs-lookup"><span data-stu-id="05536-161">id</span></span>|<span data-ttu-id="05536-162">string</span><span class="sxs-lookup"><span data-stu-id="05536-162">string</span></span>|<span data-ttu-id="05536-p103">相应集合的实例的唯一标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="05536-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="05536-165">extensionId</span><span class="sxs-lookup"><span data-stu-id="05536-165">extensionId</span></span>|<span data-ttu-id="05536-166">string</span><span class="sxs-lookup"><span data-stu-id="05536-166">string</span></span>|<span data-ttu-id="05536-p104">这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。</span><span class="sxs-lookup"><span data-stu-id="05536-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="05536-170">请求标头</span><span class="sxs-lookup"><span data-stu-id="05536-170">Request headers</span></span>
| <span data-ttu-id="05536-171">名称</span><span class="sxs-lookup"><span data-stu-id="05536-171">Name</span></span>       | <span data-ttu-id="05536-172">值</span><span class="sxs-lookup"><span data-stu-id="05536-172">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="05536-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="05536-173">Authorization</span></span> | <span data-ttu-id="05536-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05536-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05536-176">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05536-176">Content-Type</span></span> | <span data-ttu-id="05536-177">application/json</span><span class="sxs-lookup"><span data-stu-id="05536-177">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="05536-178">请求正文</span><span class="sxs-lookup"><span data-stu-id="05536-178">Request body</span></span>

<span data-ttu-id="05536-p106">提供 [openTypeExtension](../resources/opentypeextension.md) 对象的 JSON 正文（具有以下所需的名称-值对）以及要更改或添加到该扩展中的任意定义数据。JSON 负载中的数据可以是基元或基元数组类型。</span><span class="sxs-lookup"><span data-stu-id="05536-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="05536-181">名称</span><span class="sxs-lookup"><span data-stu-id="05536-181">Name</span></span>       | <span data-ttu-id="05536-182">值</span><span class="sxs-lookup"><span data-stu-id="05536-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="05536-183">@odata.type</span><span class="sxs-lookup"><span data-stu-id="05536-183">@odata.type</span></span> | <span data-ttu-id="05536-184">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="05536-184">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="05536-185">extensionName</span><span class="sxs-lookup"><span data-stu-id="05536-185">extensionName</span></span> | <span data-ttu-id="05536-186">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="05536-186">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="05536-187">响应</span><span class="sxs-lookup"><span data-stu-id="05536-187">Response</span></span>

<span data-ttu-id="05536-188">如果成功，此方法返回 `200 OK` 响应代码和更新的 [openTypeExtension](../resources/opentypeextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05536-188">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="05536-189">示例</span><span class="sxs-lookup"><span data-stu-id="05536-189">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="05536-190">请求 1</span><span class="sxs-lookup"><span data-stu-id="05536-190">Request 1</span></span>

<span data-ttu-id="05536-p107">第一个示例展示如何在邮件中更新扩展。该扩展最初由以下 JSON 负载表示：</span><span class="sxs-lookup"><span data-stu-id="05536-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="05536-193">可以按其名称引用该扩展，</span><span class="sxs-lookup"><span data-stu-id="05536-193">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="05536-194">或者，也可以通过其完全限定的名称引用扩展：</span><span class="sxs-lookup"><span data-stu-id="05536-194">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="05536-195">可以通过以下方法，使用示例请求和以下请求正文更新以上扩展：</span><span class="sxs-lookup"><span data-stu-id="05536-195">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="05536-196">将 `companyName` 从 `Wingtip Toys` 更改为 `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="05536-196">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="05536-197">将 `dealValue` 从 `500050` 更改为 `500100`</span><span class="sxs-lookup"><span data-stu-id="05536-197">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="05536-198">将新数据添加为自定义属性 `updated`</span><span class="sxs-lookup"><span data-stu-id="05536-198">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="05536-199">响应 1</span><span class="sxs-lookup"><span data-stu-id="05536-199">Response 1</span></span>

<span data-ttu-id="05536-200">无论用于引用扩展的方式如何，该响应都相同。</span><span class="sxs-lookup"><span data-stu-id="05536-200">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
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

#### <a name="request-2"></a><span data-ttu-id="05536-201">请求 2</span><span class="sxs-lookup"><span data-stu-id="05536-201">Request 2</span></span>

<span data-ttu-id="05536-p108">第二个示例展示如何在组帖子中更新扩展。该扩展最初由以下 JSON 负载表示，其中的 `expirationDate` 的值为 `2015-07-03T13:04:00Z`</span><span class="sxs-lookup"><span data-stu-id="05536-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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

<span data-ttu-id="05536-204">以下是要将 `expirationDate` 更改为 `2016-07-30T11:00:00Z` 的请求和请求正文：</span><span class="sxs-lookup"><span data-stu-id="05536-204">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"],
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
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

#### <a name="response-2"></a><span data-ttu-id="05536-205">响应 2</span><span class="sxs-lookup"><span data-stu-id="05536-205">Response 2</span></span>

<span data-ttu-id="05536-206">下面是第二个示例的响应，显示了扩展中更新的 `expirationDate`</span><span class="sxs-lookup"><span data-stu-id="05536-206">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "ignored",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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
