---
title: unifiedRolePermission 资源类型
description: 目录角色权限是允许的资源操作和条件的集合。
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b068f0aa5ef8af008e84d878d0f7a5e02bc83636
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761231"
---
# <a name="unifiedrolepermission-resource-type"></a>unifiedRolePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示允许的资源操作的集合以及使操作生效所必须满足的条件。 资源操作是可针对资源执行的任务。 例如，应用程序资源支持创建、更新、删除和重置密码资源操作。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowedResourceActions|字符串集合| 可在资源上执行的任务集。 |
|condition|String| 权限生效所必须满足的可选约束。 |

### <a name="allowedresourceactions-property"></a>allowedResourceActions 属性

下面是资源操作架构： 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
例如：`microsoft.directory/applications/credentials/update`。  

- 命名空间 - 公开任务的服务。 例如，Azure Active Directory 中所有任务均使用命名空间 microsoft.directory。  
- Entity - Microsoft Graph 中的服务公开的逻辑功能或组件。 例如，应用程序、服务主体或组。
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

- [Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) 中的管理员角色权限 - 有关内置目录角色的权限的信息。
- [Azure Active Directory 中的](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) 应用程序注册子类型和权限 - 有关可用于自定义目录角色的权限的信息。 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
