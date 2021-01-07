---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77d1d9beeab406896bda53e88e9043be0a99e8fe
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777711"
---
# <a name="applicationserviceprincipal-resource-type"></a>applicationServicePrincipal 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加 Azure AD 应用程序库中的应用程序实例时，在目录中创建应用程序和[](../resources/application.md) [servicePrincipal](../resources/serviceprincipal.md)对象。 **applicationServicePrincipal** 表示应用程序和 **servicePrincipal** 对象的连接。 

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


