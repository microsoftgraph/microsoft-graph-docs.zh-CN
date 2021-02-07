---
title: implicitGrantSettings 资源类型
description: 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 单独的属性可用于请求 ID 和访问令牌作为隐式流的一部分。 若要启用隐式流，必须至少将以下属性之一设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133278"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

命名空间：microsoft.graph

指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 单独的属性可用于请求 ID 和访问令牌作为隐式流的一部分。 若要启用隐式流，必须至少将以下属性之一设置为 true。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| 布尔 | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。|
|enableAccessTokenIssuance| 布尔 | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。|

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

