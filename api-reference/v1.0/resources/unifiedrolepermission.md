---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
ms.localizationpriority: medium
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 66c28bff1d6204dbe1a19a75bf1b9c47de6b502e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671400"
---
# <a name="unifiedrolepermission-resource-type"></a>unifiedRolePermission 资源类型

命名空间：microsoft.graph

表示允许的资源操作的集合以及允许操作必须满足的条件。 资源操作是可在资源上执行的任务。 例如，应用程序资源可能支持创建、更新、删除和重置密码操作。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedResourceActions|字符串集合| 可在资源上执行的任务集。 必填。 |
|条件|String| 为使权限有效，必须满足的可选约束。 |
|excludedResourceActions|String collection| 可能未在资源上执行的任务集。 尚不支持。 |

### <a name="allowedresourceactions-property"></a>allowedResourceActions 属性

下面是资源操作的架构： 

```
{Namespace}/{Entity}/{PropertySet}/{Action}  
```
例如：`microsoft.directory/applications/credentials/update`。  

- *{Namespace}* - 公开任务的服务。 例如，Azure Active Directory 中的所有任务都使用命名空间 `microsoft.directory`。  
- *{Entity}* - Microsoft Graph 中服务公开的逻辑功能或组件。 例如，`applications``servicePrincipals`或 `groups`.
- *{PropertySet}* - 可选。 要为其授予访问权限的实体的特定属性或方面。 例如， `microsoft.directory/applications/authentication/read` 授予在 Azure AD 中的 **应用程序对象上** 读取回复 URL、注销 URL 和隐式流属性的功能。 以下是通用属性集的保留名称：  
  - `allProperties` - 指定实体的所有属性，包括特权属性。 示例包括 `microsoft.directory/applications/allProperties/read` 和 `microsoft.directory/applications/allProperties/update`.
  - `basic` - 指定常见的读取属性，但不包括特权属性。 例如， `microsoft.directory/applications/basic/update` 包括更新标准属性（如显示名称）的功能。
  - `standard` - 指定常见的更新属性，但不包括特权属性。 例如，`microsoft.directory/applications/standard/read`。
- *{Actions}* - 正在授予的操作。 在大多数情况下，权限应以 CRUD 操作或 `allTasks`。 操作 包括:
  - `create` - 创建实体的新实例的功能。
  - `read` - 读取给定属性集的功能 (包括 allProperties) 。
  - `update` - 更新给定属性集的功能 (包括 allProperties) 。
  - `delete` - 删除给定实体的功能。
  - `allTasks` - 表示创建、读取、更新和删除)  (的所有 CRUD 操作。 

### <a name="condition-property"></a>condition 属性
条件定义必须满足的约束。 例如，要求主体是目标资源的所有者。 下面是受支持的条件：

- `Self`：“@Subject.objectId == @Resource.objectId”
- `Owner`：“@Subject.objectId Any_of @Resource.owners”

下面是角色权限的示例，其中的条件是主体是目标资源的所有者。

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
  "@odata.type": "#microsoft.graph.unifiedRolePermission",
  "allowedResourceActions": ["String"],
  "excludedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>另请参阅

- [Azure Active Directory 中的管理员角色权](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) 限 - 有关内置目录角色权限的信息。
- [Azure Active Directory 中的应用程序注册子类型和权](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) 限 - 有关可用于自定义目录角色的权限的信息。 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->