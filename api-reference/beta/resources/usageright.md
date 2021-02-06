---
title: usageRight 资源类型
description: 包含有关 usageRight 用户/设备已分配的信息
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d3d7ad0de7eb6929e54b7d3d692c6e562e9da76d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130408"
---
# <a name="usageright-resource-type"></a>usageRight 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用权限表示用户或设备具有的许可证，适用于基于电源应用构建的第三方软件，或仅针对基于设备 (订阅) 。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出用户 usageRights](../api/user-list-usagerights.md)|[usageRight](../resources/usageright.md) 集合|获取用户的使用权限列表。|
|[列出设备 usageRights](../api/device-list-usagerights.md)|[usageRight](../resources/usageright.md) 集合|获取设备的使用权限列表。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|catalogId|字符串|与使用权限对应的产品 ID。|
|id|字符串|使用权限的 ID。|
|serviceIdentifier|字符串|与使用权限对应的服务的标识符。|
|state|usageRightState|使用权限的状态。 可取值为：`active`、`inactive`、`warning`、`suspended`。|

### <a name="usagerightstate-values"></a>usageRightState 值 

| 成员             |  说明               |
| :----------------- |  :------------------------ |
|active              | 指示使用权限处于活动状态，可用于预配权益。|
|inactive                | 指示使用权限不是活动的，不能用于预配权益。|
|警告                | 指示使用权限可能由于付款违反而宽限期。 此状态可用于提醒待付款或提供降级体验。|
|已挂起                | 指示使用权限可能由于付款违反而暂停|
|unknownFutureValue      | 指示未来值的 Sentinel 值。 |

>**注意：** 只有活动状态和警告状态表示可用的好处。 其他所有状态都将被视为没有产生可用的好处。



## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "baseType": "",
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

