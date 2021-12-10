---
title: redundancyDetectionSettings 资源类型
description: 电子数据展示案例的冗余设置。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ddd3d06e7d174509cae55fab0542a286fd4c1c70
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403168"
---
# <a name="redundancydetectionsettings-resource-type"></a>redundancyDetectionSettings 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

冗余 (电子数据展示案例的电子邮件线程和) 重复检测设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否启用电子邮件线程和几乎重复检测。|
|maxWords|Int32|指定用于电子邮件线程和几乎重复检测的最大单词数。 若要了解更多信息，请参阅 [最小/最大单词数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|
|minWords|Int32|指定用于电子邮件线程和几乎重复检测的最小单词数。 若要了解更多信息，请参阅 [最小/最大单词数](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|
|similarityThreshold|Int32|指定要放入同一个近重复集的文档的相似性级别。 若要了解更多信息，请参阅文档 [和电子邮件相似性阈值](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading)。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
