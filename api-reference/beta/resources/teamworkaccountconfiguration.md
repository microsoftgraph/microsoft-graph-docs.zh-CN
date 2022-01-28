---
title: teamworkAccountConfiguration 资源类型
description: 表示有关新设备的帐户Microsoft Teams 会议室的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b3fc0edb85380f8a858bf6b9910a819443bfb8b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262337"
---
# <a name="teamworkaccountconfiguration-resource-type"></a>teamworkAccountConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关新设备的帐户配置Microsoft Teams 会议室[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|onPremisesCalendarSyncConfiguration|[teamworkOnPremisesCalendarSyncConfiguration](../resources/teamworkonpremisescalendarsyncconfiguration.md)|用于同步日历的帐户。|
|supportedClient|teamworkSupportedClient|支持的设备Teams 会议室客户端。 可能的值包括 `unknown`、`skypeDefaultAndTeams`、`teamsDefaultAndSkype`、`skypeOnly`、`teamsOnly`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkAccountConfiguration",
  "onPremisesCalendarSyncConfiguration": {
    "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
  },
  "supportedClient": "String"
}
```

