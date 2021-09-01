---
title: certificateConnectorDetails 资源类型
description: 用于检索有关 Intune 证书连接器的信息的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a882591ea334824020bc09af67d102f7fac9aa0e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58822087"
---
# <a name="certificateconnectordetails-resource-type"></a>certificateConnectorDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于检索有关 Intune 证书连接器的信息的实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 certificateConnectorDetailses](../api/intune-raimportcerts-certificateconnectordetails-list.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md) 集合|列出 [certificateConnectorDetails 对象的属性和](../resources/intune-raimportcerts-certificateconnectordetails.md) 关系。|
|[获取 certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-get.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|读取 [certificateConnectorDetails 对象的属性和](../resources/intune-raimportcerts-certificateconnectordetails.md) 关系。|
|[创建 certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-create.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|创建新的 [certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md) 对象。|
|[删除 certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-delete.md)|无|删除 [certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)。|
|[更新 certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-update.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|更新 [certificateConnectorDetails 对象](../resources/intune-raimportcerts-certificateconnectordetails.md) 的属性。|
|[getHealthMetrics 操作](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrics.md)|[keyLongValuePair](../resources/intune-shared-keylongvaluepair.md) 集合|尚未记录|
|[getHealthMetricTimeSeries 操作](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrictimeseries.md)|[certificateConnectorHealthMetricValue](../resources/intune-raimportcerts-certificateconnectorhealthmetricvalue.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此 ConnectorDetails 集的唯一标识符。|
|connectorName|String|连接器名称 (注册期间设置的) 。|
|machineName|字符串|承载此连接器服务的机器的名称。|
|enrollmentDateTime|DateTimeOffset|注册此连接器的日期/时间。|
|lastCheckinDateTime|DateTimeOffset|此连接器上次连接到服务的日期/时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.certificateConnectorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "id": "String (identifier)",
  "connectorName": "String",
  "machineName": "String",
  "enrollmentDateTime": "String (timestamp)",
  "lastCheckinDateTime": "String (timestamp)"
}
```



