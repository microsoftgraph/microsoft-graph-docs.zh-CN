---
title: teamworkActivityTopic 资源类型
description: 代表活动源通知的主题。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377522"
---
# <a name="teamworkactivitytopic-resource-type"></a>teamworkActivityTopic 资源类型

命名空间：microsoft.graph

代表活动源通知的主题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|source|teamworkActivityTopicSource|源的类型。 可取值为：`entityUrl`、`text`。 若要获取受支持的 Microsoft Graph Url，请使用 `entityUrl` 。 对于自定义文本，请使用 `text` 。|
|value|String|主题值。 如果 **source** 属性的值为，则 `entityUrl` 它必须是 Microsoft Graph URL。 如果 vaule 为 `text` ，则它必须为纯文本值。|
|WebUrl|String|用户在选择通知时单击的链接。 **源** 为时 `entityUrl` 为可选;**源** 为时为必需 `text` 。|

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

