---
title: microsoftTunnelSite 资源类型
description: 表示 Microsoft 隧道站点的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 730d0075009b605db5e132412bddfbf0f58251a6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301565"
---
# <a name="microsofttunnelsite-resource-type"></a>microsoftTunnelSite 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Microsoft 隧道站点的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 集合|列出 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象的属性和关系。|
|[获取 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|读取 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象的属性和关系。|
|[创建 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|创建新的 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。|
|[删除 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|无|删除 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)。|
|[更新 microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|更新 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|MicrosoftTunnelSite 的 Id|
|displayName|字符串|MicrosoftTunnelSite 的显示名称|
|description|字符串|MicrosoftTunnelSite 的说明|
|publicAddress|字符串|MicrosoftTunnelSite 的公共域名或 IP 地址|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|已应用于此 MicrosoftTunnelSite 的 MicrosoftTunnelConfiguration|
|microsoftTunnelServers|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 集合|注册到此 MicrosoftTunnelSite 的 MicrosoftTunnelServers 的列表|

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
  "roleScopeTagIds": [
    "String"
  ]
}
```




