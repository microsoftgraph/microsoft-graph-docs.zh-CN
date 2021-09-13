---
title: reportRoot 资源类型
description: 表示注册失败报告实例的资源。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0545c2f2b0fbabc03fbc2b628a9d1752fc3f0748
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021510"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示注册失败报告实例的资源。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune-troubleshooting-reportroot-get.md)|[reportRoot](../resources/intune-troubleshooting-reportroot.md)|读取 [reportRoot](../resources/intune-troubleshooting-reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune-troubleshooting-reportroot-update.md)|[reportRoot](../resources/intune-troubleshooting-reportroot.md)|更新 [reportRoot](../resources/intune-troubleshooting-reportroot.md) 对象的属性。|
|[managedDeviceEnrollmentFailureDetails 函数](../api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails.md)|[报告](../resources/intune-troubleshooting-report.md)|尚未记录|
|[managedDeviceEnrollmentFailureDetails 函数](../api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails.md)|[报告](../resources/intune-troubleshooting-report.md)|尚未记录|
|[managedDeviceEnrollmentTopFailures 函数](../api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures.md)|[报告](../resources/intune-troubleshooting-report.md)|尚未记录|
|[managedDeviceEnrollmentTopFailures 函数](../api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures.md)|[报告](../resources/intune-troubleshooting-report.md)|尚未记录|

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




