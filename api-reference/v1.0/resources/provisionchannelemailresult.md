---
title: provisionChannelEmailResult 资源类型
description: 表示频道电子邮件设置操作的结果。
author: anandab-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d33ebbc5e5584a8969eed6f97bf7f26042e92478
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763694"
---
# <a name="provisionchannelemailresult-resource-type"></a>provisionChannelEmailResult 资源类型

命名空间：microsoft.graph

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
