---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组的管理条件的启用/禁用设备/应用程序配置满足所有包含的管理条件时。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3292dae241a3f79cc7d3417c93ccc1187c8b8d17
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395991"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理条件语句是一组的管理条件的启用/禁用设备/应用程序配置满足所有包含的管理条件时。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|列出属性和[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象之间的关系。|
|[获取 managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|读取属性和[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的关系。|
|[创建 managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。|
|[删除 managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|无|删除[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。|
|[更新 managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。|
|[getManagementConditionStatementExpressionString 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|尚未记录|
|[getManagementConditionStatementsForPlatform 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件语句的唯一标识符。 系统生成时创建分配值。|
|displayName|String|管理员定义管理条件语句的名称。|
|说明|String|管理员定义管理条件语句的说明。|
|createdDateTime|DateTimeOffset|创建管理条件语句的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|管理条件语句上次修改时间。 更新服务端。|
|表达式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|用来评估如果管理条件语句的管理条件语句表达式已激活/停用。|
|eTag|String|管理条件语句的 ETag。 更新服务端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件语句适用的平台。
这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md)集合|管理条件语句对相关的管理条件。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




