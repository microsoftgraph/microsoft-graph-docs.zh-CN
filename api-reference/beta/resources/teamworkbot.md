---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 383c646fdb30d082daa73e37fd227238db195b6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706319"
---
# <a name="teamworkbot-resource-type"></a>teamworkBot 资源类型

命名空间：microsoft.graph

表示 Microsoft Teams 生态系统中的机器人。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取自动程序](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|读取团队合作Bot 对象 [的属性和](../resources/teamworkbot.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)相关联的机器人的 ID。 此值通常为 GUID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a>另请参阅

- 若要在团队中安装机器人，请参阅团队 [中的列表应用中的示例](../api/team-list-installedapps.md)2。
- 若要在聊天中安装聊天机器人，请参阅聊天中的 [列表应用中的示例](../api/chat-list-installedapps.md)2。
- 若要在用户的个人范围内安装机器人，请参阅为用户安装 [的列表应用中的示例](../api/userteamwork-list-installedapps.md)2。



