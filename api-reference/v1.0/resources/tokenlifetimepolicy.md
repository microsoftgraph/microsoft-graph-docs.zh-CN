---
title: tokenLifetimePolicy 资源类型
description: 表示一个可控制 Azure Active Directory 颁发的访问令牌的生存期的策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 568d8244170ade5c2e6a9faebcd910d0470635ef
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229638"
---
# <a name="tokenlifetimepolicy-resource-type"></a>tokenLifetimePolicy 资源类型

命名空间：microsoft.graph



表示一个策略，该策略可以控制 JWT 访问令牌的有效期、由 Azure Active Directory （Azure AD）颁发的 ID 令牌或 SAML 1.1/2.0 令牌。 您可以为组织中的所有应用、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。  有关更多方案的详细信息，请参阅[Azure Active Directory 中的可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

>**注意：** 不支持为刷新令牌和会话令牌配置此策略。

继承自[stsPolicy](stsPolicy.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 tokenLifetimePolicies](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 读取 tokenLifetimePolicies 对象的属性和关系。 |
| [创建 tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 创建 tokenLifetimePolicy 对象。 |
| [获取 tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 读取 tokenLifetimePolicy 对象的属性和关系。 |
| [更新 tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | 无 | 更新 tokenLifetimePolicy 对象。 |
| [删除 tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | 无 | 删除 tokenLifetimePolicy 对象。 |
| [列出 appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | [directoryObject](directoryobject.md) 集合 | 获取已应用此策略的 directoryObjects 的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|字符串| 此策略的唯一标识符。 只读。|
|定义|String 集合| 一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅下文。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必需。|
|isOrganizationDefault|布尔|如果设置为 true，则激活此策略。 对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。 可选，默认值为 false。|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>令牌生存期策略定义的属性
下面的属性构成了表示令牌生存期策略的 JSON 对象。 此 JSON 对象必须**转换为转义了引号的字符串**，以将其插入到**定义**属性中。 下面以 JSON 格式显示了一个示例：

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>**注意：** 这些属性中的所有持续时间均以 "dd. hh： mm： ss" 的格式指定。

>**注意：**"天" 中表示的属性的最大值是表示的天数的1秒。 例如，"最大值为1天" 指定为 "23:59:59"。

| 属性     | 类型   |说明| 最小值 | 最大值 | 默认值|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|控制访问和 ID 令牌被视为有效的时间。|10 分钟|1 天|1 小时|
|版本|整数|将值设置为1。 必需。|无|无|无|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) 集合| 已将此策略应用于的[directoryObject](directoryObject.md)集合。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "baseType": "",
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
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
