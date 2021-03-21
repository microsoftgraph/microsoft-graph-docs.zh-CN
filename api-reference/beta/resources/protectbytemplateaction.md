---
title: protectByTemplateAction 资源类型
description: 通知应用程序应应用 Azure 信息保护模板。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6524774af3faa496b141e37ec270f8a73770ee63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956825"
---
# <a name="protectbytemplateaction-resource-type"></a>protectByTemplateAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通知应用程序应应用 Azure 信息保护模板。 如果生成的标签已配置为应用保护，[则 evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)或 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)可能会返回 **protectionByTemplateAction。** 使用应用程序必须从结果中读取 templateId，然后使用客户端库（如 Microsoft 信息保护 SDK）通过 Azure 信息保护应用保护。

## <a name="properties"></a>属性

| 属性   | 类型   | 说明                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| templateId | String | 要应用于信息的 Azure 信息保护模板的 GUID。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

