---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f5b82357d91889aada97c835fcab2c327c05fe143988a9ed3bf47ee293687770
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253766"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

命名空间：microsoft.graph

包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|与云应用程序/服务的连接的目标 IP 地址。|
|destinationServiceName|字符串|云应用程序/服务 (例如"Salesforce"、"DropBox"等) 。|
|riskScore|String|云应用程序/服务的提供商生成/计算的风险评分。 建议的值范围为 0-1，等于百分比。|

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


