---
title: 使用开放扩展向用户添加自定义数据
description: 按照本示例中的步骤添加扩展、查询用户并返回漫游配置文件、更改和删除用户的漫游配置文件信息。
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: a94fd34daff722c0fd32bd271618626db1f50cec
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556190"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>使用开放扩展向用户添加自定义数据
本文将通过一个示例逐步介绍如何使用 *开放扩展*。 

假设你正在构建一个可在许多不同客户端平台（例如桌面和移动设备）上使用的应用程序。你希望让用户配置自己的 UI 体验，这样无论用户使用何种设备登录你的应用都能获得相同的体验。这是对大多数应用的常见要求。 

在此情况下，本文将介绍如何：

1. 添加代表有关用户的一些漫游配置文件信息的开放扩展。
2. 查询用户并返回漫游配置文件。
3. 更改用户的漫游配置文件信息（开放扩展值）。
4. 删除用户的漫游配置文件信息。

> [!NOTE]
> 本主题介绍如何在 **用户** 资源上添加、读取、更新、删除开放扩展。 开放扩展也受支持，可以针对[其他资源类型](extensibility-overview.md)进行管理。

## <a name="1-add-roaming-profile-information"></a>1.添加漫游配置文件信息
用户登录到应用并配置应用的外观。这些应用设置应可以漫游，这样用户不管从何种设备登录应用都可以获得相同的体验。在这里，我们将了解如何将漫游配置文件信息添加到用户资源。

### <a name="request"></a>请求
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
### <a name="response"></a>响应
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a>2.检索漫游配置文件信息
当用户从其他设备登录应用时，该应用可以检索用户配置文件详细信息及其漫游设置。这可以通过获取用户的资源，以及对扩展导航属性进行扩展的方式完成。

### <a name="request"></a>请求
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
### <a name="response"></a>响应
```http
HTTP/1.1 200 OK
Content-Type: application/json

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

> [!NOTE]
> 如果你有多个扩展，则可以按 **ID** 筛选，以获取感兴趣的扩展。

## <a name="3-change-roaming-profile-information"></a>3.更改漫游配置文件信息
用户可以选择更改其漫游配置文件信息。此更新可以通过开放扩展值上的 ```PATCH``` 完成。 

### <a name="request"></a>请求
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

### <a name="response"></a>响应
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a>4.删除用户漫游配置文件
用户决定不再使用漫游配置文件，因此将其删除。这可以通过开放扩展值上的 ```DELETE``` 请求完成。

### <a name="request"></a>请求
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

### <a name="response"></a>响应
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](extensibility-overview.md)
- [使用架构扩展向组添加自定义数据](extensibility-schema-groups.md)
- [openTypeExtension 资源类型](/graph/api/resources/opentypeextension)
- [创建开放扩展](/graph/api/opentypeextension-post-opentypeextension)
- [获取开放扩展](/graph/api/opentypeextension-get)
- [更新开放扩展](/graph/api/opentypeextension-update)
- [删除开放扩展](/graph/api/opentypeextension-delete)
