---
title: usageRight 资源类型
description: 包含有关使用情况的信息已分配用户/设备
author: jeeshnair
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e436ad4d793082cbd5c1c8d498b5dbe5b7c7fe54
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214734"
---
# <a name="usageright-resource-type"></a>usageRight 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用权限表示用户或设备具有的许可证，适用于基于 Power Apps 构建的第三方软件或仅针对基于设备 (订阅) 。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出用户使用情况Rights](../api/user-list-usagerights.md)|[usageRight](../resources/usageright.md) 集合|获取用户的使用权限列表。|
|[列出设备使用情况Rights](../api/device-list-usagerights.md)|[usageRight](../resources/usageright.md) 集合|获取设备的使用权限列表。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|catalogId|字符串|与使用权限对应的产品 ID。|
|id|String|使用权限的 ID。|
|serviceIdentifier|String|与使用权限对应的服务的标识符。|
|state|usageRightState|使用权限的状态。 可能的值是：`active`、`inactive`、`warning`、`suspended`。|

### <a name="usagerightstate-values"></a>usageRightState 值 

| 成员             |  说明               |
| :----------------- |  :------------------------ |
|active              | 指示使用权限处于活动状态，可用于预配权益。|
|inactive                | 指示使用权限不是活动的，并且不能用于预配权益。|
|警告                | 指示使用权限可能由于付款违反而获得宽限期。 此状态可用于提醒待付款或提供降级体验。|
|已挂起                | 指示使用权限可能由于"付款违反"而暂停|
|unknownFutureValue      | Sentinel 值，用于指示未来值。 |

>**注意：** 只有活动状态和警告状态表示一种可用的好处。 其他所有状态都将被视为未产生可用的好处。



## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

