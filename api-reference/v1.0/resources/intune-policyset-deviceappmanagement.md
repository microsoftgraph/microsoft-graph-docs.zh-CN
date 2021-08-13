---
title: deviceAppManagement 资源类型
description: 充当所有设备和应用管理功能的容器的单一实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b51aef0f56483bf3dcb575385e06b91fbab09efa1e47285adbe5b2a155a41a26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205239"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备和应用管理功能的容器的单一实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceAppManagement](../api/intune-policyset-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md)|读取 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的属性和关系。|
|[更新 deviceAppManagement](../api/intune-policyset-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md)|更新 [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|

## <a name="relationships"></a>关系
无

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




