---
title: teamworkConnection 资源类型
description: 表示有关已启用Microsoft Teams设备及其外围设备的连接状态的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a02096ce1a807d4d75db5ba12b40488ef268bb36
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262307"
---
# <a name="teamworkconnection-resource-type"></a>teamworkConnection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用[Microsoft Teams设备及其](../resources/teamworkdevice.md)外围设备的连接状态的详细信息。
当你计算设备运行状况时，连接状态非常有用，因为当所需的外围设备未正确连接时，设备运行状况将发生更改至关键状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connectionStatus|teamworkConnectionStatus|指示组件/外设是否已连接/断开连接或其状态未知。 可能的值包括 `unknown`、`connected`、`disconnected`、`unknownFutureValue`。|
|lastModifiedDateTime|DateTimeOffset|上次更改状态的时间。 例如，指示从 _状态为_ `connected` 时开始连接，自状态为 后断开连接`disconnected`。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConnection",
  "connectionStatus": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

