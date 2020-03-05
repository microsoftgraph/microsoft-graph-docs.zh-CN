---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9a7cc33e05c28e5552815778e86e5b1b9e7aaf06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508280"
---
# <a name="applicationserviceprincipal-resource-type"></a>applicationServicePrincipal 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当添加了 Azure AD 应用程序库中的应用程序实例时，将在目录中创建[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。 **ApplicationServicePrincipal**表示**应用程序**和**servicePrincipal**对象的串联。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

| 属性 | 类型        | 说明 |
|:-------------|:------------|:------------|
|application|[application](../resources/application.md)|表示在 Azure Active Directory 中注册的应用程序。|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|表示目录中的一个应用程序实例。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
