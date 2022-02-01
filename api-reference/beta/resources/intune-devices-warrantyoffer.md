---
title: warrantyOffer 资源类型
description: 帐户中托管设备型号和制造商的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f8045dcc99c2c9e28099a39e54baa1e0561b5d2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292357"
---
# <a name="warrantyoffer-resource-type"></a>warrantyOffer 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户中托管设备型号和制造商的元数据

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|[warrantyType](../resources/intune-devices-warrantytype.md)|担保产品/服务类型。 可取值为：`unknown`、`manufacturer`、`contractual`、`unknownFutureValue`。|
|description|String|担保产品/服务说明|
|startDateTime|DateTimeOffset|担保产品/服务开始日期|
|endDateTime|DateTimeOffset|担保产品/服务结束日期|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.warrantyOffer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.warrantyOffer",
  "type": "String",
  "description": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```




