---
title: teamworkActivityTopic 资源类型
description: 表示活动源通知的主题。
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 721553521d202788f894381650ccf8e45c364805
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122955"
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

