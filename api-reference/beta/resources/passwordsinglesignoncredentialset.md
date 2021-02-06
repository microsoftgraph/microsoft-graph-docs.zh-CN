---
title: passwordSingleSignOnCredentialSet 资源类型
description: 指示完全定义用户或组到应用程序的登录流的凭据集。
localization_priority: Normal
author: bharathramh92
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 95526942bcedfc20d983a8873699af6902482b2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130874"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>passwordSingleSignOnCredentialSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示完全定义用户或组到应用程序的登录流的凭据集。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|credentials|[credential](credential.md) 集合|定义完整登录流的凭据对象列表。|
|id|字符串|此凭据集所属的用户或组的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


