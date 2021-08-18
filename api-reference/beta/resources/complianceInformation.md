---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制关联的合规性数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 0b9b7385ae06b01747c0fc1c9c9001add515f43b472c3f7d419374f6e015a8a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253759"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性数据。

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName | string | 合规性认证 (例如 ISO 27018：2014、GDPR、FedRAMP、NIST 800-171)  |
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


