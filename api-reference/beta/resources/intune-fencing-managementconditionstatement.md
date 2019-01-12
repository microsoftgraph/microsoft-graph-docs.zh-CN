---
title: managementConditionStatement 资源类型
description: 管理条件语句是一组的管理条件的启用/禁用设备/应用程序配置满足所有包含的管理条件时。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82a99e878337cf04659b8bc7da7e821bd8afb6aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929982"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|id|字符串|管理条件语句的唯一标识符。 系统生成时创建分配值。|
|displayName|字符串|管理员定义管理条件语句的名称。|
|说明|字符串|管理员定义管理条件语句的说明。|
|createdDateTime|DateTimeOffset|创建管理条件语句的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|管理条件语句上次修改时间。 更新服务端。|
|表达式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|用来评估如果管理条件语句的管理条件语句表达式已激活/停用。|
|eTag|String|管理条件语句的 ETag。 更新服务端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件语句适用的平台。
这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。|

## <a name="relationships"></a>Relationships
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





