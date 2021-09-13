---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制关联的合规性数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d5d59735dd8dc3dac96607bfc012f127283ca966
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023750"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性数据。

|属性 |类型 |描述 |
|:--|:--|:--|
|certificationName | 字符串 | 合规性认证 (例如 ISO 27018：2014、GDPR、FedRAMP、NIST 800-171)  |
|certificationControls | [certificationControl](certificationcontrol.md) 集合 | 与认证关联的认证控制措施的集合 |

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


