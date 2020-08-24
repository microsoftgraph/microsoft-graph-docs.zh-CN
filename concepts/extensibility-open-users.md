---
title: 使用开放扩展向用户添加自定义数据
description: '本文将通过一个示例逐步介绍如何使用*开放扩展*。 '
author: dkershaw10
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 81c1d77ecc2e57dec9ae18bf298d7390b71651dc
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849091"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="3619e-103">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3619e-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="3619e-104">本文将通过一个示例逐步介绍如何使用*开放扩展*。</span><span class="sxs-lookup"><span data-stu-id="3619e-104">This article walks you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="3619e-p101">假设你正在构建一个可在许多不同客户端平台（例如桌面和移动设备）上使用的应用程序。你希望让用户配置自己的 UI 体验，这样无论用户使用何种设备登录你的应用都能获得相同的体验。这是对大多数应用的常见要求。</span><span class="sxs-lookup"><span data-stu-id="3619e-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="3619e-108">在此情况下，本文将介绍如何：</span><span class="sxs-lookup"><span data-stu-id="3619e-108">For this scenario, this article will show you how to:</span></span>

1. <span data-ttu-id="3619e-109">添加代表有关用户的一些漫游配置文件信息的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="3619e-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="3619e-110">查询用户并返回漫游配置文件。</span><span class="sxs-lookup"><span data-stu-id="3619e-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="3619e-111">更改用户的漫游配置文件信息（开放扩展值）。</span><span class="sxs-lookup"><span data-stu-id="3619e-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="3619e-112">删除用户的漫游配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="3619e-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="3619e-p102">**注意：** 本主题介绍如何在 **user** 资源上添加、读取、更新和删除开放扩展。**administrativeUnit**、**contact**、**device**、**event**、**group**、**organizaton**、**post**、**todoTask** 和 **todoTaskList** 资源类型也支持这些方法。</span><span class="sxs-lookup"><span data-stu-id="3619e-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a **user** resource. These methods are also supported for the **administrativeUnit**, **contact**, **device**, **event**, **group**, **organizaton**, **post**, **todoTask**, and **todoTaskList** resource types.</span></span>  
<span data-ttu-id="3619e-115">可以使用其中任一资源更新请求示例。</span><span class="sxs-lookup"><span data-stu-id="3619e-115">You can update the request examples using any of those resource types.</span></span> <span data-ttu-id="3619e-116">示例中显示的响应可能会被缩短以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="3619e-116">The responses shown in the examples might be shortened for readability.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="3619e-117">1.添加漫游配置文件信息</span><span class="sxs-lookup"><span data-stu-id="3619e-117">1. Add roaming profile information</span></span>
<span data-ttu-id="3619e-p104">用户登录到应用并配置应用的外观。这些应用设置应可以漫游，这样用户不管从何种设备登录应用都可以获得相同的体验。在这里，我们将了解如何将漫游配置文件信息添加到用户资源。</span><span class="sxs-lookup"><span data-stu-id="3619e-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

### <a name="request"></a><span data-ttu-id="3619e-121">请求</span><span class="sxs-lookup"><span data-stu-id="3619e-121">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
### <a name="response"></a><span data-ttu-id="3619e-122">响应</span><span class="sxs-lookup"><span data-stu-id="3619e-122">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="3619e-123">2.检索漫游配置文件信息</span><span class="sxs-lookup"><span data-stu-id="3619e-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="3619e-p105">当用户从其他设备登录应用时，该应用可以检索用户配置文件详细信息及其漫游设置。这可以通过获取用户的资源，以及对扩展导航属性进行扩展的方式完成。</span><span class="sxs-lookup"><span data-stu-id="3619e-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

### <a name="request"></a><span data-ttu-id="3619e-126">请求</span><span class="sxs-lookup"><span data-stu-id="3619e-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
### <a name="response"></a><span data-ttu-id="3619e-127">响应</span><span class="sxs-lookup"><span data-stu-id="3619e-127">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
><span data-ttu-id="3619e-128">**注意：** 如果你有多个扩展，则可以按 **ID** 筛选，以获取感兴趣的扩展。</span><span class="sxs-lookup"><span data-stu-id="3619e-128">**Note:** If you have multiple extensions, you can filter on the **id** to get the extension that you're interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="3619e-129">3.更改漫游配置文件信息</span><span class="sxs-lookup"><span data-stu-id="3619e-129">3. Change roaming profile information</span></span>
<span data-ttu-id="3619e-p106">用户可以选择更改其漫游配置文件信息。此更新可以通过开放扩展值上的 ```PATCH``` 完成。</span><span class="sxs-lookup"><span data-stu-id="3619e-p106">The user can choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

### <a name="request"></a><span data-ttu-id="3619e-132">请求</span><span class="sxs-lookup"><span data-stu-id="3619e-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

### <a name="response"></a><span data-ttu-id="3619e-133">响应</span><span class="sxs-lookup"><span data-stu-id="3619e-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="3619e-134">4.删除用户漫游配置文件</span><span class="sxs-lookup"><span data-stu-id="3619e-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="3619e-p107">用户决定不再使用漫游配置文件，因此将其删除。这可以通过开放扩展值上的 ```DELETE``` 请求完成。</span><span class="sxs-lookup"><span data-stu-id="3619e-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

### <a name="request"></a><span data-ttu-id="3619e-137">请求</span><span class="sxs-lookup"><span data-stu-id="3619e-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

### <a name="response"></a><span data-ttu-id="3619e-138">响应</span><span class="sxs-lookup"><span data-stu-id="3619e-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="3619e-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3619e-139">See also</span></span>

- [<span data-ttu-id="3619e-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3619e-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="3619e-141">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3619e-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="3619e-142">openTypeExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="3619e-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="3619e-143">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="3619e-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="3619e-144">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="3619e-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="3619e-145">更新开放扩展</span><span class="sxs-lookup"><span data-stu-id="3619e-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="3619e-146">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="3619e-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
