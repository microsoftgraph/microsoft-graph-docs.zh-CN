---
title: claimsMappingPolicy 资源类型
description: 表示一个策略，该策略可以控制Azure Active Directory (Azure AD) 颁发的访问令牌的生存期。
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f25d4f252c3bda6331a982f26b82cf4764a4ec7c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314609"
---
# <a name="claimsmappingpolicy-resource-type"></a>claimsMappingPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 WS-Fed、SAML、OAuth 2.0 和 OpenID 连接协议的声明映射策略，用于颁发给特定应用程序的令牌。 可以使用声明映射策略执行以下操作：

- 选择令牌中包含的声明
- 创建尚不存在的声明类型
- 选择或更改在特定声明中发出的数据源

可添加到声明映射策略的声明和转换数目限制为减少令牌大小。 达到限制后遇到的任何声明架构条目或转换将被忽略，并包含在颁发的令牌中。 有关限制的详细信息，请参阅 [声明映射策略定义的属性](#properties-of-a-claims-mapping-policy-definition)

有关更多方案和配置详细信息，请参阅 [声明映射策略类型](/azure/active-directory/develop/reference-claims-mapping-policy-type) 和 [操作方法：自定义租户中特定应用的令牌中发出的声明](/azure/active-directory/develop/active-directory-claims-mapping#claims-mapping-policy-properties)。

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
| [List appliesTo](../api/claimsmappingpolicy-list-appliesto.md) | [directoryObject](directoryobject.md) collection | 获取已应用此策略的 directoryObjects 的列表。 |
| [分配 claimsMappingPolicy](../api/serviceprincipal-post-claimsmappingpolicies.md) | 无 | 将 claimsMappingPolicy 分配给 [servicePrincipal](serviceprincipal.md) 对象。 |
| [列出分配的声明MappingPolicy](../api/serviceprincipal-list-claimsmappingpolicies.md) | [claimsMappingPolicy](claimsmappingpolicy.md) 集合 | 列出分配给 [servicePrincipal](serviceprincipal.md) 对象的 claimsMappingPolicy 对象。 |
| [删除 claimsMappingPolicy](../api/serviceprincipal-delete-claimsmappingpolicies.md) | 无 | 从 [servicePrincipal](serviceprincipal.md) 对象中删除 claimsMappingPolicy。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|定义|String collection| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅以下内容。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必填。|
|isOrganizationDefault|Boolean|忽略此属性。 声明映射策略只能应用于服务主体，不能为组织全局设置。|

### <a name="properties-of-a-claims-mapping-policy-definition"></a>声明映射策略定义的属性

下面的属性构成表示声明映射策略的 JSON 对象。 必须将此 JSON 对象 **转换为具有转义引号的字符串** ，才能插入到 **定义** 属性中。 下面显示了几个定义示例：

#### <a name="example-definition-to-include-the-employeeid-and-tenantcountry-as-claims-in-tokens"></a>示例：将 EmployeeID 和 TenantCountry 作为声明包含在令牌中的 **定义**

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

#### <a name="example-definition-that-uses-a-claims-transformation"></a>示例：使用声明转换的 **定义**

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
|版本|整数|设置值 1。 必填。|
|IncludeBasicClaimSet|Boolean|如果设置为 `true`，基本声明集中的所有声明都会在受策略影响的令牌中发出。 如果设置为 `false`，基本声明集中的声明不在令牌中，除非它们单独添加到同一策略的 ClaimsSchema 属性中。|
|ClaimsSchema|JSON 对象|定义受策略影响的令牌中存在哪些声明，以及基本声明集和核心声明集。 对于此属性中定义的每个声明架构条目，需要某些信息。 指定数据来自 (值或源/ID 配对) 的位置，以及将数据作为声明类型) 发出 (声明。 令牌中最多包含 50 个通过 ClaimsSchema 对象的声明。 达到限制后遇到的任何声明架构条目都将被忽略，并且不会显示在颁发的令牌中。 [ClaimsSchema 定义](/azure/active-directory/develop/active-directory-claims-mapping#claims-schema)中提供了更多详细信息。|
|ClaimsTransformation|JSON 对象| 定义可应用于源数据的常见转换，为 ClaimsSchema 中指定的声明生成输出数据。 通过 ClaimsTransformation 对象，令牌中最多包含 50 个转换。 达到限制后遇到的任何转换都将被忽略，并且不会显示在颁发的令牌中。 有关 ClaimsTransformation 和支持的函数的详细信息，请参阅 [声明转换](/azure/active-directory/develop/active-directory-claims-mapping#claims-transformation)。|


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) collection| 已应用此策略 [的 directoryObject](directoryObject.md) 集合。 只读。|

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
