---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bc87f30a970f305a309a320030cde419961660f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794615"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a>mobileAppTroubleshootingHistoryItem 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动应用故障排除事件中包含的历史记录项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|历史记录项目发生的时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```



