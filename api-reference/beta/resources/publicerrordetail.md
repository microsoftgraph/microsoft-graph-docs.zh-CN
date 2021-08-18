---
title: publicErrorDetail 资源类型
description: 表示错误的详细信息。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d629816bb8d06065ed74a1ff8d19638a2a84a2d964945882ec0cf57a3c7d2a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226130"
---
# <a name="publicerrordetail-resource-type"></a>publicErrorDetail 资源类型

命名空间：microsoft.graph

表示 [publicError 或](../resources/publicerror.md) [publicInnerError 的详细信息](../resources/publicinnererror.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|code|String|错误代码。|
|message|String|错误消息。|
|target|String|错误的目标值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```

