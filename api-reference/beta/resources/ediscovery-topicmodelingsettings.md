---
title: topicModelingSettings 资源类型
description: 电子数据展示案例的主题建模设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bd433de0aa88298961366f50425706e1af4bffde
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080741"
---
# <a name="topicmodelingsettings-resource-type"></a>topicModelingSettings 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

主题建模 (电子) 展示案例的主题设置。 若要了解更多信息，请参阅配置[搜索和分析Advanced eDiscovery。](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Boolean|若要了解更多信息，请参阅 [动态调整最大主题数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|ignoreNumbers|Boolean|若要了解更多信息，请参阅 [在主题中包括数字](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|
|isEnabled|Boolean|指示是否针对案例启用主题。|
|topicCount|Int32|若要了解更多信息，请参阅 [主题的最大数量](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```
