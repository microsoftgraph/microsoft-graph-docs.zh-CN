---
title: implicitGrantSettings 资源类型
description: '指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547013"
---
# <a name="implicitgrantsettings-resource-type"></a>implicitGrantSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 作为隐式流的一部分，单独的属性可用于请求 ID 和访问令牌。 若要启用隐式流，必须至少将下列属性之一设置为 true。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。|
|enableAccessTokenIssuance| Boolean | 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。|

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


