---
title: userAccountInformation 资源类型
description: userAccountInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: cdeb6a676304fe4ec69207f9df6331d0df503b56
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519552"
---
# <a name="useraccountinformation-resource-type"></a>userAccountInformation 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表特定绑定到用户帐户的信息，无论是作为 Azure AD 帐户还是 Microsoft 帐户。 实体标识符分别设置为相应的 Azure AD guid 或 Microsoft 帐户 CID。 这些字段在 Microsoft Graph 中是只读的，并且必须通过用户配置文件或租户管理员在相应的体验上进行编辑。

继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                                             | 返回类型                                         | 说明                                                         |
|:-------------------------------------------------------------------|:----------------------------------------------------|:--------------------------------------------------------------------|
| [获取 userAccountInformation](../api/useraccountinformation-get.md) | [userAccountInformation](useraccountinformation.md) | 读取**userAccountInformation**对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性            | 类型                       | 说明                                                                                                                              |
|:--------------------|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------|
|ageGroup             |String                      | 显示用户的年龄组。 允许的`null`值`minor`、 `notAdult`和`adult`由目录生成且不能更改。|
|countryCode          |String|                     | 包含与用户帐户关联的双字符国家/地区代码。                                                                |
|preferredLanguageTag |[localeInfo](localeinfo.md) | 包含用户与帐户相关的首选语言。                                                              |
|userPrincipalName    |String                      | 与帐户关联的用户的用户主体名称（UPN）。                                                                   |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
