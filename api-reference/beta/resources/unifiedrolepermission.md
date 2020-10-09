---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa327935c4e3b45c28a0f7ae01ababeffe37d61d
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405223"
---
# <a name="unifiedrolepermission-resource-type"></a>unifiedRolePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示允许的资源操作的集合，以及操作有效时必须满足的条件。 资源操作是可在资源上 perfomed 的任务。 例如，应用程序资源支持创建、更新、删除和重置密码资源操作。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedResourceActions|字符串集合| 可在资源上 perfomed 的一组任务。 |
|表达式|字符串| 要使权限生效必须满足的可选约束。 |

### <a name="allowedresourceactions-property"></a>allowedResourceActions 属性

以下是资源操作的架构： 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
例如：`microsoft.directory/applications/credentials/update`。  

- 命名空间-公开任务的服务。 例如，Azure Active Directory 中的所有任务都使用命名空间 "microsoft."。  
- Entity-Microsoft Graph 中的服务公开的逻辑功能或组件。 例如，应用程序、服务主体或组。
- PropertySet-要为其授予访问权限的实体的特定属性或方面。 例如， `microsoft.directory/applications/authentication/read` 向 AZURE AD 中的 **application** 对象授予读取回复 URL、注销 url 和隐式流属性的功能。 以下是常用属性集的保留名称：  
  - allProperties-指定实体的所有属性，包括特权属性。 示例包括 `microsoft.directory/applications/allProperties/read` 和 `microsoft.directory/applications/allProperties/update` 。
  - basic-指定常见的读取属性，但不包括特权。 例如， `microsoft.directory/applications/basic/update` 包括更新显示名称等标准属性的功能。
  - standard-指定通用更新属性，但不包括特权文件。 例如，`microsoft.directory/applications/standard/read`。
- 操作-要授予的操作。 在大多数情况下，应根据 CRUD 或 allTasks 表示权限。 操作包括：
  - 创建-创建实体的新实例的功能。
  - Read-读取给定属性集 (包括 allProperties) 的功能。
  - Update-更新给定属性集 (包括 allProperties) 的功能。
  - 删除-删除给定实体的功能。
  - AllTasks-表示 (创建、读取、更新和删除) 的所有 CRUD 操作。 

### <a name="condition-property"></a>condition 属性
条件定义必须满足的约束。 例如，要求主体是目标的 "所有者"。 以下是受支持的条件：

- Self： "@Subject = = @Resource objectId"
- Owner： "@Subject Any_of @Resource 所有者"

下面是具有条件的角色权限的一个示例。

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>另请参阅

- [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) -用于有关内置目录角色的权限的信息。
- [Azure Active Directory 中的应用程序注册子类型和权限](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -有关可用于自定义目录角色的权限的信息。 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->