---
title: publicError 资源类型
description: 表示一般错误及其详细信息。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 4aa4f336ab2b5404e2e82d26f7c38a9ed9b239d2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044291"
---
# <a name="publicerror-resource-type"></a>publicError 资源类型

命名空间：microsoft.graph

表示一般错误及其详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|code|string| 表示错误代码。
|详细信息|[publicErrorDetail](publicerrordetail.md) 集合|错误的详细信息。|
|innerError|[publicInnerError](publicinnererror.md)|内部错误的详细信息。|
|message|字符串| 针对开发人员的非本地化邮件。
|target|String|错误的目标值。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```
