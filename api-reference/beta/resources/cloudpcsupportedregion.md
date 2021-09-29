---
title: cloudPcSupportedRegion 资源类型
description: 表示一个支持的区域，用于为云电脑建立本地网络连接。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 150138b8be51fd8b333cb100aaa65dbbcd8bdfc6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997230"
---
# <a name="cloudpcsupportedregion-resource-type"></a>cloudPcSupportedRegion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个支持的区域，用于为云电脑建立本地网络连接。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcSupportedRegions](../api/virtualendpoint-list-supportedregions.md)|[cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) 集合|列出可用于创建云电脑连接的受支持区域。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|受支持区域的唯一标识符。 只读。|
|displayName|字符串|支持区域的名称。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSupportedRegion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSupportedRegion",
  "id": "String (identifier)",
  "displayName": "String"
}
```
