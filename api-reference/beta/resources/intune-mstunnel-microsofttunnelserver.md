---
title: microsoftTunnelServer 资源类型
description: 表示单个 Microsoft 隧道服务器的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed9968e5f1d0f4c530d09d0ff8950ad6864b90c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301540"
---
# <a name="microsofttunnelserver-resource-type"></a>microsoftTunnelServer 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示单个 Microsoft 隧道服务器的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 集合|列出 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的属性和关系。|
|[获取 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|读取 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的属性和关系。|
|[创建 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|创建新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。|
|[删除 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|无|删除 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)。|
|[更新 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|更新 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|MicrosoftTunnelServer 的 Id|
|displayName|字符串|MicrosoftTunnelServer 的显示名称|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|MicrosoftTunnelServer 的运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。|
|lastCheckinDateTime|DateTimeOffset|上次签入的 MicrosoftTunnelServer|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "String (identifier)",
  "displayName": "String",
  "tunnelServerHealthStatus": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```




