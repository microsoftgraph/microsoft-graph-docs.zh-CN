---
title: incomingCallOptions 资源类型
description: 表示包含传入调用选项的类。
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 700f0139f79415b264544d60386f8b7dba5dc24e
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917815"
---
# <a name="incomingcalloptions-resource-type"></a>incomingCallOptions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示包含传入调用选项的类。

继承自 [callOptions](calloptions.md)。

## <a name="properties"></a>属性

|属性                 |类型                      |说明                                                                        |
|:---                     |:---                      |:---                                                                               |
|isContentSharingNotificationEnabled   |Boolean                   |指示是否应为调用启用内容共享通知的值。 继承自 [callOptions](calloptions.md)。    |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.incomingCallOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incomingCallOptions",
  "isContentSharingNotificationEnabled": "Boolean"
}
```
