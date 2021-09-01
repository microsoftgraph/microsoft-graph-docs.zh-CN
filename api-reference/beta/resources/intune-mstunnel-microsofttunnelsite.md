---
title: microsoftTunnelSite 资源类型
description: 表示网站Microsoft Tunnel实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ac94541351c417b8f6ec3d49cc66898557ab3cf
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817647"
---
# <a name="microsofttunnelsite-resource-type"></a>microsoftTunnelSite 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示网站Microsoft Tunnel实体

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 集合|列出 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象的属性和关系。|
|[获取 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|读取 [microsoftTunnelSite 对象的属性和](../resources/intune-mstunnel-microsofttunnelsite.md) 关系。|
|[创建 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|创建新的 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。|
|[删除 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|无|删除 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)。|
|[更新 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|更新 [microsoftTunnelSite 对象](../resources/intune-mstunnel-microsofttunnelsite.md) 的属性。|
|[requestUpgrade 操作](../api/intune-mstunnel-microsofttunnelsite-requestupgrade.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelSite 的 ID|
|displayName|字符串|MicrosoftTunnelSite 的显示名称|
|description|字符串|MicrosoftTunnelSite 的说明|
|publicAddress|字符串|MicrosoftTunnelSite 的公共域名或 IP 地址|
|upgradeWindowUtcOffsetInMinutes|Int32|网站时区表示为与 UTC 的分钟偏移量|
|upgradeWindowStartTime|TimeOfDay|网站的升级窗口一天中的开始时间|
|upgradeWindowEndTime|TimeOfDay|网站的升级窗口结束时间|
|upgradeAutomatically|布尔值|网站的自动升级设置。 True 表示自动升级，false 表示手动控制|
|upgradeAvailable|布尔值|如果升级可用，则其为 True|
|internalNetworkProbeUrl|String|MicrosoftTunnelSite 的内部网络访问探测器 URL|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|已应用于此 MicrosoftTunnelSite 的 MicrosoftTunnelConfiguration|
|microsoftTunnelServers|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 集合|注册到此 MicrosoftTunnelSite 的 MicrosoftTunnelServers 列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "upgradeWindowUtcOffsetInMinutes": 1024,
  "upgradeWindowStartTime": "String (time of day)",
  "upgradeWindowEndTime": "String (time of day)",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



