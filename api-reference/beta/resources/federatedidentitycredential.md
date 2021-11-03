---
title: federatedIdentityCredential 资源类型
description: 引用应用程序的联合身份凭据。 当从受信任的颁发者交换令牌以获取链接到在 Azure AD 上注册的应用程序的访问令牌时，这些联合身份凭据将用于工作负荷Azure AD。
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: fb5d51cd16103c21656927b999bf5484d70d0800
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697239"
---
# <a name="federatedidentitycredential-resource-type"></a>federatedIdentityCredential 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

引用应用程序的联合身份凭据。 当从受信任的颁发者交换令牌以获取[](/azure/active-directory/develop/workload-identity-federation)链接到在 Azure AD 上注册的应用程序的访问令牌时，这些联合身份凭据将用于工作负荷Azure AD。

继承自 [实体](../resources/entity.md)。

>**注意：** 此资源不适用于国家 [云](/graph/deployments) 部署。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md) 集合|获取 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象及其属性的列表。|
|[创建 federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|创建新的 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。|
|[获取 federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|读取 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象的属性和关系。|
|[更新 federatedIdentityCredential](../api/federatedidentitycredential-update.md)|无|更新 [federatedIdentityCredential 对象](../resources/federatedidentitycredential.md) 的属性。|
|[删除 federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|无|删除 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| 访问群体 | String collection | 列出可在外部令牌中显示访问群体。 此字段是必需的，默认为"api://AzureADTokenExchange"。 它指出Microsoft 标识平台 `aud` 令牌中的声明应接受哪些信息。 此值表示Azure AD标识提供程序中的令牌，并且固定值标识提供程序之间没有任何关系 - 可能需要在标识提供程序中创建新的应用程序注册，以用作此令牌的受众。 必需。 |
| description | String | 未经验证的联合身份凭据的用户提供的说明。 可选。  |
| id| String | 联合标识的唯一标识符。 必需。 只读。  |
| issuer | 字符串 | 外部标识提供程序的 URL，并且必须与要交换 `issuer` 的外部令牌声明匹配。 颁发者和主题的值组合在应用中必须是唯一的。 必需。 |
| name | String | 是联合标识凭据的唯一标识符，该凭据的字符限制为 120 个字符，并且必须为 URL 友好。 创建后不可变。 必填。 不可为空。 支持 `$filter`（`eq`）。 |
| subject | String | 必需。 外部标识提供程序中的外部软件工作负荷的标识符。 与访问群体值一样，它没有固定格式，因为每个标识提供程序都使用其自己的格式，有时是 GUID，有时是冒号分隔的标识符，有时是任意字符串。 此处的值必须与 `sub` 向用户呈现的令牌中的声明Azure AD。 颁发者和 **主题****的组合在** 应用中必须是唯一的。 支持 `$filter`（`eq`）。 |


## <a name="relationships"></a>关系

无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.federatedIdentityCredential",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```

