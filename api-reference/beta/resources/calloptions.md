---
title: callOptions 资源类型
description: 包含调用的可选功能的抽象基类。
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 53d845d7667f04f5b028fdde01b2658e578a7a25
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917851"
---
# <a name="calloptions-resource-type"></a>callOptions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含调用的可选功能的抽象基类。

## <a name="properties"></a>属性

|属性                 |类型                      |说明                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |指示是否应为调用启用内容共享通知。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
