---
title: federatedIdentityCredential 资源类型
description: 引用应用程序的联合标识凭据。 从受信任的颁发者交换令牌以获取链接到在 Azure AD 上注册的应用程序的访问令牌时，这些联合标识凭据用于工作负荷标识联合。
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 4a529d1079c3058a1cb381e8b46c7849d8d4f3dd
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602740"
---
# <a name="federatedidentitycredential-resource-type"></a>federatedIdentityCredential 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

引用应用程序的联合标识凭据。 从受信任的颁发者交换令牌以获取链接到在 Azure AD 上注册的应用程序的访问令牌时，这些联合标识凭据用于 [工作负荷标识联合](/azure/active-directory/develop/workload-identity-federation) 。

继承自 [entity](../resources/entity.md)。

>**注意：** 此资源在 [国家云](/graph/deployments) 部署中不可用。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md) 集合|获取 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象及其属性的列表。|
|[Create federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|创建新的 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。|
|[Get federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|读取 [federatedIdentityCredential 对象的](../resources/federatedidentitycredential.md) 属性和关系。|
|[Update federatedIdentityCredential](../api/federatedidentitycredential-update.md)|无|更新 [federatedIdentityCredential 对象的](../resources/federatedidentitycredential.md) 属性。|
|[Delete federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|无|删除 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| 观众 | 字符串集合 | 列出可以在外部令牌中显示的受众。 此字段是必需的，默认为“api://AzureADTokenExchange”。 它说明了Microsoft 标识平台应该接受`aud`传入令牌中的声明。 此值表示外部标识提供程序中的 Azure AD，并且在标识提供者之间没有固定值 - 可能需要在标识提供者中创建新的应用程序注册，以充当此令牌的受众。 必需。 |
| description | String | 联合标识凭据的未经验证的用户提供的说明。 可选。  |
| id| String | 联合标识的唯一标识符。 必需项。 只读。  |
| 发行 | String | 外部标识提供者的 URL，必须与要交换的外部令牌的声明匹配 `issuer` 。 **颁发者** 和 **主题** 的值的组合在应用中必须是唯一的。 必需项。 |
| name | 字符串 | 是联合标识凭据的唯一标识符，其字符限制为 120 个字符，必须对 URL 友好。 创建后，它是不可变的。 必填。 不可为空。 支持 `$filter`（`eq`）。 |
| subject | String | 必需。 外部标识提供程序中外部软件工作负荷的标识符。 与受众值一样，它没有固定格式，因为每个标识提供者都使用自己的标识提供者 - 有时是 GUID，有时是冒号分隔标识符，有时是任意字符串。 此处的 `sub` 值必须与显示给 Azure AD 的令牌内的声明匹配。 **颁发者** 和 **主题** 的组合在应用中必须是唯一的。 支持 `$filter`（`eq`）。 |


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

