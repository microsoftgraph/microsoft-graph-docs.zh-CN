---
title: managedDeviceMobileAppConfigurationDeviceSummary 资源类型
description: 包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 597b153a2897f37a6c6d497617bd374ade56c6e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971380"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a>managedDeviceMobileAppConfigurationDeviceSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 MDM 移动应用配置设备状态摘要的属性、继承属性和操作。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|读取 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性和关系。|
|[更新 managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|pendingCount|Int32|挂起设备的数量|
|notApplicableCount|Int32|不适用设备的数量|
|successCount|Int32|成功设备的数量|
|errorCount|Int32|错误设备的数量|
|failedCount|Int32|失败设备的数量|
|lastUpdateDateTime|DateTimeOffset|上次更新时间|
|configurationVersion|Int32|用于此概述的策略版本|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



