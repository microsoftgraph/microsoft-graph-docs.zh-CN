---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流，下列属性中必须至少有一个设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e2d15c7468442c8ad3adbddddd843ee12a7249ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531330"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

命名空间：microsoft.graph

指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流，下列属性中必须至少有一个设置为 true。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。|
|enableAccessTokenIssuance| Boolean | 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
