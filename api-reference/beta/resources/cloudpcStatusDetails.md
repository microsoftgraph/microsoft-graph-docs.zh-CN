---
title: cloudPcStatusDetails 资源类型
description: 云电脑状态的详细信息。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 28735467ef1bc233f5ba6d5ecc3144d64e31df3e
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780896"
---
# <a name="cloudpcstatusdetails-resource-type"></a>cloudPcStatusDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

云电脑状态的详细信息。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|code|字符串|与云电脑状态相关联的代码。|
|message|String|状态消息。|
|additionalInformation|[KeyValuePair](../resources/keyvaluepair.md) 集合|有关云电脑状态的其他信息。|

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
