---
title: deviceEnrollmentPlatformRestrictionConfiguration 资源类型
description: 设备注册 配置，用于限制用户可为单个平台注册的设备类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82281bcdd6c11a6498f8aa5d2541073bbb93a71f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046727"
---
# <a name="deviceenrollmentplatformrestrictionconfiguration-resource-type"></a>deviceEnrollmentPlatformRestrictionConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备注册 配置，用于限制用户可为单个平台注册的设备类型


继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceEnrollmentPlatformRestrictionConfigurations](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-list.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 集合|列出 [deviceEnrollmentPlatformRestrictionConfiguration 对象的属性和](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 关系。|
|[获取 deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|读取 [deviceEnrollmentPlatformRestrictionConfiguration 对象的属性和](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 关系。|
|[创建 deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|创建新的 [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 对象。|
|[删除 deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-delete.md)|无|删除 [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)。|
|[更新 deviceEnrollmentPlatformRestrictionConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)|更新 [deviceEnrollmentPlatformRestrictionConfiguration 对象](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|设备注册显示名称继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|说明|String|设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|如果用户位于分配了注册配置的多个组中，则使用优先级。 用户仅受优先级值最低的配置使用。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|String collection|注册限制的可选角色范围标记。 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|platformRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|基于平台、平台操作系统版本和设备所有权的限制|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|应用此限制的平台类型。 可取值为：`allPlatforms`、`ios`、`windows`、`windowsPhone`、`android`、`androidForWork`、`androidAosp`、`mac`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合|设备配置文件的组分配列表 继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String",
    "blockedManufacturers": [
      "String"
    ],
    "blockedSkus": [
      "String"
    ]
  },
  "platformType": "String"
}
```



