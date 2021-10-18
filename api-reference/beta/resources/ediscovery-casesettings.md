---
title: caseSettings 资源类型
description: 包含电子数据展示案例的 ettings。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 97b79952653c33d614276ca57c4b726a97cd9be4
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446454"
---
# <a name="casesettings-resource-type"></a>caseSettings 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含电子数据展示案例的设置。 有关详细信息，请参阅配置[搜索和分析Advanced eDiscovery。](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 caseSettings](../api/ediscovery-casesettings-get.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|读取 [microsoft.graph.ediscovery.caseSettings 对象的属性和](../resources/ediscovery-casesettings.md) 关系。|
|[Update caseSettings](../api/ediscovery-casesettings-update.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|更新 [microsoft.graph.ediscovery.caseSettings 对象](../resources/ediscovery-casesettings.md) 的属性。|
|[resetToDefault](../api/ediscovery-casesettings-resettodefault.md)|无|将所有设置重置为默认值。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|Id|String|电子数据展示案例的 ID。 继承自 [实体](../resources/entity.md)。|
|ocr|[microsoft.graph.ediscovery.ocrSettings](../resources/ediscovery-ocrsettings.md)|OCR (光学字符识别) 大小写的设置。|
|redundancyDetection|[microsoft.graph.ediscovery.redundancyDetectionSettings](../resources/ediscovery-redundancydetectionsettings.md)|冗余 (复制和电子邮件线程) 案例的检测设置。|
|topicModeling|[microsoft.graph.ediscovery.topicModelingSettings](../resources/ediscovery-topicmodelingsettings.md)|主题建模 (主题) 大小写设置。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseSettings",
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
