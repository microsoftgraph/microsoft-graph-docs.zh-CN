---
title: deviceManagement 资源类型
description: 充当设备管理下的 Android for Work 设置功能容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f57cdc68d814c00ff61c22db8855f2131e5ae1c
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452907"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当设备管理下的 Android for Work 设置功能容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-androidforwork-devicemanagement-get.md)|[deviceManagement](../resources/intune-androidforwork-devicemanagement.md)|读取 [deviceManagement](../resources/intune-androidforwork-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-androidforwork-devicemanagement-update.md)|[deviceManagement](../resources/intune-androidforwork-devicemanagement.md)|更新 [deviceManagement](../resources/intune-androidforwork-devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|

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



