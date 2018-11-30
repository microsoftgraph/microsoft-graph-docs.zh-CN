---
title: locationManagementCondition 资源类型
description: 包含定义位置管理条件，感兴趣，要监视的领域的信息。
ms.openlocfilehash: 45f6fedf55c7a45147b9a8d988823666a4dc9988
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048962"
---
# <a name="locationmanagementcondition-resource-type"></a>locationManagementCondition 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含定义位置管理条件，感兴趣，要监视的领域的信息。

继承自[managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 locationManagementConditions](../api/intune-fencing-locationmanagementcondition-list.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)集合|列出属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象之间的关系。|
|[获取 locationManagementCondition](../api/intune-fencing-locationmanagementcondition-get.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|读取属性和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件的唯一标识符。 系统生成时创建分配值。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|唯一名称|字符串|管理条件的唯一名称。 在管理条件表达式中使用。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|字符串|管理员定义管理条件的名称。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|说明|字符串|管理员定义的管理条件说明。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务方。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|管理条件上次修改时间。 更新服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件适用的平台。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|为管理 condition 相关联的管理条件语句。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|

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





