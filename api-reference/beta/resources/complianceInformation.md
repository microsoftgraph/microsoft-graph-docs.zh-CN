---
title: " complianceInformation 资源类型"
description: 此资源包含合规性与关联数据安全分数控件。
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380957"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

包含合规性与关联数据安全分数控件。

|属性 |类型 |说明 |
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
