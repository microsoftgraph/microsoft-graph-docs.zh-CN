---
title: cloudAppSecurityState 资源类型
description: 包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045900"
---
# <a name="cloudappsecuritystate-resource-type"></a>cloudAppSecurityState 资源类型

包含状态信息的云应用程序 （destinationServiceName、 destinationServiceIp）。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationServiceIp|字符串|连接到云应用程序/服务的目标 IP 地址。|
|destinationServiceName|字符串|云应用程序/服务名称 （例如"销售"、"收存箱"等）。|
|riskScore|字符串|带有提供程序生成/计算风险分数的云应用程序/服务。 建议值的范围为 0-1，这相当于百分比。|

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