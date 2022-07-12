---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7004b3748a75d2bc680d0bd6bc7cbbb0d6c7e780
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735570"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备管理功能的容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-reporting-devicemanagement-get.md)|[deviceManagement](../resources/intune-reporting-devicemanagement.md)|读取 [deviceManagement](../resources/intune-reporting-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-reporting-devicemanagement-update.md)|[deviceManagement](../resources/intune-reporting-devicemanagement.md)|更新 [deviceManagement](../resources/intune-reporting-devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|报告|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|单一实例报表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```





