---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 35abee6b3028111ce4237828b58492a546ff5d4b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476424"
---
# <a name="applicationserviceprincipal-resource-type"></a>applicationServicePrincipal 资源类型

命名空间：microsoft.graph

添加 Azure AD 应用程序库中的应用程序实例时，在目录中创建应用程序和[](../resources/application.md) [servicePrincipal](../resources/serviceprincipal.md)对象。 **applicationServicePrincipal** 表示应用程序和 **servicePrincipal** 对象的连接。 

## <a name="methods"></a>Methods

无

## <a name="properties"></a>属性

| 属性         | 类型                                                 | 说明                                                     |
| :--------------- | :--------------------------------------------------- | :-------------------------------------------------------------- |
| application      | [application](../resources/application.md)           | 表示在 Azure Active Directory 中注册的应用程序。 |
| servicePrincipal | [servicePrincipal](../resources/serviceprincipal.md) | 表示目录中的一个应用程序实例。        |

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
  "servicePrincipal": { "@odata.type": "microsoft.graph.servicePrincipal" },
  "application": { "@odata.type": "microsoft.graph.application" }
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
