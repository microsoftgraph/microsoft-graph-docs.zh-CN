---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe26bc7b5effb24fb0855da6d84b464f36de4927
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732263"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示一个历史记录报告实例的资源。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 reportRoot](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|读取 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|更新 [reportRoot](../resources/intune-shared-reportroot.md) 对象的属性。|
|**设备配置**|
|[deviceConfigurationDeviceActivity 函数](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[报告](../resources/intune-shared-report.md)|设备配置设备活动报告的元数据|
|[deviceConfigurationUserActivity 函数](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[报告](../resources/intune-shared-report.md)|设备配置用户活动报告的元数据|
|**疑难解答**|
|[managedDeviceEnrollmentFailureDetails 函数](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[报告](../resources/intune-shared-report.md)|尚未记录。|
|[managedDeviceEnrollmentTopFailures 函数](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[报告](../resources/intune-shared-report.md)|尚未记录。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>示例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```






