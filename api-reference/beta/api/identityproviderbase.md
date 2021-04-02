---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 71c6d58e9ad70773df39adc7d2a91393d64cd460
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491059"
---
# <a name="identityproviderbase-resource-type"></a>identityProviderBase 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|identityProviderBase 集合|检索在租户中配置的所有标识提供程序。|
|[列出可用的提供程序类型](../api/identityproviderbase-list-availableprovidertypes.md)|String 集合|检索所有可用的身份提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|字符串|标识提供程序的 ID。|
|displayName|字符串|标识提供程序的显示名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
