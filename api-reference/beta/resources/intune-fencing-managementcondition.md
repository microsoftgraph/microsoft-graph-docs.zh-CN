---
title: managementCondition 资源类型
description: 管理条件都可以地理范围，如动态触发的事件时限和网络范围。
localization_priority: Normal
ms.openlocfilehash: a836aeaa660de8f02c4e441e9eb390e1513c917c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834109"
---
# <a name="managementcondition-resource-type"></a>managementCondition 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理条件都可以地理范围，如动态触发的事件时限和网络范围。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 managementConditions](../api/intune-fencing-managementcondition-list.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)集合|列出属性和[managementCondition](../resources/intune-fencing-managementcondition.md)对象之间的关系。|
|[获取 managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|读取属性和[managementCondition](../resources/intune-fencing-managementcondition.md)对象的关系。|
|[getManagementConditionsForPlatform 函数](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件的唯一标识符。 系统生成时创建分配值。|
|唯一名称|字符串|管理条件的唯一名称。 在管理条件表达式中使用。|
|displayName|字符串|管理员定义管理条件的名称。|
|说明|字符串|管理员定义的管理条件说明。|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务方。|
|modifiedDateTime|DateTimeOffset|管理条件上次修改时间。 更新服务端。|
|eTag|String|管理条件的 ETag。 更新服务端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件适用的平台。|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|为管理 condition 相关联的管理条件语句。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





