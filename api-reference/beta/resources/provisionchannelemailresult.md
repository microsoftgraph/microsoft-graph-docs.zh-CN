---
title: provisionChannelEmailResult 资源类型
description: 表示频道电子邮件设置操作的结果。
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813229"
---
# <a name="provisionchannelemailresult-resource-type"></a>provisionChannelEmailResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为[频道设置](..\api\channel-provisionemail.md)[的电子邮件地址](channel.md)。

## <a name="properties"></a>属性
| 属性 | 类型   | 说明                               |
| :------- | :----- | :---------------------------------------- |
| email    | String | 表示已设置的电子邮件地址。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
