---
title: cloudPcLoginResult 资源类型
description: 表示结果中云电脑设备的详细信息。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b0ab1d22d5eabeaed84e8ee0d15f9527d64387e7
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391114"
---
# <a name="cloudpcloginresult-resource-type"></a>cloudPcLoginResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示结果中云电脑设备的详细信息。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|time|DateTimeOffSet|云电脑运行的时间。 时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。 例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLoginResult",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLoginResult",
  "time": "String (timestamp)"
}
```
