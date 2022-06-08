---
title: topicModelingSettings 资源类型
description: 电子数据展示案例的主题建模设置
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 865368b2d6d0723a47cc352e64f5400f254b3183
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945148"
---
# <a name="topicmodelingsettings-resource-type"></a>topicModelingSettings 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

主题建模 (电子数据展示案例的主题) 设置。 若要了解详细信息，请参阅 [高级电子数据展示中的配置搜索和分析设置](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|布尔值|若要了解详细信息，请参阅 [动态调整主题的最大数目](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|ignoreNumbers|布尔值|若要了解详细信息，请参阅 [主题中包含数字](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|isEnabled|Boolean|指示是否为案例启用主题。|
|topicCount|Int32|若要了解详细信息，请参阅 [主题的最大数目](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.topicModelingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```

