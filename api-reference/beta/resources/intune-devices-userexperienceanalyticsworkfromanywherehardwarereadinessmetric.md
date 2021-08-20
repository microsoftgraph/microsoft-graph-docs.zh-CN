---
title: userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 资源类型
description: 用户体验分析硬件准备情况实体包含有关 Windows 升级的硬件阻止程序的帐户级别信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9092b35287b1da40c92c1df7f5f157ee02cab8f
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259217"
---
# <a name="userexperienceanalyticsworkfromanywherehardwarereadinessmetric-resource-type"></a>userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析硬件准备情况实体包含有关 Windows 升级的硬件阻止程序的帐户级别信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-get.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|读取 [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) 关系。|
|[更新 userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-update.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|更新 [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析硬件准备情况指标对象的唯一标识符。|
|totalDeviceCount|Int32|组织中设备总数。 有效值 -2147483648 2147483647|
|upgradeEligibleDeviceCount|Int32|组织中符合 Windows 升级条件的设备计数。 有效值 -2147483648 2147483647|
|ramCheckFailedPercentage|双精度|RAM 硬件检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|storageCheckFailedPercentage|双精度|存储硬件检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorCoreCountCheckFailedPercentage|双精度|处理器硬件核心计数检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorSpeedCheckFailedPercentage|双精度|处理器硬件速度检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|tpmCheckFailedPercentage|双精度|受信任的平台模块用于 TPM (硬件检查) 的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|secureBootCheckFailedPercentage|双精度|安全启动硬件检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processorFamilyCheckFailedPercentage|双精度|处理器硬件系列检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|processor64BitCheckFailedPercentage|双精度|处理器硬件 64 位体系结构检查失败的设备百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|osCheckFailedPercentage|双精度|操作系统检查失败的设备的百分比。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "String (identifier)",
  "totalDeviceCount": 1024,
  "upgradeEligibleDeviceCount": 1024,
  "ramCheckFailedPercentage": "4.2",
  "storageCheckFailedPercentage": "4.2",
  "processorCoreCountCheckFailedPercentage": "4.2",
  "processorSpeedCheckFailedPercentage": "4.2",
  "tpmCheckFailedPercentage": "4.2",
  "secureBootCheckFailedPercentage": "4.2",
  "processorFamilyCheckFailedPercentage": "4.2",
  "processor64BitCheckFailedPercentage": "4.2",
  "osCheckFailedPercentage": "4.2"
}
```




