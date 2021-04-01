---
title: teamworkActivityTopic 资源类型
description: 表示活动源通知的主题。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473993"
---
# <a name="teamworkactivitytopic-resource-type"></a>teamworkActivityTopic 资源类型

命名空间：microsoft.graph

表示活动源通知的主题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|source|teamworkActivityTopicSource|源的类型。 可取值为：`entityUrl`、`text`。 对于支持的 Microsoft Graph URL，请使用 `entityUrl` 。 对于自定义文本，请使用 `text` 。|
|value|String|主题值。 如果源 **属性的值为** `entityUrl` ，则它必须是 Microsoft Graph URL。 如果模块是 `text` ，则它必须是纯文本值。|
|webUrl|String|用户在选择通知时单击的链接。 当 **source** 为 `entityUrl` 时可选;当 **source** 为 时为 必需 `text` 。|

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

