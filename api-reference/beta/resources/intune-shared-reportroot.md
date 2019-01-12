---
title: reportRoot 资源类型
description: 表示的设备或疑难解答的报告，具体取决于上下文实例的资源。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: efb8950b9956901161c822df8b467b0182a4cc75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959585"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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



