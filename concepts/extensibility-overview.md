---
title: 使用扩展向资源添加自定义数据
description: 可以使用自己的应用程序数据扩展 Microsoft Graph。 添加用于在 Microsoft Graph 资源中存储自定义数据的自定义属性，而无需外部数据存储。
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: a7d2a2eeba27877afe5c1aba4fbc416ad10d48c9
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856111"
---
# <a name="add-custom-data-to-resources-using-extensions"></a>使用扩展向资源添加自定义数据

Microsoft Graph 提供单个 API 终结点，以通过 [用户](/graph/api/resources/user) 和 [消息](/graph/api/resources/message) 等资源访问以人为本的丰富数据和见解。 还可以通过将自定义属性添加到资源实例来扩展 Microsoft Graph，而无需使用外部数据存储。

在本文中，我们将讨论 Microsoft Graph 如何支持扩展其资源、添加自定义属性的可用选项，以及何时使用它们。

> [!IMPORTANT]
> 请勿使用扩展存储敏感的个人身份信息，例如帐户凭据、政府标识号、持卡人数据、财务帐户数据、医疗保健信息或敏感的背景信息。

## <a name="why-add-custom-properties-to-microsoft-graph"></a>为什么要将自定义属性添加到 Microsoft Graph？

> [!IMPORTANT]
> 不应使用扩展存储敏感的个人身份信息，例如帐户凭据、政府标识号、持卡人数据、财务帐户数据、医疗保健信息或敏感的背景信息。
* 作为 ISV 开发人员，你可能会决定通过扩展 **用户** 资源，让应用处于轻量级水平，并将特定于应用的用户配置文件数据存储在 Microsoft Graph 中。
* 或者，你可能想要保留应用的现有用户配置文件存储，并将特定于应用的标识符添加到 **用户** 资源。
* 作为企业开发人员，你生成的内部应用程序可能依赖于组织的 HR 特定数据。 可以通过将此数据存储在 Microsoft Graph 的自定义属性中来简化多个应用程序中的集成。

## <a name="custom-property-options-in-microsoft-graph"></a>Microsoft Graph 中的自定义属性选项

Microsoft Graph 提供四种类型的扩展，用于添加自定义属性。

- 扩展属性特性
- 目录 (Azure AD) 扩展
- 架构扩展
- 开放扩展

### <a name="extension-attributes"></a>扩展属性

Azure AD 在 [用户](/graph/api/resources/onpremisesextensionattributes) 和 [设备](/graph/api/resources/onpremisesextensionattributes) 资源上提供一组 15 个具有预定义名称的自定义属性。 这些属性最初是在本地 Active Directory (AD) 和 Microsoft Exchange 中提供的自定义属性。 但现在其用途已不仅限于通过 Microsoft Graph 将本地 AD 和 Microsoft Exchange 数据同步到 Azure AD。

#### <a name="developer-experience"></a>开发者体验

可以使用这 15 个属性分别通过 **onPremisesExtensionAttributes** 和 **extensionAttributes** 属性在 **用户** 或 **设备** 资源实例上存储字符串值。 在创建新资源实例或更新现有资源实例时，可以分配这些值。 还可以对它们进行筛选。

##### <a name="add-or-update-data-in-extension-attributes"></a>在扩展属性中添加或更新数据

下面的示例演示如何使用 PATCH 方法通过更新操作将数据存储在 **extensionAttribute1** 中，以及如何从 **extensionAttribute12** 中删除现有数据。

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b

{
    "onPremisesExtensionAttributes": {
        "extensionAttribute1": "skypeId.adeleVance",
        "extensionAttribute13": null
    }
}
```

请求会返回 `204 No Content` 响应对象。

##### <a name="retrieve-data-from-extension-attributes-1-15"></a>从扩展属性 1-15 中检索数据

###### <a name="request"></a>请求

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,displayName,onPremisesExtensionAttributes
```

###### <a name="response"></a>响应

```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,onPremisesExtensionAttributes)",
    "value": [
        {
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "displayName": "Adele Vance",
            "onPremisesExtensionAttributes": {
                "extensionAttribute1": "Contractor",
                "extensionAttribute2": "50",
                "extensionAttribute3": null,
                "extensionAttribute4": "1478354",
                "extensionAttribute5": "10239390",
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": "11",
                "extensionAttribute11": null,
                "extensionAttribute12": "/o=ExchangeLabs/ou=Exchange Administrative Group (FYDIBOHF47SPDLT)/cn=Recipients/cn=5ee781fc7egc7aa0b9394bddb44e7f04-Adele Vance",
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```

### <a name="directory-azure-ad-extensions"></a>目录 (Azure AD) 扩展

[目录扩展](/graph/api/resources/extensionProperty) 为开发人员提供了针对目录对象的强类型、可发现和可筛选的扩展体验。

目录扩展首先通过 [创建 extensionProperty](/graph/api/application-post-extensionproperty) 操作在应用程序上注册，并且必须明确针对特定目录对象。 在应用程序获得用户或管理员同意后，扩展属性将立即在租户中可以访问。 租户中的所有授权应用程序都可以读取和写入目标目录对象实例上定义的任何扩展属性上的数据。

有关可指定为目录扩展目标对象的资源类型的列表，请参阅 [为应用程序选择扩展类型](#choose-an-extension-type-for-your-application)。

#### <a name="developer-experience"></a>开发者体验

目录扩展定义通过 [extensionProperty](/graph/api/resources/extensionproperty) 资源及其关联的方法进行管理。 数据通过用于管理资源实例的相同 REST 请求进行管理。

##### <a name="create-a-directory-extension-definition"></a>创建目录扩展定义

必须先创建目录扩展定义，然后才能将目录扩展添加到资源实例。

###### <a name="request"></a>请求

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/applications/30a5435a-1871-485c-8c7b-65f69e287e7b/extensionProperties

{
    "name": "jobGroupTracker",
    "dataType": "String",
    "targetObjects": [
        "User"
    ]
}
```

###### <a name="response"></a>响应

使用遵循以下命名约定的扩展名创建名为 `extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker` 的目录扩展属性：*extension_{appId-without-hyphens}_{extensionProperty-name}*。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications('30a5435a-1871-485c-8c7b-65f69e287e7b')/extensionProperties/$entity",
    "id": "4e3dbc8f-ca32-41b4-825a-346215d7d20f",
    "deletedDateTime": null,
    "appDisplayName": "HR-sync-app",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "name": "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker",
    "targetObjects": [
        "User"
    ]
}
```

##### <a name="add-a-directory-extension-property-to-a-target-object"></a>将目录扩展属性添加到目标对象

创建目录扩展定义后，现在可以将其添加到目标对象类型的实例。 创建目标对象的新实例或更新现有对象时，可以将数据存储在目录扩展属性中。 下面的示例演示如何在创建新的用户对象时将数据存储在目录扩展属性中。

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "JobGroupN"
}
```

请求会在响应正文中返回 `201 Created` 响应代码和 [用户](/graph/api/resources/user)对象。

##### <a name="retrieve-a-directory-extension-property"></a>检索目录扩展属性

下面的示例演示如何在资源实例上显示目录扩展属性和关联的数据。 默认情况下，将通过 `beta` 终结点返回扩展属性，但仅在 `$select` 时通过 `v1.0` 终结点返回。

##### <a name="request"></a>请求

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable
```

##### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable)",
    "value": [
        {
            "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
            "displayName": "Adele Vance",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": true
        }
    ]
}
```

##### <a name="update-or-delete-directory-extension-properties"></a>更新或删除目录扩展属性

要更新或删除资源实例的目录扩展属性的值，请使用 PATCH 方法。 要从资源实例中删除扩展属性及其关联值，请将其值设置为 `null`。

以下请求会更新一个目录扩展属性的值并删除另一个扩展属性。

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/63384f56-42d2-4aa7-b1d6-b10c78f143a2

{
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": null,
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4"
}
```

请求会返回 `204 No Content` 响应代码。

### <a name="schema-extensions"></a>架构扩展

[Microsoft Graph 架构扩展](/graph/api/resources/schemaextension) 在概念上类似于目录扩展。 首先，创建架构扩展定义。 然后，使用它来扩展具有强类型自定义属性的受支持资源实例。 此外，还可以控制架构扩展的[状态](/graph/api/resources/schemaextension#schema-extensions-lifecycle)，让它可被其他应用发现。

有关支持架构扩展的资源类型的列表，请参阅 [为应用程序选择扩展类型](#choose-an-extension-type-for-your-application)。

> [!VIDEO https://www.youtube-nocookie.com/embed/3MOAlUFNus0]

#### <a name="developer-experience"></a>开发者体验

在创建架构扩展定义时，你必须提供其 **id** 的唯一名称。提供两个命名选项：

- 如果已有通过租户验证的 `.com`、`.net`、`.gov`、`.edu` 或 `.org` 虚域，则可以使用域名和架构名称来定义唯一名称，格式如下：*{domainName}* _ *{schemaName}*。 例如，如果虚域为 `contoso.com`，则可以定义 `contoso_mySchema` 的 **ID**。 强烈建议使用此选项。
- 如果没有经过验证的虚域，则可以将 **ID** 设置为架构名称（不带域名前缀）。 例如，`mySchema`。 根据所提供的名称，Microsoft Graph 将为你分配一个字符串 ID，采用以下格式：`ext{8-random-alphanumeric-chars}_{schema-name}`。 例如，`extkvbmkofy_mySchema`。

**ID** 将是将数据存储在扩展资源实例上的复杂类型的名称。

注册架构扩展后，可以由与关联的所有者应用程序位于同一租户中的所有应用程序（处于 `InDevelopment` 状态）或任何租户中的所有应用程序（处于 `Available` 状态时）使用。 与目录扩展一样，授权应用可以读取和写入目标对象上定义的任何扩展上的数据。

与开放扩展不同，可将扩展资源实例上的 [架构扩展定义](/graph/api/resources/schemaextension) 及其数据作为单独的 API 操作集进行管理。 要管理扩展资源实例上的架构扩展数据，请使用你用于管理资源实例的同一 REST 请求。

##### <a name="create-a-schema-extension-definition"></a>创建架构扩展定义

###### <a name="request"></a>请求

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/schemaExtensions

{
    "id": "graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

###### <a name="response"></a>响应

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#schemaExtensions/$entity",
    "id": "extkmpdyld2_graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "status": "InDevelopment",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="add-a-schema-extension-to-a-resource-instance"></a>将架构扩展添加到资源实例

创建架构扩展定义后，现在可以将扩展属性添加到目标对象类型的实例。 在创建目标对象的新实例或更新现有对象时，可以将数据存储在架构扩展中。 下面的示例演示如何在创建新的用户对象时将数据存储在架构扩展属性中。

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@m365x72712789.onmicrosoft.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extkmpdyld2_graphLearnCourses": {
        "courseId": 100,
        "courseName": "Explore Microsoft Graph",
        "courseType": "Online"
    }
}
```

请求会在响应正文中返回 `201 Created` 响应代码和 [schemaExtension](/graph/api/resources/schemaextension) 对象

##### <a name="update-or-delete-a-schema-extension-property"></a>更新或删除架构扩展属性

使用 PATCH 操作更新架构扩展属性或删除现有架构扩展对象。 要从资源实例中删除扩展属性及其关联值，请将其值设置为 `null`。

以下示例删除 **courseId** 属性的值并更新 **courseType** 属性。 要完整删除 `extkmpdyld2_graphLearnCourses` 扩展属性，请将其值设置为 `null`。

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e

{
    "extkmpdyld2_graphLearnCourses": {
        "courseType": "Instructor-led",
        "courseId": null
    }
}
```

请求会返回 `204 No Content` 响应对象。

##### <a name="retrieve-the-schema-extension-property"></a>检索架构扩展属性

要读取资源实例上的架构扩展属性，请在 `$select` 请求中指定扩展名。

###### <a name="request"></a>请求
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e?$select=id,displayName,extkmpdyld2_graphLearnCourses
```

###### <a name="response"></a>响应
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,displayName,extkmpdyld2_graphLearnCourses)/$entity",
    "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
    "displayName": "Adele Vance",
    "extkmpdyld2_graphLearnCourses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseType": "Instructor-led",
        "courseName": "Explore Microsoft Graph",
        "courseId": null
    }
}
```

有关如何使用架构扩展添加自定义属性和关联数据的详细信息，请参阅 [schemaExtension 资源类型](/graph/api/resources/schemextension) 和 [使用架构扩展将自定义属性添加到组](extensibility-schema-groups.md)。

### <a name="open-extensions"></a>开放扩展

[Microsoft Graph 开放扩展](/graph/api/resources/opentypeextension) 是 [开放类型](https://www.odata.org/getting-started/advanced-tutorial/#openType) ，可提供一种简单灵活的方式将非类型化数据直接添加到资源实例。 这些扩展不是强类型、可发现或可筛选的。

有关支持 Microsoft Graph 开放扩展的资源类型的列表，请参阅 [为应用程序选择扩展类型](#choose-an-extension-type-for-your-application)。

> [!VIDEO https://www.youtube-nocookie.com/embed/ibdlADb8IZc]

#### <a name="developer-experience"></a>开发者体验

可通过资源实例的 **扩展** 导航属性访问开放扩展及其数据。 使用这些属性，可以对相关属性进行分组，以实现更轻松的访问和管理。

**extensionName** 属性是开放扩展中的 *预定义* 唯一可写属性。 创建开放扩展时，必须为 **extensionName** 属性分配在租户内唯一的名称。 为此，一种方法是使用反向域名系统 (DNS) 格式，此格式依赖 *用户自己的域*。例如，`Com.Contoso.ContactInfo`。 **不要在扩展名中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）**。

##### <a name="create-an-open-extension"></a>创建开放扩展

下面的示例演示了一个具有三个属性的开放扩展定义，以及如何在资源实例上显示自定义属性和关联数据。

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.socialSettings",
    "skypeId": "skypeId.AdeleV",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "xboxGamerTag": "AwesomeAdele",
    "id": "com.contoso.socialSettings"
}
```

请求会在响应正文中返回 `201 Created` 响应代码和 [openTypeExtension](/graph/api/resources/opentypeextension) 对象。

##### <a name="update-an-existing-open-extension"></a>更新现有开放扩展

要更新开放扩展，必须在请求正文中指定其所有属性。 否则，未指定的属性将更新为 `null` 并从开放扩展中删除。

以下请求仅指定 **linkedInProfile** 和 **xboxGamerTag** 属性。 **xboxGamerTag** 属性的值正在更新，而 **linkedInProfile** 属性将保持不变。 此请求还会删除未指定的 **skypeId** 属性。

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile"
}
```
此请求会返回 `204 No Content` 响应代码。


##### <a name="retrieve-the-open-extensions"></a>检索开放扩展

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('3fbd929d-8c56-4462-851e-0eb9a7b3a2a5')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "id": "com.contoso.socialSettings"
}
```

有关如何使用开放扩展添加自定义属性和关联数据的详细信息，请参阅 [openTypeExtension 资源类型](/graph/api/resources/opentypeextension) 和 [使用开放扩展将自定义属性添加到用户](extensibility-open-users.md)。

## <a name="choose-an-extension-type-for-your-application"></a>为应用程序选择扩展类型

下表对扩展类型进行了对比和比较，这应有助于确定最适合你的方案的选项。

| 功能 | 扩展属性 1-15 | 目录扩展 | 架构扩展 | 开放扩展 |
|--|--|--|--|--|
| 支持的资源类型 | [user][] <br/>[设备][] | [user][] <br/> [group][] [administrativeUnit][] <br/> [application][] <br/>[设备][] <br/> [组织][] | [用户][] <br/> [group][] [administrativeUnit][] <br/> [联系人][] <br/> [设备][] <br/> [事件][]（用户和组日历） <br/> [邮件][] <br/> [组织][] <br/> [帖子][] <br/> [todoTask][] <br/> [todoTaskList][] | [user][] <br/> [group][] <!--<br/> [administrativeUnit][]--> <br/> [联系人][] <br/> [设备][] <br/> [事件][] <sup>1</sup>（用户和组日历） <br/> [邮件][] <br/> [组织][] <br/> [帖子][] |
| 强类型 | 否 | 是 | 是 | 否 |
| Filterable | 是 | 是 | 是 | 否 |
| 管理方式 | Microsoft Graph <br/> Exchange 管理中心 | Microsoft Graph | Microsoft Graph | Microsoft Graph |
| 使用 [AD Connect][] 将数据从本地同步到扩展 | 是，对于用户 | [是][ADConnect-YES] | 否 | 否 |
| 使用自定义扩展属性和数据创建 [动态成员资格规则][]  | [是][DynamicMembership-YES] | [是][DynamicMembership-YES] | 否 | 否 |
| 可用于自定义令牌声明 | 是 | [是][DirectoryExt-CustomClaims] | 否 | 否 |
| 在 Azure AD B2C 中提供 | 是 | [是][B2CDirectoryExt] | 是 | 是 |
| 限制 | <li>每个用户或设备资源实例 15 个预定义属性 | <li>每个资源实例 100 个扩展值 | <li>每个所有者应用最多五个定义 <br/><li> 每个资源实例 100 个扩展值（仅限目录对象） | <li>每个资源实例每个创建者应用两个开放扩展<sup>2</sup> <br/><li> 最大 每个开放扩展 2Kb <sup>2</sup><li> 对于 Outlook 资源，每个开放扩展都存储在 [MAPI 命名属性][MAPI-named-property]<sup>3</sup> 中 |


> [!NOTE]
> 
> <sup>1</sup> 由于现有的服务限制，代理无法在共享邮箱日历中创建已追加开放扩展的事件。 尝试这样做将导致 `ErrorAccessDenied` 响应。
>
> <sup>2</sup> 对开放扩展的这些限制适用于以下目录资源：**用户**、**组**、**设备**， <!--**administrativeUnit**,--> 以及 **组织**。
>
> <sup>3</sup> 每个 [开放扩展](/graph/api/resources/opentypeextension) 都存储在 [MAPI 命名属性](/office/client-developer/outlook/mapi/mapi-named-properties) 中，该属性是用户邮箱中的有限资源。 此限制适用于以下 Outlook 资源：**邮件**、**事件** 和 **联系人**
>
> 使用工作或学校帐户登录时，可以管理所有扩展。 此外，使用个人 Microsoft 帐户登录时，可以管理以下资源的开放扩展：**事件**、**帖子**、**组**、**消息**、**联系人** 和 **用户**。

## <a name="permissions"></a>权限

还需要对特定资源执行读取或写入操作所需的相同[权限](./permissions-reference.md)，才能对相应资源上的任意扩展数据执行读取或写入操作。 例如，要让应用使用自定义应用数据更新任何用户的配置文件，必须已向应用授予 *User.ReadWrite.All* 权限。

## <a name="known-limitations"></a>已知限制

有关使用扩展的已知限制，请参阅已知问题文章中的[扩展部分](known-issues.md#extensions)。

## <a name="next-steps"></a>后续步骤

- [使用开放扩展向用户添加自定义数据](extensibility-open-users.md)
- [使用架构扩展向组添加自定义数据](extensibility-schema-groups.md)


<!-- Links -->

[user]: /graph/api/resources/user
[group]: /graph/api/resources/group
[contact]: /graph/api/resources/contact
[administrativeUnit]: /graph/api/resources/administrativeunit
[application]: /graph/api/resources/application
[设备]: /graph/api/resources/device
[事件]: /graph/api/resources/event
[邮件]: /graph/api/resources/message
[组织]: /graph/api/resources/organization
[帖子]: /graph/api/resources/post
[todoTask]: /graph/api/resources/todotask
[todoTaskList]: /graph/api/resources/todotasklist
[servicePrincipal]: /graph/api/resources/serviceprincipal
[AD connect]: /azure/active-directory/hybrid/whatis-hybrid-identity?context=/azure/active-directory/enterprise-users/context/ugr-context
[ADConnect-YES]: /azure/active-directory/hybrid/how-to-connect-sync-feature-directory-extensions
[动态成员资格规则]: /azure/active-directory/enterprise-users/groups-dynamic-membership
[DynamicMembership-YES]: /azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties
[DirectoryExt-CustomClaims]: /azure/active-directory/develop/active-directory-optional-claims#configuring-directory-extension-optional-claims
[B2CDirectoryExt]: /azure/active-directory-b2c/user-profile-attributes#extension-attributes
[MAPI-named-property]: /office/client-developer/outlook/mapi/mapi-named-properties