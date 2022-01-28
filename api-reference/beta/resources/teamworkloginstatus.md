---
title: teamworkLoginStatus 资源类型
description: 表示Microsoft Teams Skype for Business设备Exchange登录状态Microsoft Teams登录状态。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460b9bfb341f7b8a564347f0ab4f64d824120d09
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262470"
---
# <a name="teamworkloginstatus-resource-type"></a>teamworkLoginStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Microsoft Teams Skype for Business设备Exchange登录状态Microsoft Teams登录[状态](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|exchangeConnection|[teamworkConnection](../resources/teamworkconnection.md)|有关连接Exchange的信息。|
|skypeConnection|[teamworkConnection](../resources/teamworkconnection.md)|有关连接Skype for Business的信息。|
|teamsConnection|[teamworkConnection](../resources/teamworkconnection.md)|有关连接Teams的信息。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkLoginStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkLoginStatus",
  "exchangeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "teamsConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "skypeConnection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  }
}
```

