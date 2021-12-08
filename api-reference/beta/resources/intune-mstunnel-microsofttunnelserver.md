---
title: microsoftTunnelServer 资源类型
description: 表示单个服务器Microsoft Tunnel的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507c3d7af22614b96235853e0f5e0351adaf1198
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336130"
---
# <a name="microsofttunnelserver-resource-type"></a>microsoftTunnelServer 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示单个服务器Microsoft Tunnel的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 集合|列出 [microsoftTunnelServer 对象的属性和](../resources/intune-mstunnel-microsofttunnelserver.md) 关系。|
|[获取 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|读取 [microsoftTunnelServer 对象的属性和](../resources/intune-mstunnel-microsofttunnelserver.md) 关系。|
|[创建 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|创建新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。|
|[删除 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|无|删除 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)。|
|[更新 microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|更新 [microsoftTunnelServer 对象](../resources/intune-mstunnel-microsofttunnelserver.md) 的属性。|
|[getHealthMetrics 操作](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrics.md)|[keyLongValuePair](../resources/intune-shared-keylongvaluepair.md) 集合|尚未记录|
|[getHealthMetricTimeSeries 操作](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrictimeseries.md)|[metricTimeSeriesDataPoint](../resources/intune-mstunnel-metrictimeseriesdatapoint.md) 集合|尚未记录|
|[createServerLogCollectionRequest 操作](../api/intune-mstunnel-microsofttunnelserver-createserverlogcollectionrequest.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelServer 的 ID|
|displayName|String|MicrosoftTunnelServer 的显示名称|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|MicrosoftTunnelServer 的运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。|
|lastCheckinDateTime|DateTimeOffset|MicrosoftTunnelServer 上次签入时间|
|agentImageDigest|String|在此服务器上运行的当前代理映像的摘要 |
|serverImageDigest|String|在此服务器上运行的当前服务器映像的摘要 |

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
  "lastCheckinDateTime": "String (timestamp)",
  "agentImageDigest": "String",
  "serverImageDigest": "String"
}
```




