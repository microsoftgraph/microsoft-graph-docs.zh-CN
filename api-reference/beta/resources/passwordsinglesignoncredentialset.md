---
title: passwordSingleSignOnCredentialSet 资源类型
description: 指示将用户或组的登录流完全定义为应用程序的一组凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6293c6a2fbdffd124a8e011bd00a22c30efa77e5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658791"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>passwordSingleSignOnCredentialSet 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示将用户或组的登录流完全定义为应用程序的一组凭据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|凭据|[凭据](credential.md)集合|定义完整的登录流的 credential 对象的列表。|
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
