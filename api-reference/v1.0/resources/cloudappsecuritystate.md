---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序（destinationServiceName、destinationServiceIp）的状态信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 116f6a6ccdc65e518ebdb69476d3c3aaea42ab91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533066"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

命名空间：microsoft.graph

包含有关云应用程序（destinationServiceName、destinationServiceIp）的状态信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|字符串|指向云应用程序/服务的连接的目标 IP 地址。|
|destinationServiceName|字符串|云应用程序/服务名称（例如，"Salesforce"、"DropBox" 等）。|
|riskScore|字符串|提供程序生成/计算的风险分数（云应用程序/服务）。 建议的值范围为0-1，这相当于一个百分比。|

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
