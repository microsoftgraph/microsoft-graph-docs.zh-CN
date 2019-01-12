---
title: ndesConnector 资源类型
description: 代表 OnPrem Ndes 连接器的实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a65a95310bf3bd4994dd29427cd19cca121d129
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946663"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表 OnPrem Ndes 连接器的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)集合|列出属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象之间的关系。|
|[获取 ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|读取属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的关系。|
|[创建 ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|创建新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。|
|[删除 ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|无|删除[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)。|
|[更新 ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|NDES 连接符的键。|
|lastConnectionDateTime|DateTimeOffset|Ndes 连接器的最后一个连接时间|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Ndes 连接器状态。 可取值为：`none`、`active`、`inactive`。|
|displayName|字符串|Ndes 连接器的友好名称。|

## <a name="relationships"></a>Relationships
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





