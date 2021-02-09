---
title: profileCardProperty 资源类型
description: 用于指定要以共享、人员体验显示的新属性或将应用自定义显示名称或批注的属性。 管理员可以定义一个默认显示名称字符串和一组替代翻译，供他们在组织中支持的语言使用。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 33d2b1111580ba2302848ab1dbce3f773055a0b4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153562"
---
# <a name="profilecardproperty-resource-type"></a>profileCardProperty 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示组织在 Microsoft 365 个人资料卡上显示共享人员体验的用户属性。

该属性可以是 Azure Active Directory (Azure AD) 内置属性（如 `Alias` or）或自定义 `UserPrincipalName` 属性。 对于自定义属性，管理员可以定义一个默认显示名称字符串和一组替代翻译，用于他们在组织中支持 `en-us` 的语言。

有关向组织的配置文件卡添加属性详细信息，请参阅 [自定义配置文件卡片](/graph/add-properties-profilecard)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [List](../api/organizationsettings-list-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | 获取组织的 **profileCardProperty** 资源的集合。 |
| [创建](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | 为组织 **创建新的 profileCardProperty** 资源。 |
| [Get](../api/profilecardproperty-get.md) | [profileCardProperty](profilecardproperty.md) | 读取 **profileCardProperty** 资源的属性和关系，其中包含给定字段的 Microsoft 365 组织中存在的配置文件卡自定义项。 |
| [更新](../api/profilecardproperty-update.md)               | [profileCardProperty](profilecardproperty.md) | 更新 **profileCardProperty** 对象。                               |
| [删除](../api/profilecardproperty-delete.md)               | 无                                          | 删除 **profileCardProperty** 对象。                               |

## <a name="properties"></a>属性

| 属性             | 类型                                                        | 说明 |
|:---------------------|:------------------------------------------------------------|:------------|
|批注           |[profileCardAnnotation](profilecardannotation.md) 集合 | 允许管理员为目录属性设置自定义显示标签，并针对租户中的用户进行本地化。|
|directoryPropertyName |String                                                       | 标识 **获取、更新或删除操作中的 profileCardProperty** [资源。](../api/profilecardproperty-delete.md) [](../api/profilecardproperty-get.md) [](../api/profilecardproperty-update.md) 允许管理员在其租户内的 Microsoft 365 (Azure AD) 显示隐藏的 Azure Active Directory 属性。 存在此状态时，此字段中引用的 Azure AD 字段将在个人资料卡片的联系人窗格上对租户中的所有用户可见。 此字段允许的值是： `UserPrincipalName` ， `Fax` ， ， ， `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1`  `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` 。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty"
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

