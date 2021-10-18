---
title: dataSubject 资源类型
description: 包含与内容搜索主题有关的信息。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: cefcd13dbd36c23cd014979fedce118861b58632
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457735"
---
# <a name="datasubject-resource-type"></a>dataSubject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与内容搜索主题有关的信息。 此资源是开放类型，支持添加添加属性;例如，客户 ID。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|email|String|数据主体的电子邮件。|
|firstName|String|数据主体的名字。|
|lastName|String|数据主体的姓氏。|
|驻留|String|驻留的国家/地区。 驻留信息仅为内部报告提供，而不是用于内容搜索。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dataSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSubject",
  "email": "String",
  "firstName": "String",
  "lastName": "String",
  "residency": "String",
  "SSN": "String"
}
```

