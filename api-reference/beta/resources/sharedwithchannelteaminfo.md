---
title: sharedWithChannelTeamInfo 资源类型
description: 表示与频道共享的团队。
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15f6e3138d24bf93a2546be404c21e6bcf4b6daa
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060998"
---
# <a name="sharedwithchannelteaminfo-resource-type"></a>sharedWithChannelTeamInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与之共享频道的[团队](team.md)的信息。 可以与一个[团队](team.md)共享多个频道。


继承自 [teamInfo](../resources/teaminfo.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-list.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) 集合|获取 [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) 对象及其属性的列表。|
|[Get sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|读取 [authenticationFlowsPolicy](../resources/sharedwithchannelteaminfo.md) 对象的属性和关系。|
|[Delete sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-delete.md)|无|删除 [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) 对象。|
|[列出 allowedMembers](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|[conversationMember](../resources/conversationmember.md) 集合|获取有权访问共享频道的团队成员的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|团队的名称。 继承自 [teamInfo](../resources/teaminfo.md)。|
|isHostTeam|Boolean|指示[团队](team.md)是否是[频道](channel.md)的主持人。|
|tenantId|字符串|Azure Active Directory 租户 ID。 继承自 [teamInfo](../resources/teaminfo.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|allowedMembers|[conversationMember](../resources/conversationmember.md) 集合|有权访问共享频道的团队成员的集合。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "isHostTeam": "Boolean",
  "tenantId": "String"
}
```

