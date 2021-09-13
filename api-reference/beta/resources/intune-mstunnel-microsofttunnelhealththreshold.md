---
title: microsoftTunnelHealthThreshold 资源类型
description: 表示运行状况指标的运行状况阈值的实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6661fac1b2096f4164d81ce111032a0bb551dfdc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057290"
---
# <a name="microsofttunnelhealththreshold-resource-type"></a>microsoftTunnelHealthThreshold 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示运行状况指标的运行状况阈值的实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftTunnelHealthThresholds](../api/intune-mstunnel-microsofttunnelhealththreshold-list.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 集合|列出 [microsoftTunnelHealthThreshold 对象的属性和](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 关系。|
|[获取 microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-get.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|读取 [microsoftTunnelHealthThreshold 对象的属性和](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 关系。|
|[创建 microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-create.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|创建新的 [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 对象。|
|[删除 microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-delete.md)|无|删除 [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)。|
|[更新 microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-update.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|更新 [microsoftTunnelHealthThreshold 对象](../resources/intune-mstunnel-microsofttunnelhealththreshold.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|指标名称|
|healthyThreshold|Int64|正常运行的阈值|
|unhealthyThreshold|Int64|不正常的阈值|
|defaultHealthyThreshold|Int64|正常运行的默认阈值|
|defaultUnhealthyThreshold|Int64|不正常的默认阈值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelHealthThreshold"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "String (identifier)",
  "healthyThreshold": 1024,
  "unhealthyThreshold": 1024,
  "defaultHealthyThreshold": 1024,
  "defaultUnhealthyThreshold": 1024
}
```



