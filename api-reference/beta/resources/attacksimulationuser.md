---
title: attackSimulationUser 资源类型
description: 攻击模拟和培训活动中的用户。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 961a8af1bed831b019f41ddf6a7643ac3b26ab07
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979482"
---
# <a name="attacksimulationuser-resource-type"></a>attackSimulationUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

攻击模拟和培训活动中的用户。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|用户的显示名称。|
|email|字符串|用户的电子邮件地址。|
|userId|字符串|这是表示 **Azure** AD [](../resources/user.md)租户中的用户的用户资源的 id 属性值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationUser",
  "userId": "String",
  "displayName": "String",
  "email": "String"
}
```

