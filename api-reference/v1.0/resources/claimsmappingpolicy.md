---
title: claimsMappingPolicy 资源类型
description: 表示 WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议（针对颁发给特定应用程序的令牌）声明映射策略。
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 01a8fd0f25936c496846a30b6ee69b8454719325
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109323"
---
# <a name="claimsmappingpolicy-resource-type"></a>claimsMappingPolicy 资源类型

命名空间：microsoft.graph

表示 WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议（针对颁发给特定应用程序的令牌）声明映射策略。 可以使用声明映射策略：

- 选择令牌中包含的声明
- 创建不存在声明类型
- 选择或更改特定声明发出的数据源  

有关更多方案和配置详细信息，请参阅如何：自定义在令牌中为租户中的特定 [应用发出的声明](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)。

继承自 [stsPolicy](stsPolicy.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 claimsMappingPolicy](../api/claimsmappingpolicy-post-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | 创建 claimsMappingPolicy 对象。 |
| [获取 claimsMappingPolicy](../api/claimsmappingpolicy-get.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | 读取 claimsMappingPolicy 对象的属性和关系。 |
| [列出 claimsMappingPolicies](../api/claimsmappingpolicy-list.md) | [claimsMappingPolicy](claimsmappingpolicy.md) | 读取 claimsMappingPolicies 对象的属性和关系。 |
| [更新 claimsMappingPolicy](../api/claimsmappingpolicy-update.md) | 无 | 更新 claimsMappingPolicy 对象。 |
| [删除 claimsMappingPolicy](../api/claimsmappingpolicy-delete.md) | 无 | 删除 claimsMappingPolicy 对象。 |
| **目录对象** |  |  |
| [List appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | [directoryObject](directoryobject.md) 集合 | 获取已应用此策略的 directoryObjects 列表。 |
| [分配 claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md) | 无 | 将 claimsMappingPolicy 分配给 [servicePrincipal](serviceprincipal.md) 对象。 |
| [列出分配的 claimsMappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) 集合 | 列出分配给 [servicePrincipal](serviceprincipal.md) 对象的 claimsMappingPolicy 对象。 |
| [删除 claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md) | 无 | 从 [servicePrincipal](serviceprincipal.md) 对象中删除 claimsMappingPolicy。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|definition|String collection| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关 [此属性的](#properties-of-a-claims-mapping-policy-definition) JSON 架构的更多详细信息，请参阅声明映射策略定义的属性。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必需。|
|isOrganizationDefault|Boolean|忽略此属性。 声明映射策略只能应用于服务主体，并且不能为组织全局设置。|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>声明映射策略定义的属性

下面的属性构成表示声明映射策略的 JSON 对象。 此 JSON 对象必须 **转换为** 转义为要插入到定义属性中的引号 **的** 字符串。 下面显示了一些定义示例：

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>示例： **定义** 以将 EmployeeID 和 TenantCountry 作为声明包括在令牌中
<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"employeeid\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\",\"JwtClaimType\":\"name\"},{\"Source\":\"company\",\"ID\":\"tenantcountry\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/country\",\"JwtClaimType\":\"country\"}]}}"
    ],
    "displayName": "Test1234"
}
```

#### <a name="example-definition-that-uses-a-claims-transformation"></a>示例 **：** 使用声明转换的定义
<!-- {
  "blockType": "ignored"
}-->
``` json
{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\",\"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"},{\"Source\":\"user\",\"ID\":\"givenname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\"},{\"Source\":\"user\",\"ID\":\"displayname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\"},{\"Source\":\"user\",\"ID\":\"surname\",\"SamlClaimType\":\"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\"},{\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\":\"username\"}],\"ClaimsTransformation\":[{\"ID\":\"CreateTermsOfService\",\"TransformationMethod\":\"CreateStringClaim\",\"InputParameters\": [{\"ID\":\"value\",\"DataType\":\"string\", \"Value\":\"sandbox\"}],\"OutputClaims\":[{\"ClaimTypeReferenceId\":\"TOS\",\"TransformationClaimType\":\"createdClaim\"}]}]}}"
    ],
    "displayName": "Test1234"
}
```

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|版本|整数|将值设置为 1。 必需。|
|IncludeBasicClaimSet|Boolean|如果设置为 ，则基本声明集内的所有声明在受策略影响的令牌 `true` 中发出。 如果设置为 ，则基本声明集内声明不在令牌中，除非它们分别添加到同一策略的 `false` ClaimsSchema 属性中。|
|ClaimsSchema|JSON 对象|定义除了基本声明集和核心声明集之外，受策略影响的令牌中还显示哪些声明。 对于此属性中定义的每个声明架构条目，都需要某些信息。 指定数据来自 (值或源/ID 对) ，以及将数据作为声明类型 (哪个声明) 。 有关详细信息，请参阅 [ClaimsSchema definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)。|
|ClaimsTransformation|JSON 对象| 定义可应用于源数据的常见转换，以生成 ClaimsSchema 中指定的声明的输出数据。 有关详细信息，请参阅 [ClaimsTransformation definition](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation)。|


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) 集合| 已应用此策略的 [directoryObject](directoryObject.md) 集合。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": false,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "claimsMappingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
