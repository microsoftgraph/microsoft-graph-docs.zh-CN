---
title: userRegistrationMethodCount 资源类型
description: 为身份验证方法注册的用户数。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 8e4c19c48771ccd0bd1dd1f1a4b049334266834a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132930"
---
# <a name="userregistrationmethodcount-resource-type"></a>userRegistrationMethodCount 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为身份验证方法注册的用户数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationMethod|字符串|身份验证方法的名称。|
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
