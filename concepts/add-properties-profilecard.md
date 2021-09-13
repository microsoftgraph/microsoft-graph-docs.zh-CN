---
title: 使用 Microsoft Graph 中个人资料 API 自定义个人资料卡（预览版）
description: 本文介绍如何通过使其他属性可见或添加自定义属性来自定义个人资料卡。
author: PollyNincevic
ms.localizationpriority: high
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: a4d43cee6a2fb0d442a8dbf4db2f8283dc0c30be
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066966"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a>使用 Microsoft Graph 中的个人资料卡 API 向个人资料卡添加其他属性（预览版）

在 Microsoft 365 的 [个人资料卡](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)上，可以找到由组织存储和维护的有关用户的信息，例如 **职位名称** 或 **办公室位置**。

使用 [profileCardProperty](/graph/api/resources/profilecardproperty) 资源通过以下方式在组织的个人资料卡上显示Azure AD 的其他属性：

* 使其他属性可见
* 添加自定义属性

其他属性将显示在 Microsoft 365 中的个人资料卡的 **联系人** 部分中。

> [!NOTE]
> 在 **profileCardProperty** 资源上使用委派权限的操作要求登录的用户具有租户管理员或全局管理员角色。

## <a name="make-additional-attributes-visible"></a>使其他属性可见

可以在用户的个人资料卡片上显示 Azure Active Directory (Azure AD) 中的以下属性。这些属性 *不区分大小写*：

* `UserPrincipalName`
* `Fax`
* `StreetAddress`
* `PostalCode`
* `StateOrProvince`
* `Alias`

下表显示了Azure AD 属性如何与 Microsoft Graph [user](/graph/api/resources/user) 实体的属性相对应。

| Azure AD 属性 | 用户实体属性 |
| ------------------ | -------------------- |
| UserPrincipalName | userPrincipalName |
| Fax | faxNumber |
| StreetAddress | streetAddress |
| PostalCode | postalCode |
| StateOrProvince | state |
| Alias | mailNickname |

可以通过配置 [组织设置](/graph/api/resources/organizationsettings)并将此属性添加为 Microsoft Graph 中 **profileCardProperty** 的 **directoryPropertyName** 属性来将任何这些属性添加到个人资料卡片中。 当使其他属性可见时，必须使用 `en-us` 的属性名称。 不必添加本地化值。 其他属性将自动以用户为 Microsoft 365 指定的语言设置显示。

> [!IMPORTANT]
> 向个人资料卡添加属性时，最多需要 24 小时才能显示添加内容。

### <a name="example"></a>示例

以下示例在个人资料卡片上显示 `Alias` 属性。

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

如果成功，则响应在响应正文中返回 `201 OK` 响应代码和 **profileCardProperty** 对象。 `Alias` 属性的值将显示在用户的个人资料卡片上。

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>添加自定义属性

可以通过配置组织设置并在 Microsoft Graph 中 [将相应值添加为 profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties)，以将 15 个 Azure AD [自定义扩展属性](/graph/api/resources/onpremisesextensionattributes)中的任何一个属性添加到用户的个人资料卡片中。一次可以添加一个 **profileCardProperty** 资源。

所做的更改最多需要 24 小时才能显示在个人资料卡上。

自定义属性不可搜索，不能用于在 Microsoft 应用程序和服务中搜索人员。

下表显示了 Azure AD 自定义扩展属性名称如何与 [profileCardProperty](/graph/api/resources/profilecardproperty) 资源的 **directoryPropertyName** 属性支持的值对应。这些 Azure AD 自定义扩展属性名称 *不区分大小写*：

| Azure AD 自定义扩展属性 | 指定为 directoryPropertyName 的值 |
| ----------------------------------- | ----------------------------------------- |
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

### <a name="example"></a>示例

下面的示例使用显示名称 **成本中心** 将第一个 Azure AD 自定义扩展属性添加到个人资料卡。 对于将语言设置设置为德语的用户，显示名称将为 **Kostenstelle**。

``` http
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

如果语言不受支持，则将使用默认值显示属性名称。

如果成功，则响应在响应正文中返回 `201 OK` 响应代码和 **profileCardProperty** 对象。 在此示例中，你可以假设对于已在个人资料卡上将其语言设置为德语的所有用户，个人资料卡显示 **Kostenstelle**。 对于所有其他用户，**成本中心** 将显示在个人资料卡上。

``` http
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

- [查找 Microsoft 365 租户 ID](/onedrive/find-your-office-365-tenant-id)
- [onPremisesExtensionAttributes 资源类型](/graph/api/resources/onpremisesextensionattributes)
- [用户资源类型](/graph/api/resources/user)
- [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)
- [Get profileCardProperty](/graph/api/profilecardproperty-get)
