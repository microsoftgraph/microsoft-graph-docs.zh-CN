---
title: '电子数据展示 (设置资源) '
description: 设置电子数据展示案例
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9f0248fa0c6080a143272d997b9d6125e0ccb5a2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080742"
---
# <a name="settings-resource-type-ediscovery"></a>电子数据展示 (设置资源) 

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置电子数据展示案例的条目。 有关详细信息，请参阅配置[搜索和分析Advanced eDiscovery。](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取设置](../api/ediscovery-settings-get.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|读取 [microsoft.graph.ediscovery.settings 对象的属性和](../resources/ediscovery-settings.md) 关系。|
|[更新设置](../api/ediscovery-settings-update.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|更新 [microsoft.graph.ediscovery.settings 对象](../resources/ediscovery-settings.md) 的属性。|
|[resetToDefault](../api/ediscovery-settings-resettodefault.md)|无|将所有设置重置为默认值。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|Id|String|电子数据展示案例的 ID。 继承自 [实体](../resources/entity.md)。|
|ocr|[microsoft.graph.ediscovery.ocrSettings](../resources/ediscovery-ocrsettings.md)|OCR (光学字符识别) 大小写设置。|
|redundancyDetection|[microsoft.graph.ediscovery.redundancyDetectionSettings](../resources/ediscovery-redundancydetectionsettings.md)|冗余 (复制和电子邮件线程) 情况检测设置。|
|topicModeling|[microsoft.graph.ediscovery.topicModelingSettings](../resources/ediscovery-topicmodelingsettings.md)|主题建模 (主题) 案例的设置。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.settings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.settings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
  }
}
```
