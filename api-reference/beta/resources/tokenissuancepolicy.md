---
title: tokenIssuancePolicy 资源类型
description: 表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。
ms.localizationpriority: medium
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 257e2b98ffd2e63093b2c5f53b96f9565c13712f
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66767945"
---
# <a name="tokenissuancepolicy-resource-type"></a>tokenIssuancePolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。 可以使用令牌颁发策略执行以下操作：

- 设置签名选项
- 设置签名算法
- 设置 SAML 令牌版本

继承自 [stsPolicy](stsPolicy.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 创建 tokenIssuancePolicy 对象。 |
| [获取 tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 读取 tokenIssuancePolicy 对象的属性和关系。 |
| [列出 tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 读取 tokenIssuancePolicy 对象的属性和关系。 |
| [更新 tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | 无 | 更新 tokenIssuancePolicy 对象。 |
| [删除 tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | 无 | 删除 tokenIssuancePolicy 对象。 |
| [List appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | [directoryObject](directoryobject.md) 集合 | 获取已应用此策略的 directoryObjects 的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|定义|String collection| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅以下内容。 必需。|
|description|字符串| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必需。|
|isOrganizationDefault|布尔值|忽略此属性。 令牌颁发策略只能应用于服务主体，不能为组织全局设置。|


### <a name="properties-of-a-token-issuance-policy-definition"></a>令牌颁发策略定义的属性
这些属性构成表示令牌颁发策略的 JSON 对象。 必须将此 JSON 对象 **转换为具有转义引号的字符串** ，才能插入到 **定义** 属性中。 下面是 JSON 格式的示例：

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":\"1\",\"EmitSAMLNameFormat\": \"true\"}}"
  ]
```


| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|字符串|表示 Azure AD 中可用的证书签名选项。 支持的值为： `ResponseOnly`， ， `ResponseAndToken``TokenOnly`.  |
|SamlTokenVersion|String|SAML 令牌的版本。 支持的值为： `1.1`. `2.0` |
|SigningAlgorithm|字符串|Azure AD 使用签名算法对 SAML 令牌进行签名。 支持的值为： `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256`. `http://www.w3.org/2000/09/xmldsig#rsa-sha1`|
|版本|整数|设置值 1。 必需。|
| EmitSamlNameFormat | 布尔值 | 如果选中，Azure Active Directory 将添加一个名为“NameFormat”的其他属性，该属性描述此应用程序的受限、核心和可选声明的名称格式。 [了解详细信息](/azure/active-directory/develop/reference-claims-mapping-policy-type#claim-sets) | 

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) 集合| 已应用此策略 [的 directoryObject](directoryObject.md) 集合。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenIssuancePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


