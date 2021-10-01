---
title: redirectUriSettings 资源类型
description: 指定 redirectUri 的索引
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 756b1e1caf92e505e62380e0ca56cc2a6f549aef
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60069345"
---
# <a name="redirecturisettings-resource-type"></a>redirectUriSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定发送用户令牌用于登录的 URL 的索引。 这仅适用于使用 SAML 的应用程序。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| uri | String | 指定令牌发送到的 URI。 |
|index|Int32|标识 SAML SSO 流中 redirectURIs 集合内的特定 URI。 默认为 `null`。 索引在应用程序的所有 redirectUri 中是唯一的。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.redirectUriSettings"
}-->

``` json
{
  "@odata.type": "#microsoft.graph.redirectUriSettings",
  "uri": "String",
  "index": "Integer"
}
```
