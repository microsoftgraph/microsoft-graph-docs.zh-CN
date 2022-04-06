---
title: teamInfo 资源类型
description: 表示具有基本信息的团队。
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e2d683428dae15a0b51989906dbb9ecac16b945
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685339"
---
# <a name="teaminfo-resource-type"></a>teamInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示具有基本信息的 [团队](team.md) 。

[associatedTeamInfo](associatedteaminfo.md) 和 [sharedWithChannelTeamInfo](sharedwithchannelteaminfo.md) 的基础类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|团队的名称。|
|tenantId|字符串|Azure Active Directory租户的 ID。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```
