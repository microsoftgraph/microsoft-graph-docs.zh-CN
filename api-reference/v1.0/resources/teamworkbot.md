---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99bdde9a4ff26945dd5aa040f2741fdf50c1273b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476408"
---
# <a name="teamworkbot-resource-type"></a>teamworkBot 资源类型

命名空间：microsoft.graph

表示 Microsoft Teams 生态系统中的机器人。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取自动程序](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|读取团队合作Bot 对象 [的属性](../resources/teamworkbot.md) 和关系。|

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

- 若要在团队中安装机器人，请参阅团队中 [列表应用的示例](../api/team-list-installedapps.md)2。 <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- 若要在用户的个人范围内安装自动程序，请参阅为用户安装的列表 [应用中的示例](../api/userteamwork-list-installedapps.md)2。



