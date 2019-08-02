---
title: complianceInformation 资源类型
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032856"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

包含与安全得分控制相关联的合规性数据。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName|String| 合规性认证名称 (例如, ISO 27018:2014、GDPR、FedRAMP、NIST 800-171) |
|certificationControls|[certificationControl](certificationcontrol.md)集合|与证书关联的证书控制的集合|

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
