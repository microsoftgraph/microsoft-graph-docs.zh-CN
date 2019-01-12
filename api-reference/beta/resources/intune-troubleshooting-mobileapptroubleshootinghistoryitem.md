---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 713bf06c65bd8d651e1d885d41876822d62eade1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947237"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a>mobileAppTroubleshootingHistoryItem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

移动应用程序疑难解答事件中包含的历史记录项。
## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|历史记录项所发生的时间。|

## <a name="relationships"></a>Relationships
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





