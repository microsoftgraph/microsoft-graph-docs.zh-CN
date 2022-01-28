---
title: teamworkDateTimeConfiguration 资源类型
description: 表示已启用移动设备的Microsoft Teams配置详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489c76f123124aa0b6d6023d5a21dbc780e88a13
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262309"
---
# <a name="teamworkdatetimeconfiguration-resource-type"></a>teamworkDateTimeConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已启用移动设备的Microsoft Teams配置[详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dateFormat|String|设备的日期格式。|
|officeHoursEndTime|TimeOfDay|设备关闭的一天中的时间。|
|officeHoursStartTime|TimeOfDay|设备打开的一天中的时间。|
|timeFormat|String|设备的时间格式。|
|timeZone|String|工作时间所应用到的时区。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDateTimeConfiguration",
  "dateFormat": "String",
  "officeHoursEndTime": "String (time of day)",
  "officeHoursStartTime": "String (time of day)",
  "timeFormat": "String",
  "timeZone": "String"
}
```

