---
title: associatedTeamInfo 资源类型
description: 表示与用户关联的团队。
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2e3c8c83d10d5c15595edf9aef8f0b3b50e661e4
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685409"
---
# <a name="associatedteaminfo-resource-type"></a>associatedTeamInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与[用户](../resources/user.md)关联的[团队](team.md)。 目前， [用户](../resources/user.md) 可以通过两种不同的方式与 [团队](../resources/team.md) 关联：
* [用户](../resources/user.md)可以是[团队](../resources/team.md)的直接成员。
* [用户](../resources/user.md)可以是托管在[团队](../resources/team.md)中的共享[频道](../resources/channel.md)的成员。



继承自 [teamInfo](../resources/teaminfo.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 associatedTeamInfo](../api/associatedteaminfo-list.md)|[associatedTeamInfo](../resources/associatedteaminfo.md) 集合|获取 [associatedTeamInfo](../resources/associatedteaminfo.md) 对象及其属性的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|团队的名称。 继承自 [teamInfo](../resources/teaminfo.md)。|
|tenantId|String|Azure Active Directory租户的 ID。 继承自 [teamInfo](../resources/teaminfo.md)。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.associatedTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```

## <a name="see-also"></a>另请参阅
- [获取团队](../api/team-get.md)