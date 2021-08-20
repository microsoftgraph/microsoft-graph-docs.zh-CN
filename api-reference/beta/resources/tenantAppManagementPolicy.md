---
title: tenantAppManagementPolicy 资源类型
description: 应用程序身份验证方法租户默认策略强制实施应用管理操作限制。
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e5177fe5bc69a3f083619823146c605152498d71
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2021
ms.locfileid: "58397108"
---
# <a name="tenantappmanagementpolicy-resource-type"></a>tenantAppManagementPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

租户范围的应用程序身份验证方法策略，用于强制执行所有应用程序和服务主体的应用管理限制。 此策略适用于所有应用和服务主体，除非在 [将 appManagementPolicy](../resources/appmanagementpolicy.md) 应用于对象时被覆盖。

继承自 [policyBase](policybase.md)。

## <a name="methods"></a>方法

| 方法                                                | 返回类型                                                             | 说明                                                                         |
| :---------------------------------------------------- | :---------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [Get](../api/tenantAppManagementPolicy-get.md)       | [tenantAppManagementPolicy](../resources/tenantAppManagementPolicy.md) | 读取应用程序和服务主体的默认应用管理策略集的属性。 |
| [更新](../api/tenantAppManagementPolicy-update.md) | 无                                                                    | 更新应用程序和服务主体的默认应用管理策略。  |

## <a name="properties"></a>属性

| 属性                     | 类型                                                                     | 说明                                                           |
| :--------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| id                           | String                                                                   | 默认策略标识符。                                        |
| displayName                  | String                                                                   | 默认显示名称的默认值。 继承自 [policyBase](policybase.md)。                                |
| 说明                  | String                                                                   | 默认策略的说明。 继承自 [policyBase](policybase.md)。                                |
| isEnabled                    | Boolean                                                                  | 表示是否启用策略。 默认值为 `false`。                                    |
| applicationRestrictions      | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有应用程序对象的默认限制。               |
| servicePrincipalRestrictions | [appManagementConfiguration](../resources/appManagementConfiguration.md) | 应用于租户中所有服务主体对象的默认限制。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAppManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/defaultAppManagementPolicy",
  "id": "string (identifier)",
  "description": "string",
  "displayName": "string",
  "isEnabled": false,
  "applicationRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type":"microsoft.graph.appManagementConfiguration"
  }
}
```
