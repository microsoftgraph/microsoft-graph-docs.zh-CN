---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 00447f134b2c54bdda92857c6c84c05e8c52b3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018933"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间：microsoft.graph

包含与安全得分控制相关联的合规性数据。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName|String| 合规性认证名称 (例如，ISO 27018:2014、GDPR、FedRAMP、NIST 800-171)  |
|certificationControls|[certificationControl](certificationcontrol.md) 集合|与证书关联的证书控制的集合|

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
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

