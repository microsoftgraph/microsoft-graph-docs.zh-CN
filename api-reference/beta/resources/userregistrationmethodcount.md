---
title: userRegistrationMethodCount 资源类型
description: 注册身份验证方法的用户数。
author: besiler
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: c505ea408599dbb7b0c6803d03b87b2586d6d0c3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820075"
---
# <a name="userregistrationmethodcount-resource-type"></a>userRegistrationMethodCount 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册身份验证方法的用户数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationMethod|String|身份验证方法的名称。|
|userCount|Int64|注册的用户数。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```
