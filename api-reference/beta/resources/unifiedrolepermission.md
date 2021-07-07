---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316476"
---
# <a name="unifiedrolepermission-resource-type"></a>unifiedRolePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示允许的资源操作的集合以及使操作生效所必须满足的条件。 资源操作是可在资源上执行的任务。 例如，应用程序资源支持创建、更新、删除和重置密码资源操作。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedResourceActions|字符串集合| 可在资源上执行的任务集。 |
|condition|字符串| 权限生效所必须满足的可选约束。 |

### <a name="allowedresourceactions-property"></a>allowedResourceActions 属性

下面是资源操作架构： 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
例如：`microsoft.directory/applications/credentials/update`。  

- 命名空间 - 公开任务的服务。 例如，所有任务Azure Active Directory命名空间 microsoft.directory。  
- Entity - Microsoft 服务公开的逻辑功能或Graph。 例如，应用程序、服务主体或组。
- PropertySet - 要授予其访问权限的实体的特定属性或方面。 例如，授予在 Azure AD 中读取应用程序对象上的回复 URL、注销 URL 和隐式流 `microsoft.directory/applications/authentication/read` 属性的能力。  以下是常见属性集的保留名称：  
  - allProperties - 指定实体的所有属性，包括特权属性。 示例包括 `microsoft.directory/applications/allProperties/read` `microsoft.directory/applications/allProperties/update` 和 。
  - basic - 指定常用读取属性，但不包括特权属性。 例如， `microsoft.directory/applications/basic/update` 包括更新标准属性（如 显示名称）。
  - standard - 指定常用更新属性，但不包括特权属性。 例如，`microsoft.directory/applications/standard/read`。
- 操作 - 要授予的操作。 在大多数情况下，权限应表示为 CRUD 或 allTasks。 操作包括：
  - Create - 创建实体的新实例的能力。
  - 读取 - 读取给定属性集 (包括 allProperties) 。
  - Update - 更新给定属性集 (包括 allProperties) 。
  - Delete - 删除给定实体的能力。
  - AllTasks - 表示创建、 (、更新和删除文件的所有 CRUD) 。 

### <a name="condition-property"></a>condition 属性
条件定义必须满足的约束。 例如，要求主体是目标"所有者"的要求。 以下是受支持的条件：

- 自我："$ResourceIsSelf"
- 所有者："$SubjectIsOwner"

下面是具有条件的角色权限的示例。

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
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

- [管理员角色权限Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - 有关内置目录角色的权限的信息。
- [应用程序注册子类型和](/azure/active-directory/users-groups-roles/roles-custom-available-permissions)Azure Active Directory - 有关可用于自定义目录角色的权限的信息。 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
