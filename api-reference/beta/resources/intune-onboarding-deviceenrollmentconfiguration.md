---
title: deviceEnrollmentConfiguration 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ce79b3c760a24857e1856204ba6aefcf28e44168
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414366"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceEnrollmentConfigurations](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合|列出 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。|
|[获取 deviceEnrollmentConfiguration](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|读取 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。|
|[setPriority action](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|无|尚未记录|
|[分配操作](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|displayName|String|尚未记录|
|description|String|尚未记录|
|优先级|Int32|尚未记录|
|createdDateTime|DateTimeOffset|尚未记录|
|lastModifiedDateTime|DateTimeOffset|尚未记录|
|version|Int32|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|设备配置文件的组分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```




