---
title: deviceEnrollmentConfiguration 资源类型
description: 设备注册配置的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7e15322dd41eaa15e4b00c83a59b361059bbedb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287660"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备注册配置的基类

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceEnrollmentConfigurations](../api/intune-shared-deviceenrollmentconfiguration-list.md)|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合|列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。|
|[获取 deviceEnrollmentConfiguration](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。|
|**载入**|
|[setPriority action](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|无|尚未记录|
|[分配操作](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|无|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|帐户的唯一标识符|
|displayName|字符串|设备注册配置的显示名称|
|description|字符串|设备注册配置的说明|
|priority|Int32|当用户存在于分配有注册配置的多个组中时，将使用优先级。 用户仅限于具有最低优先级值的配置。|
|createdDateTime|DateTimeOffset|设备注册配置的 UTC 格式的创建日期时间|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）|
|version|Int32|设备注册配置的版本|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|**载入**|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|设备配置文件的组分配列表|

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




