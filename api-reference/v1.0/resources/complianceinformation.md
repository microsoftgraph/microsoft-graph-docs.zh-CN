---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制关联的合规性数据。
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 05ba1b7900f50474e2eaaac64326f02eeadfd913
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109260"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性数据。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName|String| 合规性认证 (例如 ISO 27018：2014、GDPR、FedRAMP、NIST 800-171)  |
|certificationControls|[certificationControl](certificationcontrol.md) 集合|与认证关联的认证控制措施的集合|

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

