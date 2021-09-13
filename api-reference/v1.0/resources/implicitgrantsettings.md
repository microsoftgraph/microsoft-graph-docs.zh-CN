---
title: implicitGrantSettings 资源类型
description: 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 作为隐式流的一部分，单独的属性可用于请求 ID 和访问令牌。 若要启用隐式流，必须至少将下列属性之一设置为 true。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 2ccf78ded6c9fa482f5054e2734d369acf041b18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118605"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

命名空间：microsoft.graph

指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 作为隐式流的一部分，单独的属性可用于请求 ID 和访问令牌。 若要启用隐式流，必须至少将下列属性之一设置为 true。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| 布尔值 | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。|
|enableAccessTokenIssuance| 布尔值 | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。|

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

