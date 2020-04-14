---
title: locationManagementCondition 资源类型
description: 包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f49359a9c3e527e30944030a8c0969c7c12ce9e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382729"
---
# <a name="locationmanagementcondition-resource-type"></a>locationManagementCondition 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于定义位置管理条件（要监视的感兴趣的区域）的信息。


继承自[managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 locationManagementConditions](../api/intune-fencing-locationmanagementcondition-list.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合|列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。|
|[获取 locationManagementCondition](../api/intune-fencing-locationmanagementcondition-get.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|读取[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件的唯一标识符。 创建时分配的系统生成值。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|字符串|管理条件的唯一名称。 在管理条件表达式中使用。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|管理条件的管理员定义名称。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|字符串|管理条件的管理员定义的说明。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|管理条件的创建时间。 生成的服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|上次修改管理条件的时间。 更新了服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新了服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|适用于此管理条件的平台。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|与管理条件相关联的管理条件语句。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
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



