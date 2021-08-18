---
title: deviceComplianceDeviceStatus 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 34fee125b5b7842cc836035e99b135126fc33a073cec094d86136961d1322021
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209936"
---
# <a name="devicecompliancedevicestatus-resource-type"></a>deviceComplianceDeviceStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceDeviceStatuses](../api/intune-deviceconfig-devicecompliancedevicestatus-list.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合|列出 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性和关系。|
|[获取 deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-get.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|读取 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性和关系。|
|[创建 deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-create.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|创建新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。|
|[删除 deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-delete.md)|无|删除 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)。|
|[更新 deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-update.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceDisplayName|String|DevicePolicyStatus 的设备名。|
|userName|String|报告的用户名|
|deviceModel|String|报告的设备模型|
|平台|Int32|报告的设备平台|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备符合性宽限期的到期日期/时间|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|策略报告的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|字符串|UserPrincipalName。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```




