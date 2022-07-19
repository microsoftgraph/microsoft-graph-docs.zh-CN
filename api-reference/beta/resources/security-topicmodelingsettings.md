---
title: topicModelingSettings 资源类型
description: 表示电子数据展示案例的主题建模设置
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1c056b15217aa1cff55f3303a83cb5f22ead930d
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838218"
---
# <a name="topicmodelingsettings-resource-type"></a>topicModelingSettings 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示主题建模 (主题) 电子数据展示案例的设置。 若要了解详细信息，请参阅电子数据 [展示 (高级) 中配置搜索和分析设置 ](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)。


## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Boolean|指示主题模型是否应动态优化生成的主题数。 若要了解详细信息，请参阅 [动态调整主题的最大数目](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|ignoreNumbers|Boolean|指示主题模型在分析文档文本时是否应排除数字。 若要了解详细信息，请参阅 [主题中包含数字](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|isEnabled|Boolean|指示是否为案例启用主题模型。|
|topicCount|Int32|主题模型将为审阅集生成的主题总数。 若要了解详细信息，请参阅 [主题的最大数目](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|

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

