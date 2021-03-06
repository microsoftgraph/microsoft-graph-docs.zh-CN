---
title: deviceAppManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b99cd14d949d4043fe1ecb4b911c6f89a8f12b10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756413"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备应用管理功能的容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceAppManagement](../api/intune-apps-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-apps-deviceappmanagement.md)|读取 [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) 对象的属性和关系。|
|[更新 deviceAppManagement](../api/intune-apps-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-apps-deviceappmanagement.md)|更新 [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|mobileApps|[mobileApp](../resources/intune-apps-mobileapp.md) 集合|移动应用。|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|移动应用类别。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合|托管设备移动应用程序配置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




