---
title: appleManagedIdentityProvider 资源类型
description: 在 Azure AD B2C 租户中表示 Apple 标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: fe342e88e8651f61c6e9d29bf33611829756d28a
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667825"
---
# <a name="applemanagedidentityprovider-resource-type"></a>appleManagedIdentityProvider 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以将 Apple 配置为 Azure AD B2C 租户的社交标识提供程序。 根据 Apple 提供的信息，API 将生成客户端密码。 Apple 需要每六个月更新一次秘诀。 必须手动轮换机密。

继承自 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索租户中配置的所有标识提供程序，包括 Apple 标识提供程序。 无法仅检索租户中的 Apple 标识提供者。|
|[Create](../api/identitycontainer-post-identityproviders.md)|[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |创建新的 Apple 标识提供程序配置。|
|[Get](../api/identityproviderbase-get.md) |[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |检索 Apple 标识提供程序配置的属性。|
|[更新](../api/identityproviderbase-update.md)|无|更新 Apple 标识提供程序配置。|
|[删除](../api/identityproviderbase-delete.md)|无|删除 Apple 标识提供程序配置。|
|[列出可用的提供程序类型](../api/identityproviderbase-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|developerId|String|Apple 开发人员标识符。必填。|
|服务 Id|String|Apple 服务标识符。必填。|
|keyId|String|Apple 密钥标识符。必填。|
|certificateData|String|证书中长文本字符串的证书数据可能是 null。|
|id|String|标识提供程序的标识符。继承自 [identityProviderBase](../resources/identityproviderbase.md)。只读。|
|displayName|字符串|标识提供者的显示名称。继承自 [identityProviderBase](../resources/identityproviderbase.md)。|

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
