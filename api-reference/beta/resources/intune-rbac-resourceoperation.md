---
title: resourceOperation 资源类型
description: 介绍 Intune，支持基于角色的访问控制 (RBAC) 的 Microsoft Graph api resourceOperation 资源。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 897c076139f3a385152738dd5f4b15c06320990d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425020"
---
# <a name="resourceoperation-resource-type"></a>resourceOperation 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

这可以定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有读取、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，Assign 操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。这会定义能够在 Intune 资源（或实体）上执行的操作或行为。  常用操作有获取、列出、删除、更新或创建。  这些操作提供对基础 Intune 资源本身的基本管理。  某些情况下，Intune 资源可以采用资源使用的操作，以与其他资源合并采用。  例如，“Assign”操作用于向 AAD 安全组分配 MobileApp 资源。  无法修改内置角色的资源操作。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List resourceOperations](../api/intune-rbac-resourceoperation-list.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合|列出 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。|
|[Get resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|读取 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性和关系。|
|[Create resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。|
|[Delete resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|无|删除 [resourceOperation](../resources/intune-rbac-resourceoperation.md)。|
|[Update resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。|
|[getScopesForUser 函数](../api/intune-rbac-resourceoperation-getscopesforuser.md)|String collection|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|资源操作的键。 只读，且自动生成。|
|资源|String|资源此操作所属类别。|
|resourceName|String|执行此操作的资源的名称。|
|actionName|String|此操作将执行的操作类型。 actionName 应简明，并尽可能限制在几个字以内。|
|说明|String|资源操作的说明。 当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。|
|enabledForScopeValidation|Boolean|确定是否定义每个角色分配的作用域验证权限。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```




