---
title: reportRoot 资源类型
description: 表示一个历史记录报告实例的资源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a56c45110ecc2c31ca510ae8d18c29a5c9601e80
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755242"
---
# <a name="reportroot-resource-type"></a>reportRoot 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示一个历史记录报告实例的资源。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 reportRoot](../api/intune-deviceconfig-reportroot-get.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|读取 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 对象的属性和关系。|
|[更新 reportRoot](../api/intune-deviceconfig-reportroot-update.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|更新 [reportRoot](../resources/intune-deviceconfig-reportroot.md) 对象的属性。|
|[deviceConfigurationUserActivity 函数](../api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity.md)|[报告](../resources/intune-deviceconfig-report.md)|设备配置用户活动报告的元数据|
|[deviceConfigurationDeviceActivity 函数](../api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity.md)|[报告](../resources/intune-deviceconfig-report.md)|设备配置设备活动报告的元数据|

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




