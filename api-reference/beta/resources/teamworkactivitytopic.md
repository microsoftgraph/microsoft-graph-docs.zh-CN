---
title: teamworkActivityTopic 资源类型
description: 表示活动源通知的主题。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe34a16382d3a2e806fd0c95fe9d09d55c3e2dbea4f3cea1e7d861f05f9af1b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185465"
---
# <a name="teamworkactivitytopic-resource-type"></a>teamworkActivityTopic 资源类型

命名空间：microsoft.graph

表示活动源通知的主题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|source|teamworkActivityTopicSource|源的类型。 可取值为：`entityUrl`、`text`。 对于支持的 Microsoft Graph URL，请使用 `entityUrl` 。 对于自定义文本，请使用 `text` 。|
|value|String|主题值。 如果源 **属性的值为** `entityUrl` ，则它必须是 Microsoft Graph URL。 如果模块是 `text` ，则它必须是纯文本值。|
|WebUrl|String|用户在选择通知时单击的链接。 当 **source** 为 `entityUrl` 时可选;当 **source** 为 时为 必需 `text` 。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

