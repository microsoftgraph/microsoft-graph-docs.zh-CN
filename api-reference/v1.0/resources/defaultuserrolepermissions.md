---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581195"
---
# <a name="defaultuserrolepermissions-resource-type"></a>defaultUserRolePermissions 资源类型

包含 Azure Active Directory (AD) 中的默认用户角色的一些可自定义权限。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-------- |:---- |:----------- |
| allowedToCreateApps | 布尔值 | 指示默认用户角色是否可以创建应用程序。 |  
| allowedToCreateSecurityGroups | 布尔值 | 指示默认用户角色是否可以创建安全组。 |  
| allowedToReadOtherUsers | 布尔值 | 指示默认用户角色是否可以读取其他用户。 |
|permissionGrantPoliciesAssigned|字符串集合|指示是否允许用户同意应用程序，如果是，授予同意的权限以及 (permissionGrantPolicy 的应用程序同意策略) 管理用户授予同意的权限。 值的格式应为 `managePermissionGrantsForSelf.{id}` ，其中 `{id}` 是内置或自定义 [应用程序许可策略](/azure/active-directory/manage-apps/manage-app-consent-policies)的 **id** 。 空列表指示用户同意应用程序已被禁用。 |

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
