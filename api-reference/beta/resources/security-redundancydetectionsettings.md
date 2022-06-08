---
title: redundancyDetectionSettings 资源类型
description: 电子数据展示案例的冗余设置。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8fcc425c95540552479cfd07b862e5e9ba29e53e
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945153"
---
# <a name="redundancydetectionsettings-resource-type"></a>redundancyDetectionSettings 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

冗余 (电子数据展示案例的电子邮件线程和近乎重复的检测) 设置。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否启用电子邮件线程和近乎重复的检测。|
|maxWords|Int32|指定用于电子邮件线程和近乎重复检测的最大字词数。 若要了解详细信息，请参阅 [最小/最大单词数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|
|minWords|Int32|指定用于电子邮件线程和几乎重复检测的字词的最小数目。 若要了解详细信息，请参阅 [最小/最大单词数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|
|similarityThreshold|Int32|指定要放入相同近重复集的文档的相似性级别。 若要了解详细信息，请参阅 [文档和电子邮件相似性阈值](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```

