---
title: teamworkBot 资源类型
description: 生态系统中的自动Microsoft Teams程序。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ccfbb82cace0f9bc38eeb3a5e49a185b12abc99376497bb900e0f150bc39b5c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249102"
---
# <a name="teamworkbot-resource-type"></a>teamworkBot 资源类型

命名空间：microsoft.graph

代表生态系统中的Microsoft Teams程序。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取自动程序](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|读取 [teamworkBot](../resources/teamworkbot.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)关联的机器人的 ID。 此值通常为 GUID。|

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

- 若要在团队中安装机器人，请参阅在团队中[列出应用中的示例 2。](../api/team-list-installedapps.md) <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- 若要在用户的个人范围内安装机器人，请参阅为用户安装的列表 [应用中的示例](../api/userteamwork-list-installedapps.md)2。



