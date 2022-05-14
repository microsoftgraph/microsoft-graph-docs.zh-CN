---
title: cloudAppSecurityState 资源类型
description: 包含有关 cloud 应用程序 (destinationServiceName，destinationServiceIp) 的有状态信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: d509aa92fafb3848a5bb77c5f4fb1b0674d66f31
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420752"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

命名空间：microsoft.graph

包含有关 cloud 应用程序 (destinationServiceName，destinationServiceIp) 的有状态信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|连接到云应用程序/服务的目标 IP 地址。|
|destinationServiceName|String|云应用程序/服务名称 (，例如“Salesforce”、“DropBox”等) 。|
|riskScore|String|云应用程序/服务的提供程序生成/计算风险分数。 建议的值范围为 0-1，这等同于百分比。|

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


