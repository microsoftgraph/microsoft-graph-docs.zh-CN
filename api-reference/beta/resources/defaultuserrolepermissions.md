---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71edaa99eedc7a37abe5694ace6e5c3c05e29884
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202327"
---
# <a name="defaultuserrolepermissions-resource-type"></a>defaultUserRolePermissions 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含Azure AD中默认用户角色的某些可自定义权限。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| allowedToCreateApps | Boolean | 指示默认用户角色是否可以创建应用程序。 |  
| allowedToCreateSecurityGroups | Boolean | 指示默认用户角色是否可以创建安全组。 |  
| allowedToReadBitlockerKeysForOwnedDevice | Boolean | 指示设备的注册所有者是否可以使用默认用户角色读取自己的 BitLocker 恢复密钥。 |
| allowedToReadOtherUsers | Boolean | 指示默认用户角色是否可以读取其他用户。 |  

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
  "allowedToReadBitlockerKeysForOwnedDevice": true,
  "allowedToReadOtherUsers": true
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


