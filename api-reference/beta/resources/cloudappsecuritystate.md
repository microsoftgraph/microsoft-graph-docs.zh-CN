---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 82046f855f3ce8d994c3b212b1513098e1c042ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034054"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

命名空间：microsoft.graph

包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|指向云应用程序/服务的连接的目标 IP 地址。|
|destinationServiceName|String|云应用程序/服务名称 (例如 "Salesforce"、"DropBox" 等 ) 。|
|riskScore|String|提供程序生成/计算的风险分数（云应用程序/服务）。 建议的值范围为0-1，这相当于一个百分比。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


