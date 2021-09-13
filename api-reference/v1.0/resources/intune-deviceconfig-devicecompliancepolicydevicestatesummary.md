---
title: deviceCompliancePolicyDeviceStateSummary 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 57680c6ab5a1ead59e48e54303ee80d885ff4eea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072356"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a>deviceCompliancePolicyDeviceStateSummary 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceCompliancePolicyDeviceStateSummary](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。|
|[更新 deviceCompliancePolicyDeviceStateSummary](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inGracePeriodCount|Int32|宽限期内的设备数|
|configManagerCount|Int32|由 System Center Configuration Manager 管理符合性的设备数|
|id|String|实体的键。|
|unknownDeviceCount|Int32|未知设备的数量|
|notApplicableDeviceCount|Int32|不适用设备的数量|
|compliantDeviceCount|Int32|兼容设备的数量|
|remediatedDeviceCount|Int32|已修复设备的数量|
|nonCompliantDeviceCount|Int32|不兼容设备的数量|
|errorDeviceCount|Int32|错误设备的数量|
|conflictDeviceCount|Int32|冲突设备的数量|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




