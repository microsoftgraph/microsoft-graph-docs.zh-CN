---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制关联的符合性数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 9d65043ca09ce945bbc87b83bfe2ec84d7f512bb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944925"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性数据。

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName | string | 符合性认证名称 (例如 ISO 27018：2014、GDPR、FedRAMP、NIST 800-171)  |
|certificationControls | [certificationControl](certificationcontrol.md) 集合 | 与认证关联的认证控件的集合 |

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


