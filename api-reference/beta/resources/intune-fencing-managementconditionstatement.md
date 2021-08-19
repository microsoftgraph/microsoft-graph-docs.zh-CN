---
title: managementConditionStatement 资源类型
description: 管理条件声明是一组管理条件，当满足所有所包含的管理条件时，可启用/禁用设备/应用程序配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb0864749fd04fe6ba9979dd31e0a0adaf15854b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256014"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理条件声明是一组管理条件，当满足所有所包含的管理条件时，可启用/禁用设备/应用程序配置。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|列出 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 对象的属性和关系。|
|[获取 managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|读取 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 对象的属性和关系。|
|[创建 managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|创建新的 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 对象。|
|[删除 managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|无|删除 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。|
|[更新 managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|更新 [managementConditionStatement 对象](../resources/intune-fencing-managementconditionstatement.md) 的属性。|
|[getManagementConditionStatementExpressionString 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|尚未记录|
|[getManagementConditionStatementsForPlatform 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件语句的唯一标识符。 创建时分配的系统生成值。|
|displayName|String|管理员定义的管理条件声明的名称。|
|description|String|管理员定义的管理条件声明的说明。|
|createdDateTime|DateTimeOffset|创建管理条件语句的时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改管理条件语句的时间。 更新的服务器端。|
|表达式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|用于评估管理条件语句是否被激活/停用的管理条件语句表达式。|
|eTag|String|管理条件声明的 ETag。 更新的服务器端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-fencing-deviceplatformtype.md) 集合|此管理条件声明的适用平台。
这是通过查看与管理条件声明关联的管理条件并查找适用平台的交集得出的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) 集合|与管理条件语句关联的管理条件。|

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
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "String"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




