---
title: tokenIssuancePolicy 资源类型
description: 表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a135376fef5d5a422a22bd862cffa8ef4f3ff9a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442797"
---
# <a name="tokenissuancepolicy-resource-type"></a>tokenIssuancePolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。 可以使用令牌颁发策略：

- 设置签名选项
- 设置签名算法
- 设置 SAML 令牌版本

继承自 [stsPolicy](stsPolicy.md)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 tokenIssuancePolicy](../api/tokenissuancepolicy-post-tokenissuancepolicy.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 创建 tokenIssuancePolicy 对象。 |
| [获取 tokenIssuancePolicy](../api/tokenissuancepolicy-get.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 读取 tokenIssuancePolicy 对象的属性和关系。 |
| [列出 tokenIssuancePolicy](../api/tokenissuancepolicy-list.md) | [tokenIssuancePolicy](tokenissuancepolicy.md) | 读取 tokenIssuancePolicy 对象的属性和关系。 |
| [更新 tokenIssuancePolicy](../api/tokenissuancepolicy-update.md) | 无 | 更新 tokenIssuancePolicy 对象。 |
| [删除 tokenIssuancePolicy](../api/tokenissuancepolicy-delete.md) | 无 | 删除 tokenIssuancePolicy 对象。 |
| [List appliesTo](../api/tokenissuancepolicy-list-appliesto.md) | [directoryObject](directoryobject.md) 集合 | 获取已应用此策略的 directoryObjects 列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|definition|字符串集合| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅下文。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必需。|
|isOrganizationDefault|布尔|忽略此属性。 令牌颁发策略只能应用于服务主体，并且不能为组织全局设置。|


### <a name="properties-of-a-token-issuance-policy-definition"></a>令牌颁发策略定义的属性
这些属性形成表示令牌颁发策略的 JSON 对象。 此 JSON 对象 **必须转换为带** 转义引号的字符串，以插入到 **定义** 属性中。 下面是 JSON 格式的示例：

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{ \"TokenIssuancePolicy\":{\"TokenResponseSigningPolicy\":\"TokenOnly\",\"SamlTokenVersion\":\"1.1\",\"SigningAlgorithm\":\"http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\",\"Version\":1}}"
  ]
```


| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|TokenResponseSigningPolicy|String|表示 Azure AD 中可用的证书签名选项。 支持的值是： `ResponseOnly` ， `TokenOnly` `ResponseAndToken` 。  |
|SamlTokenVersion|String|SAML 令牌的版本。 支持的值是： `1.1` `2.0` 。 |
|SigningAlgorithm|String|Azure AD 使用签名算法对 SAML 令牌进行签名。 支持的值是： `http://www.w3.org/2001/04/xmldsig-more#rsa-sha256` `http://www.w3.org/2000/09/xmldsig#rsa-sha1` 。|
|版本|整数|设置值 1。 必填。|


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


