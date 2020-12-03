---
title: cloudPcStatusDetails 资源类型
description: 云电脑状态的详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563834"
---
# <a name="cloudpcstatusdetails-resource-type"></a>cloudPcStatusDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

云电脑状态的详细信息。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|code|String|与云电脑状态关联的代码。|
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
