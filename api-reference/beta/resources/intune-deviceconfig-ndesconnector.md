---
title: ndesConnector 资源类型
description: 表示 OnPrem Ndes 连接器的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5f7e4311dd9af0cb7e9ee292f7322deaac702c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728540"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 OnPrem Ndes 连接器的实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 集合|列出 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的属性和关系。|
|[获取 ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|读取 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的属性和关系。|
|[创建 ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|创建新的 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象。|
|[删除 ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|无|删除 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)。|
|[更新 ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|更新 [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|NDES 连接器的键。|
|lastConnectionDateTime|DateTimeOffset|Ndes 连接器的上次连接时间|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Ndes 连接器状态。 可取值为：`none`、`active`、`inactive`。|
|displayName|String|Ndes 连接器的友好名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```





