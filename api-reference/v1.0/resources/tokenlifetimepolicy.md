---
title: tokenLifetimePolicy 资源类型
description: 表示一个策略，该策略可以控制由用户颁发的访问Azure Active Directory。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1d35f0befc6e61aafb515e19cbc777029f627989078b003d12728e034d668896
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189154"
---
# <a name="tokenlifetimepolicy-resource-type"></a>tokenLifetimePolicy 资源类型

命名空间：microsoft.graph



表示可以控制 JWT 访问令牌、ID 令牌或由 Azure AD Azure Active Directory (颁发的 SAML 1.1/2.0) 。 可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。 

>**注意：** 不支持为刷新令牌和会话令牌配置此策略。

继承自 [stsPolicy](stsPolicy.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 tokenLifetimePolicies](../api/tokenlifetimepolicy-list.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 读取 tokenLifetimePolicies 对象的属性和关系。 |
| [创建 tokenLifetimePolicy](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 创建 tokenLifetimePolicy 对象。 |
| [获取 tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md) | [tokenLifetimePolicy](tokenlifetimepolicy.md) | 读取 tokenLifetimePolicy 对象的属性和关系。 |
| [更新 tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md) | 无 | 更新 tokenLifetimePolicy 对象。 |
| [删除 tokenLifetimePolicy](../api/tokenlifetimepolicy-delete.md) | 无 | 删除 tokenLifetimePolicy 对象。 |
| [List appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | [directoryObject](directoryobject.md) collection | 获取已应用此策略的 directoryObjects 列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。|
|definition|String collection| 包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。 有关此属性的 JSON 架构的更多详细信息，请参阅下文。 必需。|
|description|String| 此策略的说明。|
|displayName|String| 此策略的显示名称。 必填。|
|isOrganizationDefault|Boolean|如果设置为 `true` ，则激活此策略。 同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。 可选，默认值为 `false` 。|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>令牌生存期策略定义的属性
下面的属性构成表示令牌生存期策略的 JSON 对象。 此 JSON 对象必须 **转换为** 转义为要插入到定义属性中的引号 **的** 字符串。 下面以 JSON 格式显示了一个示例：

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>**注意：** 这些属性的所有持续时间均以"dd.hh：mm：ss"格式指定。

>**注意：** 用"天"表示的属性的最大值比指定天数短 1 秒。 例如，最大值 1 天指定为"23：59：59"。

| 属性     | 类型   |说明| 最小值 | 最大值 | 默认值|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|控制访问令牌和 ID 令牌都被视为有效的时间。|10 分钟|1 天|1 小时|
|版本|整数|将值设置为 1。 必填。|无|无|无|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) collection| 已应用此策略的 [directoryObject](directoryObject.md) 集合。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
