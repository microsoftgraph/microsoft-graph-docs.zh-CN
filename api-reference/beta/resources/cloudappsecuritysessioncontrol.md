---
title: cloudAppSecuritySessionControl 资源类型
description: 用于强制执行云应用安全检查的会话控制。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 630c558981b3dc9bbb0ec48c9a81ff74868c43bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941829"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>cloudAppSecuritySessionControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于强制执行云应用安全检查的会话控制。 条件访问会话 [控件中的指令](conditionalaccesssessioncontrol.md)。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | 指定是否启用会话控件。 |
|cloudAppSecurityType|cloudAppSecuritySessionControlType| 可取值为：`mcasConfigured`、`monitorOnly`、`blockDownloads`。 在此处了解有关这些值的更多信息： https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy- |

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

