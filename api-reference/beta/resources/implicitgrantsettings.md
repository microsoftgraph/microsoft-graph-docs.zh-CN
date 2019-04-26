---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中, 可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流, 下列属性中必须至少有一个设置为 true。
localization_priority: Normal
ms.openlocfilehash: 1026f3b97a3305dff7a715fae000ab9695ac8e9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333608"
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
