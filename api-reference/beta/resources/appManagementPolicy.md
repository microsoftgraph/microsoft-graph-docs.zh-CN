---
title: appManagementPolicy 资源类型
description: 用于对特定应用程序或服务主体强制执行应用管理限制的应用程序身份验证方法策略。
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c3a705a567e4692d07220398317cc36c2bab71a6
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660387"
---
# <a name="appmanagementpolicy-resource-type"></a>appManagementPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对特定应用程序和服务主体的应用管理操作强制实施限制。 如果未为应用程序或服务主体配置此资源，则限制默认为 [tenantAppManagementPolicy 对象中的](tenantappmanagementpolicy.md) 设置。

## <a name="methods"></a>方法

| 方法                                                         | 返回类型                                                                | Description                                                                                                            |
| :------------------------------------------------------------- | :------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| [List](../api/appManagementPolicy-list.md)      | [appManagementPolicy](../resources/appManagementPolicy.md) | 返回为应用程序和服务主体创建的应用管理策略及其属性的列表。 |
| [Create](../api/appManagementPolicy-post.md)    | [appManagementPolicy](../resources/appManagementPolicy.md) | 创建可分配给应用程序或服务主体对象的应用管理策略。                   |
| [Get](../api/appManagementPolicy-get.md)       | [appManagementPolicy](../resources/appManagementPolicy.md) | 获取单个应用管理策略对象。                                                                            |
| [更新](../api/appManagementPolicy-update.md) | 无                                                                       | 更新应用管理策略。                                                                                      |
| [删除](../api/appManagementPolicy-delete.md) | 无                                                                       | 从 appManagementPolicies 中的策略集合中删除应用管理策略。                             |
| [List appliesTo](../api/appManagementPolicy-list-appliesTo.md)| [appManagementPolicy](../resources/appManagementPolicy.md)|返回应用了策略的应用程序和服务主体的列表。 |
| [Assign appliesTo](../api/appManagementPolicy-post-appliesTo.md)| 无 |返回应用了策略的应用程序和服务主体的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型                                                        | 说明                                                            |
| :----------- | :---------------------------------------------------------- | :--------------------------------------------------------------------- |
| id           | 字符串                                                      | 策略标识符。                                                 |
| displayName  | 字符串                                                      | 策略显示名称。 继承自 [policyBase](policybase.md)。                                        |
| 说明  | 字符串                                                      | 策略的说明。 继承自 [policyBase](policybase.md)。                                         |
| isEnabled    | Boolean                                                     | 表示是否启用策略。                                      |
| 限制 | [appManagementConfiguration](appManagementConfiguration.md) | 应用于应用程序或服务主体对象的限制。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                  | 说明                                                                         |
| :----------- | :------------------------------------ | :---------------------------------------------------------------------------------- |
| appliesTo    | [directoryObject](directoryobject.md) | 应用策略的应用程序和服务主体的集合。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appManagementPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

```json
[
  {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies",
    "id": "string (identifier)",
    "description": "string",
    "displayName": "string",
    "isEnabled": true,
    "restrictions": {
      "@odata.type": "microsoft.graph.appManagementConfiguration"
    }
  }
]
```
