---
title: 使用 Microsoft Graph 中的配置文件 API 自定义配置文件卡片（预览）
description: 本文介绍如何通过显示其他属性来自定义配置文件卡片，或添加自定义属性。
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: dc0c78ecfdf00488c7c9c12969eea8b405be496c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050973"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a>使用 Microsoft Graph 中的配置文件 API 将其他属性添加到配置文件卡片（预览）

在 Microsoft 365 中的[配置文件卡片](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)中，可以找到组织存储和维护的用户的相关信息，例如**职务**或**办公室位置**。

使用[profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta)资源显示来自组织的配置文件卡上的 Azure AD 的其他属性，方法如下：

- 让其他属性可见

- 添加自定义属性

其他属性将显示在 Microsoft 365 的配置文件卡片的 "**联系人**" 部分中。

> [!NOTE]
>使用委派权限的**profileCardProperty**资源上的操作要求已登录用户拥有租户管理员或全局管理员角色。

## <a name="make-additional-attributes-visible"></a>使其他属性可见

你可以在用户配置文件卡上看到 Azure Active Directory （Azure AD）中的以下属性。 这些属性*不区分大小写*：

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

下表显示了 Azure AD 属性如何与 Microsoft Graph[用户](/graph/api/resources/user?view=graph-rest-beta)实体的属性相对应。

|Azure AD 属性 |User entity 属性|
|:---------------|:----------|
|UserPrincipalName|userPrincipalName |
|传真|faxNumber|
|StreetAddress|streetAddress|
|PostalCode|postalCode|
|StateOrProvince|状态
|Alias|mailNickname

您可以通过配置您的[组织设置](/graph/api/resources/organizationsettings?view=graph-rest-beta)并将属性添加为 Microsoft Graph 中**profileCardProperty**的*directoryPropertyName** 属性，将这些属性中的任何属性添加到配置文件卡片中。 当您使其他属性可见时，您必须使用的属性名称 `en-us` 。 您不必添加本地化的值。 其他属性将自动显示在用户为 Microsoft 365 指定的语言设置中。

> [!IMPORTANT]
> 将属性添加到配置文件卡片时，将需要长达24小时才能显示加法。

## <a name="example"></a>示例

下面的示例显示 `Alias` 配置文件卡片上的属性：

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

如果成功，响应会 `201 OK` 在响应正文中返回响应代码和**profileCardProperty**对象。 属性的值 `Alias` 将显示在用户的配置文件卡片上。  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>添加自定义属性

您可以通过配置组织设置并在 Microsoft Graph 中[将相应的值添加为 profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) ，将任何15个 Azure AD[自定义扩展属性](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)添加到用户的配置文件卡中。 您可以一次添加一个**profileCardProperty**资源。

需要长达24小时才能在配置文件卡片上显示所做的更改。

自定义属性不可搜索，且不能用于在 Microsoft 应用程序和服务中搜索人员。

下表显示了 Azure AD 自定义扩展属性名称如何对应于[profileCardProperty](/graph/api/resources/profilecardproperty?view=graph-rest-beta)资源的**directoryPropertyName**属性的受支持的值。 这些 Azure AD 自定义扩展属性名称*不区分大小写*：

|Azure AD 自定义扩展属性 | 要指定为 directoryPropertyName 的值 |
|:--------------------|:-----------------|
| extensionAttribute1 | customAttribute1 |
| extensionAttribute2 | customAttribute2 |
| extensionAttribute3 | customAttribute3 |
| extensionAttribute4 | customAttribute4 |
| extensionAttribute5 | customAttribute5 |
| extensionAttribute6 | customAttribute6 |
| extensionAttribute7 | customAttribute7 |
| extensionAttribute8 | customAttribute8 |
| extensionAttribute9 | customAttribute9 |
| extensionAttribute10 | customAttribute10 |
| extensionAttribute11 | customAttribute11 |
| extensionAttribute12 | customAttribute12 |
| extensionAttribute13 | customAttribute13 |
| extensionAttribute14 | customAttribute14 |
| extensionAttribute15 | customAttribute15 |

## <a name="example"></a>示例

下面的示例使用显示名称**成本中心**将第一个 Azure AD 自定义扩展属性添加到配置文件卡片中。 对于已将其语言设置设置为德语的用户，显示名称将为**Kostenstelle**。

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

如果语言不受支持，则将以默认值显示属性名称。  

如果成功，响应会 `201 OK` 在响应正文中返回响应代码和**profileCardProperty**对象。 在此示例中，您可以假定配置文件卡片显示了在配置文件卡片上将其语言设置为德语的所有用户的**Kostenstelle** 。 对于所有其他用户，**成本中心**将显示在配置文件卡片上。

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

[查找你的 Microsoft 365 租户 ID](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[onPremisesExtensionAttributes 资源类型](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[用户资源类型](/graph/api/resources/user?view=graph-rest-beta)

[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)

[获取 profileCardProperty](/graph/api/profilecardproperty-get?view=graph-rest-beta)
