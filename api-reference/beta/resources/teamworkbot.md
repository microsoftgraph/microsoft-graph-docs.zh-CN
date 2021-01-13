---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c21e7ab3b88c2659bf055e39b931cbc6e9d2f39
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844674"
---
# <a name="teamworkbot-resource-type"></a>teamworkBot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft Teams 生态系统中的机器人。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取机器人](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|读取团队合作Bot 对象 [的属性和](../resources/teamworkbot.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)相关联的机器人的 ID。 此值通常为 GUID。|

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

- 若要在团队中安装机器人，请参阅团队中的[列表应用中的示例 2。](../api/team-list-installedapps.md)
- 若要在聊天中安装聊天机器人，请参阅聊天中的 [列表应用中的示例](../api/chat-list-installedapps.md)2。
- 若要在用户的个人范围内安装机器人，请参阅为用户安装 [的列表应用中的示例](../api/userteamwork-list-installedapps.md)2。



