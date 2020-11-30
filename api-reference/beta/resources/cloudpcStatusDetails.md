---
title: cloudPcStatusDetails 资源类型
description: 云电脑状态的详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378327"
---
# <a name="cloudpcstatusdetails-resource-type"></a>cloudPcStatusDetails 资源类型

命名空间：microsoft.graph

云电脑状态的详细信息。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|code|字符串|与云电脑状态关联的代码。|
|message|String|状态邮件。|
|additionalInformation|[KeyValuePair](../resources/keyvaluepair.md) 集合|有关云电脑状态的任何其他信息。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
