---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e102061864c39fcba9354fce916cf57c43a88b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007227"
---
# <a name="defaultuserrolepermissions-resource-type"></a>defaultUserRolePermissions 资源类型

包含默认用户角色在 AD Azure Active Directory (中的) 。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| allowedToCreateApps | 布尔值 | 指示默认用户角色是否可以创建应用程序。 |  
| allowedToCreateSecurityGroups | Boolean | 指示默认用户角色是否可以创建安全组。 |  
| allowedToReadOtherUsers | 布尔值 | 指示默认用户角色是否可以读取其他用户。 |
|permissionGrantPoliciesAssigned|String collection|指示是否允许用户同意应用，如果允许，授予同意的权限以及哪个应用许可策略 (permissionGrantPolicy) 管理用户授予同意的权限。 值的格式应为 ，其中 是内置或自定义应用同意策略 `managePermissionGrantsForSelf.{id}` `{id}` 的[ID。](/azure/active-directory/manage-apps/manage-app-consent-policies)  空列表表示已禁用用户对应用的同意。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
