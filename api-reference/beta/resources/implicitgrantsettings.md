---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中, 可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流, 下列属性中必须至少有一个设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92ba18488cc2700b565be47bac3874b6d75e1c13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005791"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中, 可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流, 下列属性中必须至少有一个设置为 true。

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
