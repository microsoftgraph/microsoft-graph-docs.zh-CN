---
title: " complianceInformation 资源类型"
description: 此资源包含合规性与关联数据安全分数控件。
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820599"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

包含合规性与关联数据安全分数控件。

|属性 |类型 |Description |
|:--|:--|:--|
|certificationName | string | 合规性证书名称 (如 ISO 27018:2014，GDPR FedRAMP、 NIST 800 171) |
|certificationControls | [certificationControl](certificationcontrol.md)集合 | 与证书关联的证书控件集合 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
