---
title: cloudAppSecurityState 资源类型
description: 包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d04a23bb38c9f5264057d56d43de0f053dd58b9c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118755"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

命名空间：microsoft.graph

包含有关云应用程序的状态信息 (destinationServiceName、destinationServiceIp) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|String|与云应用程序/服务的连接的目标 IP 地址。|
|destinationServiceName|String|云应用程序/服务名称 (例如"Salesforce"、"DropBox"等) 。|
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

