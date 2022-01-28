---
title: teamworkTeamsClientConfiguration 资源类型
description: 表示在 Microsoft Teams 设备上运行的 Microsoft Teams 会议室 配置详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 46c1ac98c9992df65441dd3b92e12f81ae8804b0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262494"
---
# <a name="teamworkteamsclientconfiguration-resource-type"></a>teamworkTeamsClientConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 Microsoft Teams 设备上运行的 Microsoft Teams 会议室 [配置详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountConfiguration|[teamworkAccountConfiguration](../resources/teamworkaccountconfiguration.md)|设备的Microsoft Teams客户端用户帐户的配置。|
|featuresConfiguration|[teamworkFeaturesConfiguration](../resources/teamworkfeaturesconfiguration.md)|设备Microsoft Teams客户端功能的配置。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTeamsClientConfiguration",
  "accountConfiguration": {
    "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
  },
  "featuresConfiguration": {
    "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
  }
}
```

