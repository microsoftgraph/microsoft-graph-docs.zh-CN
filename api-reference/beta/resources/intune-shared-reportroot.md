---
title: reportRoot 资源类型
description: 表示的设备或疑难解答的报告，具体取决于上下文实例的资源。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421331"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示的设备或疑难解答的报告，具体取决于上下文实例的资源。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune-shared-reportroot-get.md)|读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune-shared-reportroot-update.md)|更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。|
|**设备配置**|
|[deviceConfigurationUserActivity 函数](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|设备配置用户活动报告的元数据|
|[deviceConfigurationDeviceActivity 函数](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|设备配置设备活动报告的元数据|
|**疑难解答**|
|[managedDeviceEnrollmentAbandonmentDetails 函数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[报告](../resources/intune-shared-report.md)|注册放弃的元数据的详细信息报表|
|[managedDeviceEnrollmentAbandonmentSummary 函数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[报告](../resources/intune-shared-report.md)|注册放弃摘要报告的元数据|
|[managedDeviceEnrollmentFailureDetails 函数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|尚未记录|
|[managedDeviceEnrollmentFailureTrends 函数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|注册失败趋势报告的元数据|
|[managedDeviceEnrollmentTopFailures 函数](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



