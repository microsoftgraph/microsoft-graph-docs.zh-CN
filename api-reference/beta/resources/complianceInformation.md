---
title: " complianceInformation 资源类型"
description: 此资源包含与安全分数控制相关的合规性数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507574"
---
#  <a name="complianceinformation-resource-type"></a>complianceInformation 资源类型

命名空间： microsoft. graph

包含与安全得分控制相关联的合规性数据。

|属性 |类型 |说明 |
|:--|:--|:--|
|certificationName | string | 合规性认证名称（例如，ISO 27018:2014、GDPR、FedRAMP、NIST 800-171） |
|certificationControls | [certificationControl](certificationcontrol.md)集合 | 与证书关联的证书控制的集合 |

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
