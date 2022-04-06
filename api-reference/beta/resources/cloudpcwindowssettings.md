---
title: cloudPcWindowsSettings 资源类型
description: 表示在创建Windows策略的云电脑时要配置的特定策略设置。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3a58fe434e73402f9d69902c58da5f20f78c5a89
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722624"
---
# <a name="cloudpcwindowssettings-resource-type"></a>cloudPcWindowsSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在创建Windows策略的云电脑时要配置的特定策略设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|language|String|要Windows语言包配置和云电脑本地化的组语言/区域标记。 默认值为 ， `en-US`它对应于美国 (英语) 。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcWindowsSettings",
  "language": "String"
}
```
