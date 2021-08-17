---
title: microsoftTunnelServerLogCollectionResponse 资源类型
description: 存储服务器日志集合状态的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59542a568047fab6103a3af9520a2239ddceaad6ebe97161aefd7d8e49f0042d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178876"
---
# <a name="microsofttunnelserverlogcollectionresponse-resource-type"></a>microsoftTunnelServerLogCollectionResponse 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

存储服务器日志集合状态的实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelServerLogCollectionResponses](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-list.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 集合|列出 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象的属性和关系。|
|[获取 microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-get.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|读取 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象的属性和关系。|
|[创建 microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-create.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|创建新的 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象。|
|[删除 microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-delete.md)|无|删除 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)。|
|[更新 microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-update.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|更新 [microsoftTunnelServerLogCollectionResponse 对象](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一 ID|
|status|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|日志集合的状态。 可取值为：`pending`、`completed`、`failed`。|
|startDateTime|DateTimeOffset|收集的日志的开始时间 |
|endDateTime|DateTimeOffset|收集的日志的结束时间|
|sizeInBytes|Int64|日志的大小（以字节为单位）|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServerLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "sizeInBytes": 1024
}
```




