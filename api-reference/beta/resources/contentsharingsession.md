---
title: contentSharingSession 资源类型
description: 表示调用中的内容共享会话。
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d642350b3fe5e6b1edf5e35dbc3cb5a1f677aea
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917856"
---
# <a name="contentsharingsession-resource-type"></a>contentSharingSession 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示调用中的内容共享会话。

## <a name="methods"></a>方法

| 方法                                                             | 返回类型                                                 | 说明                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [获取 contentSharingSession](../api/contentsharingsession-get.md )                                     | [contentSharingSession](contentsharingsession.md)                                             | 检索 **contentSharingSession 对象的** 属性。                                         |
| [列出 contentSharingSessions](../api/call-list-contentsharingsessions.md )              | [contentSharingSession](contentsharingsession.md) 集合                    | 检索调用中 **contentSharingSession** 对象的列表。                                            |

## <a name="properties"></a>属性

|属性                 |类型                      |说明                                                                        |
|:---                     |:---                      |:---                                                                               |
| id                      | 字符串                   | 内容共享会话的唯一标识符。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentSharingSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentSharingSession",
  "id": "String(identifier)"
}
```
