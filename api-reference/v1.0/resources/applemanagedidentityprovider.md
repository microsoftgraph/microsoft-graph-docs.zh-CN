---
title: appleManagedIdentityProvider 资源类型
description: 表示 B2C 租户Azure AD Apple 标识提供程序。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ce307ea651515482c6c82baa91c8fe4dcd598219
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891242"
---
# <a name="applemanagedidentityprovider-resource-type"></a>appleManagedIdentityProvider 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 B2C 租户Azure AD Apple 标识提供程序。

可以将 Apple 配置为 Azure AD B2C 租户的社交标识提供程序。 根据 Apple 提供的信息，API 将生成客户端密码。 Apple 需要每六个月更新一次秘诀。 必须手动轮换机密。

继承自 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索在租户中配置的所有标识提供程序，包括 Apple 标识提供程序。 无法仅检索租户中的 Apple 标识提供者。|
|[Create](../api/identitycontainer-post-identityproviders.md)|[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |创建新的 Apple 标识提供程序配置。|
|[Get](../api/identityproviderbase-get.md) |[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |检索 Apple 标识提供程序配置的属性。|
|[更新](../api/identityproviderbase-update.md)|无|更新 Apple 标识提供程序配置。|
|[删除](../api/identityproviderbase-delete.md)|无|删除 Apple 标识提供程序配置。|
|[列出可用的提供程序类型](../api/identityproviderbase-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|描述|
|:---------------|:--------|:----------|
|certificateData|String|证书数据，它是证书中的长字符串文本。 可以是 null。|
|developerId|String|Apple 开发人员标识符。必填。|
|displayName|字符串|标识提供者的显示名称。继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|id|String|标识提供程序的标识符。继承自 [identityProviderBase](../resources/identityproviderbase.md)。只读。|
|keyId|String|Apple 密钥标识符。必填。|
|服务 Id|String|Apple 服务标识符。必填。|

从 Apple 开发人员门户检索 **developerId**、 **serviceId**、 **keyId** 和 **certificateData** 。 有关详细信息，请按照指南[创建 Apple ID 应用程序](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
