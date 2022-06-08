---
title: ediscoveryCaseSettings 资源类型
description: 包含电子数据展示事例的设置。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 76ec63befe49601e404c3d2dc21e8832cd82ed8c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945310"
---
# <a name="ediscoverycasesettings-resource-type"></a>ediscoveryCaseSettings 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含电子数据展示事例的设置。 有关详细信息，请参阅 [高级电子数据展示中的配置搜索和分析设置](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 ediscoveryCaseSettings](../api/security-ediscoverycasesettings-get.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|读取 [ediscoveryCaseSettings 对象的](../resources/security-ediscoverycasesettings.md) 属性和关系。|
|[更新 ediscoveryCaseSettings](../api/security-ediscoverycasesettings-update.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|更新 [ediscoveryCaseSettings 对象的](../resources/security-ediscoverycasesettings.md) 属性。|
|[resetToDefault](../api/security-ediscoverycasesettings-resettodefault.md)|无|将所有设置重置为默认值。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|电子数据展示案例的 ID。 继承自 [entity](../resources/entity.md)。|
|Ocr|[microsoft.graph.security.ocrSettings](../resources/security-ocrsettings.md)|OCR (光学字符识别) 事例的设置。|
|redundancyDetection|[microsoft.graph.security.redundancyDetectionSettings](../resources/security-redundancydetectionsettings.md)|冗余 (几乎重复和电子邮件线程) 检测设置的情况下。|
|topicModeling|[microsoft.graph.security.topicModelingSettings](../resources/security-topicmodelingsettings.md)|主题建模 (主题) 案例设置。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCaseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.security.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.security.ocrSettings"
  }
}
```

