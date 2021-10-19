---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制执行云应用安全检查的会话控制。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 689b065a6156f009d2425a294aaec8e49c4bee93
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60488610"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>cloudAppSecuritySessionControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于强制执行云应用安全检查的会话控制。 条件访问会话 [控件中的指令](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | 指定是否启用会话控件。 |
|cloudAppSecurityType|cloudAppSecuritySessionControlType| 可取值为：`mcasConfigured`、`monitorOnly`、`blockDownloads`。 若要了解有关这些值的信息，请为特别推荐的应用 [部署条件访问应用控制](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1--configure-your-idp-to-work-with-cloud-app-security)。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

