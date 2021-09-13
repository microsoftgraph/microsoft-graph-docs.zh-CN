---
title: reportRoot 资源类型
description: 表示设备或疑难解答报告的实例的资源，具体取决于上下文。
ms.localizationpriority: medium
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56e3bc6d11c913a35ee69a803a7e038a86971518
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115273"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备或疑难解答报告的实例的资源，具体取决于上下文。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune-shared-reportroot-get.md)|读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune-shared-reportroot-update.md)|更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。|
|**设备配置**|
|[deviceConfigurationUserActivity 函数](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|设备配置用户活动报告的元数据|
|[deviceConfigurationDeviceActivity 函数](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|设备配置设备活动报告的元数据|
|**疑难解答**|
|[managedDeviceEnrollmentAbandonmentDetails 函数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[报告](../resources/intune-shared-report.md)|注册的元数据详细信息报告|
|[managedDeviceEnrollmentAbandonmentSummary 函数](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[报告](../resources/intune-shared-report.md)|注册的元数据摘要报告|
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



