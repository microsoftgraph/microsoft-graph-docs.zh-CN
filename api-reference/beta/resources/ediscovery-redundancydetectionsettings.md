---
title: redundancyDetectionSettings 资源类型
description: 电子数据展示案例的冗余设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fd1ca1ea3faf03e2639896c79acd0629931c71c9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080745"
---
# <a name="redundancydetectionsettings-resource-type"></a>redundancyDetectionSettings 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

冗余 (电子数据展示案例的电子邮件线程和) 重复检测设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否启用电子邮件线程和几乎重复检测。|
|maxWords|Int32|有关详细信息 [，请参阅最小/最大](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 单词数。|
|minWords|Int32|有关详细信息 [，请参阅最小/最大](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 单词数。|
|similarityThreshold|Int32|有关详细信息 [，请参阅文档和电子邮件相似性](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) 阈值。|

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
