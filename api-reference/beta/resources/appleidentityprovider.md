---
title: appleManagedIdentityProvider 资源类型
description: 在 Azure AD B2C 租户中表示 Apple 标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491097"
---
# <a name="applemanagedidentityprovider-resource-type"></a>appleManagedIdentityProvider 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以将 Apple 配置为 Azure AD B2C 租户的社交标识提供程序。 根据 Apple 提供的信息，API 将生成客户端密码。 Apple 需要每六个月更新一次秘诀。 必须囘圼旋转編密編。

此类型将从 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|identityProviderBase 集合|检索租户中配置的所有标识提供程序，包括 Apple 标识提供程序。|
|[Create](../api/identityproviderbase-post-identityproviders.md)|appleManagedIdentityProvider |创建新的 Apple 标识提供程序配置。|
|[Get](../api/identityproviderbase-get.md) |appleManagedIdentityProvider |检索 Apple 标识提供程序配置的属性。|
|[更新](../api/identityproviderbase-update.md)|无|更新 Apple 标识提供程序配置。|
|[删除](../api/identityproviderbase-delete.md)|无|删除 Apple 标识提供程序配置。|
|[列出可用的提供程序类型](../api/identityproviderbase-list-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|developerId|String|Apple 开发人员标识符。 必填。|
|服务 Id|String|Apple 服务标识符。 必填。|
|keyId|String|Apple 密钥标识符。 必填。|
|certificateData|String|证书中长文本字符串的证书数据可能是 null。|
|id|String|标识提供程序的标识符。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。 只读。|
|displayName|字符串|标识提供程序的显示名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|

你可以从 Apple 开发人员门户找到 developerId、serviceId、keyId 和 certificateData。 有关更多详细信息，你可以按照指南创建 [Apple ID 应用程序](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)

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
