---
title: microsoftTunnelConfiguration 资源类型
description: 表示设置集合Microsoft Tunnel实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6603dc8b69816762e903bbab51f467684b8888a4
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265177"
---
# <a name="microsofttunnelconfiguration-resource-type"></a>microsoftTunnelConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设置集合Microsoft Tunnel实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelConfigurations](../api/intune-mstunnel-microsofttunnelconfiguration-list.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 集合|列出 [microsoftTunnelConfiguration 对象的属性和](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 关系。|
|[获取 microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-get.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|读取 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象的属性和关系。|
|[创建 microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-create.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|创建新的 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象。|
|[删除 microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-delete.md)|无|删除 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)。|
|[更新 microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-update.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|更新 [microsoftTunnelConfiguration 对象](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MicrosoftTunnelConfiguration 的 ID|
|displayName|字符串|MicrosoftTunnelConfiguration 显示名称|
|description|String|MicrosoftTunnelConfiguration 的说明|
|network|String|将用于为客户端分配虚拟地址的子网|
|dnsServers|String collection|客户端将使用的 DNS 服务器|
|defaultDomainSuffix|字符串|客户端将使用的默认域附录|
|routesInclude|String collection|服务器将路由的路由|
|routesExclude|String collection|服务器不会路由的路由子集|
|splitDNS|String collection|使用提供的 dns 服务器解析的域|
|listenPort|Int32|TCP 和 UPD 将在服务器上侦听的端口|
|advancedSettings|[keyValuePair](../resources/intune-mstunnel-keyvaluepair.md) 集合|可应用于服务器的其他设置|
|lastUpdateDateTime|DateTimeOffset|上次更新 MicrosoftTunnelConfiguration 的时间|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "network": "String",
  "dnsServers": [
    "String"
  ],
  "defaultDomainSuffix": "String",
  "routesInclude": [
    "String"
  ],
  "routesExclude": [
    "String"
  ],
  "splitDNS": [
    "String"
  ],
  "listenPort": 1024,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "lastUpdateDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




