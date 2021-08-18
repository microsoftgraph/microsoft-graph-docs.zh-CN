---
title: managedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb5ea02b6c5d4a8162aab622a0c747868c5e255b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264988"
---
# <a name="managedappconfiguration-resource-type"></a>managedAppConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于将一组自定义设置按原样提供给配置范围确定的用户应用的配置。


继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppConfigurations](../api/intune-mam-managedappconfiguration-list.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 集合|列出 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。|
|[Get managedAppConfiguration](../api/intune-mam-managedappconfiguration-get.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合|一组字符串键和字符串值对，要发送到配置范围确定的用户应用，且不被此服务改变|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




