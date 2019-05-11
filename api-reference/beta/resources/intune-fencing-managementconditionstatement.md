---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组管理条件, 在满足所有包含的管理条件时启用/禁用设备/应用程序配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 78f2464793ac8410b3636f3ef378cfc623cc08d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941237"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理条件语句是一组管理条件, 在满足所有包含的管理条件时启用/禁用设备/应用程序配置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|列出[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。|
|[获取 managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|读取[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性和关系。|
|[创建 managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。|
|[删除 managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|无|删除[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)。|
|[更新 managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。|
|[getManagementConditionStatementExpressionString 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|尚未记录|
|[getManagementConditionStatementsForPlatform 函数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件语句的唯一标识符。 创建时分配的系统生成值。|
|displayName|String|管理条件语句的管理员定义名称。|
|说明|字符串|管理员定义的管理条件语句的说明。|
|createdDateTime|DateTimeOffset|管理条件语句的创建时间。 生成的服务端。|
|modifiedDateTime|DateTimeOffset|上次修改管理条件语句的时间。 更新了服务端。|
|表达式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|用于评估管理条件语句是否已激活/停用的管理条件语句表达式。|
|eTag|String|管理条件语句的 ETag。 更新了服务端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|适用于此管理条件语句的平台。
这是通过查看与管理条件语句相关的管理条件和查找适用平台的交集计算得出的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md)集合|与管理条件语句关联的管理条件。|

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




