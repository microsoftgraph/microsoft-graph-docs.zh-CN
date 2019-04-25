---
title: ndesConnector 资源类型
description: 表示 OnPrem Ndes 连接器的实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3781827d93f1e646becc2ee47de57cbba82dfc63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554469"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 OnPrem Ndes 连接器的实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)集合|列出[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性和关系。|
|[获取 ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|读取[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性和关系。|
|[创建 ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|创建新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。|
|[删除 ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|无|删除[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)。|
|[更新 ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。|

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





