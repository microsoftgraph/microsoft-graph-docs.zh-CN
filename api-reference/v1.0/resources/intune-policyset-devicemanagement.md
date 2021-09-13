---
title: deviceManagement 资源类型
description: 充当所有设备和应用管理功能的容器的单一实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 429c9eaba9f0f6af0da78fb4cf502f5fd9b7c8d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044522"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备和应用管理功能的容器的单一实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-policyset-devicemanagement-get.md)|[deviceManagement](../resources/intune-policyset-devicemanagement.md)|读取 [deviceManagement](../resources/intune-policyset-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-policyset-devicemanagement-update.md)|[deviceManagement](../resources/intune-policyset-devicemanagement.md)|更新 [deviceManagement](../resources/intune-policyset-devicemanagement.md) 对象的属性。|

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
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




