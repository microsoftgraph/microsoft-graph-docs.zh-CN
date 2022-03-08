---
title: cloudPcRestorePointSetting 资源类型
description: 表示时间点还原的特定设置。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e49cebd6f3bcb9a6af0ac469608b4c54081a7d8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338343"
---
# <a name="cloudpcrestorepointsetting-resource-type"></a>cloudPcRestorePointSetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑的时间点还原设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|frequencyInHours|Int32|自动获取云电脑 (还原) 的时间间隔（以小时为单位）。 可能的值是 、`4``6`、`12`、`16`和 `24`。 默认频率为 12 小时。|
|userRestoreEnabled|Boolean|如果 `true`为 ，则用户能够使用快照还原云电脑。 如果 `false`为 ，非管理员用户无法使用快照还原云电脑。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRestorePointSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRestorePointSetting",
  "frequencyInHours": "Integer",
  "userRestoreEnabled": "Boolean"
}
```
