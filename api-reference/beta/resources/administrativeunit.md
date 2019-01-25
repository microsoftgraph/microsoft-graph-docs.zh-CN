---
title: administrativeUnit 资源类型
description: 一个管理单元的用户和组目录对象提供的概念的容器。 公司管理员使用管理单元，现在可以委托管理责任管理用户和组中包含或范围为一个区域或部门管理员对一个管理单元。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f99fb1cd54e28aaa9526f25a0f8e09d6470df2ff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519743"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个管理单元的用户和组目录对象提供的概念的容器。 公司管理员使用管理单元，现在可以委托管理责任管理用户和组中包含或范围为一个区域或部门管理员对一个管理单元。

请看示例。 假设 Contoso Corp 由构成的两个部门-西海岸部门和东海岸除法。 Contoso 目录角色作用于整个租户。 李，Contoso 公司管理员，希望将管理责任委派但到西海岸部门或东海岸部门范围它们。  李可以创建*西海岸 admistrative 单位*，并将所有西海岸用户都放到此管理单元。  同样，李可以创建一个*东海岸管理单元*。  现在李，可以开始委派管理责任向其他人，但为新的管理单位**范围**他创建。 李将以下放在*服务台管理员*角色**范围**对*西海岸管理单元*中。  这样，以下*西海岸管理单元*中这些用户时重置任何用户的密码，但仅。  同样，李置于 Dave*用户帐户管理员*角色**范围**对*东海岸管理单元*。  这样，Dave 来更新用户、 分配许可证和重置任何用户的密码，但如果这些用户是*东海岸管理单元*中。 有关的视频的概述，请参阅[Introduction to Azure Active Directory 管理单位](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。

通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。

本主题提供的声明的属性和导航属性公开的 administrativeUnit 实体，以及操作和可对 administrativeUnits 资源调用的函数的说明。


## <a name="methods"></a>方法

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建 administrativeUnit](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 创建一个新的管理单元。|
|[列表 administrativeUnits](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md)集合 |列出所有 administrativeUnits 的属性。|
|[Get administrativeUnit](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |读取属性和特定 administrativeUnit 对象的关系。|
|[更新 adminstrativeUnit](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |更新 administrativeUnit 对象。 |
|[删除 adminstrativeUnit](../api/administrativeunit-delete.md) | 无 |删除 administrativeUnit 对象。 |
|[添加成员](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| 添加成员 （用户或组）。|
|[List members](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) 集合| 获取 （用户和组） 的成员的列表。|
|[获取成员](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 获取特定成员。|
|[删除成员](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| 删除成员|
|[添加范围角色成员](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 添加的作用域角色成员。|
|[列表范围内的角色成员](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) 集合| 获取作用域角色管理员的列表。|
|[要获取的作用域角色成员](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 获取特定范围内的角色成员。|
|[删除的作用域角色成员](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 删除范围角色成员身份。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|description|string|管理单元的可选说明。|
|displayName|string|管理单元的显示名称。|
|id|字符串|管理单元的唯一标识符。 只读。|
|visibility|string|控制是否隐藏管理单元和及其成员或公共。 可以设置为 HiddenMembership 或公共。 如果不设置，默认行为是公共。 如果设置为 HiddenMembership，只有管理单元的成员可以列出管理单元中的其他成员。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|打开扩展名为此管理单元定义的集合。 可为 Null。|
|members|[directoryObject](directoryobject.md) 集合|用户和组成员的此 Adminsitrative 单位。 HTTP 方法： 获取 （列表成员），POST （添加成员），删除 （删除成员）。|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) 集合| 此管理单元的作用域角色成员。  HTTP 方法： 获取 (列表 scopedRoleMemberships)，POST （添加 scopedRoleMembership），请删除 (删除 scopedRoleMembership)。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/administrativeunit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
