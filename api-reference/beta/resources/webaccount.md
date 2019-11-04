---
title: webAccount 资源类型
description: webAccount 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 414e3f491736f51ee670390519241110bc81f66e
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950353"
---
# <a name="webaccount-resource-type"></a>webAccount 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户已将其添加到其用户[配置文件](profile.md)中的 web 帐户。

此资源类型继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                     | 返回类型                 | 说明                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [获取 webAccount](../api/webaccount-get.md) | [webAccount](webaccount.md) | 读取**webAccount**对象的属性和关系。 |
| [更新 webAccount](../api/webaccount-update.md)      | [webAccount](webaccount.md) | 更新**webAccount**对象。                               |
| [删除 webAccount](../api/webaccount-delete.md)      | 无                        | 删除**webAccount**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型                                      | 说明                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|说明   |字符串                                     | 包含用户为所引用服务上的帐户提供的说明。|
|service       |[serviceInformation](serviceinformation.md)| 包含有关要关联的服务的基本详细信息。                              |
|statusMessage |String                                     | 包含来自云服务的状态邮件（如果提供或已同步）。                  |
|userId        |String                                     | 为 webaccount 显示的用户名。                                    |
|webUrl        |String                                     | 包含指向云服务上的用户配置文件的链接（如果存在）。                       |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
