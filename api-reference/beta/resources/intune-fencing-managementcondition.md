---
title: managementCondition 资源类型
description: 管理条件是可动态触发的事件，如地理围栏、时间围栏和网络围栏。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8db902ca0f5b0fb00a72e9fd8eee8af02d2c8cab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030254"
---
# <a name="managementcondition-resource-type"></a>managementCondition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理条件是可动态触发的事件，如地理围栏、时间围栏和网络围栏。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managementConditions](../api/intune-fencing-managementcondition-list.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) 集合|列出 [managementCondition 对象的属性和](../resources/intune-fencing-managementcondition.md) 关系。|
|[获取 managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|读取 [managementCondition 对象的属性和](../resources/intune-fencing-managementcondition.md) 关系。|
|[getManagementConditionsForPlatform 函数](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件的唯一标识符。 创建时分配的系统生成值。|
|唯一名称|String|管理条件的唯一名称。 在管理条件表达式中使用。|
|displayName|String|管理员定义的管理条件名称。|
|说明|String|管理员定义的管理条件说明。|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务器端。|
|modifiedDateTime|DateTimeOffset|上次修改管理条件的时间。 更新的服务器端。|
|eTag|String|管理条件的 ETag。 更新的服务器端。|
|applicablePlatforms|[devicePlatformType](../resources/intune-fencing-deviceplatformtype.md) 集合|此管理条件的适用平台。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|与管理条件关联的管理条件语句。|

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



