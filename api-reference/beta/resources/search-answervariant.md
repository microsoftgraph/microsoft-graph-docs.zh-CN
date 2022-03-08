---
title: answerVariant 资源类型
description: 应答变量可用于根据国家/地区或平台更改搜索答案的某些属性。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 99d196273ae772091f236b18d2821288f63eefe9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338372"
---
# <a name="answervariant-resource-type"></a>answerVariant 资源类型

命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

应答变量可用于根据国家/地区或平台更改搜索答案的某些字段。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|搜索结果页上显示的应答变体说明。|
|displayName|String|搜索结果中显示的应答变体名称。|
|webUrl|String|应答变体 URL 链接。 当用户在搜索结果中单击此答案变体时，他们将转到此 URL。|
|languageTags|String collection|可查看此搜索答案的一个或多个国家/地区列表。|
|平台|microsoft.graph.platform 集合|能够查看此答案变体的设备和操作系统列表。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerVariant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerVariant",
  "displayName": "String",
  "webUrl": "String",
  "description": "String",
  "languageTags": ["String"],
  "platforms": ["String"]
}
```

