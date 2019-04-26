---
title: 策略资源类型
description: '表示 Azure AD 策略。 策略是可在应用程序、服务主体、组或其分配到的整个组织中强制实施的自定义规则。 目前, 只有一种类型的策略是可用的:'
localization_priority: Normal
ms.openlocfilehash: 118bac238d58734b5cbdeb1a4f346aedf680de6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563625"
---
# <a name="policy-resource-type"></a>策略资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 策略。 策略是可在应用程序、服务主体、组或其分配到的整个组织中强制实施的自定义规则。 目前, 只有一种类型的策略是可用的:

- 令牌生存期策略-指定为应用程序和服务主体颁发的令牌的生存期持续时间。

下面将进一步详细介绍此策略。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
| [获取策略](../api/policy-get.md) |策略|读取 user 对象的属性和关系。|
|[创建策略](../api/policy-post.md)|策略|创建新的策略对象。|
|[更新策略](../api/policy-update.md)|无|更新 policy 对象。|
|[删除策略](../api/policy-delete.md)|无|删除 policy 对象。|
|[分配策略](../api/policy-assign.md)|无|将策略分配给应用程序和服务主体。|
|[列出策略](../api/policy-list.md)|策略集合|获取组织中的所有 policy 对象。|
|[列出已分配策略](../api/policy-list-assigned.md)|策略集合|获取分配给应用程序或服务主体的所有策略对象。|

### <a name="common-properties"></a>常用属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|定义|String|特定策略的字符串版本。 请参阅下文。 必需。|
|displayName|String|策略的自定义名称。 必需。|
|IsOrganizationDefault|Boolean|如果设置为 true, 则激活此策略。 对于同一策略类型, 可以有多个策略, 但只有一个策略可以作为组织默认激活。 可选, 默认值为 false。|
|type|String|指定策略的类型。 当前必须是 "TokenLifetimePolicy"。 必需。|

#### <a name="common-relationships"></a>共同关系
|关系|类型|说明|
|:-------------|:-----------|:-----------|
|appliesTo|[directoryObject](../resources/directoryobject.md) 集合|策略应用于的应用程序、服务主体、组或组织。|

## <a name="token-lifetime-policy"></a>令牌生存期策略
指定出于不同目的而颁发的令牌的生存期。 此类策略可[分配](../api/policy-assign.md)给应用程序和服务主体。 有四种令牌可以配置其生存期。 在通过客户端进行身份验证期间获取访问/刷新令牌对, 而在通过浏览器进行身份验证期间获取 ID/会话令牌对。

- **访问令牌**包含与客户端用来访问受保护的资源 (如应用程序) 所使用的用户帐户相关联的标识和权限的相关信息。
- 当用户通过客户端对 Azure AD 进行身份验证以访问受保护的资源时, 将与访问令牌一起获取**刷新令牌**。 如果未将其废除或保留不使用的 MaxInactiveTime (以下), 则可以使用它在当前访问令牌过期时获取新的访问/刷新令牌对。
- **ID 令牌**的行为与访问令牌类似, 但通过浏览器获取。
- **会话令牌**的行为类似于刷新令牌, 但通过浏览器获取。

## <a name="properties"></a>属性
下面的属性构成了表示令牌生存期策略的 JSON 对象。 此 JSON 对象必须**转换为转义了引号的字符串**, 以插入到 "定义" 常见策略属性中。 下面是一个示例。

>注意: 这些属性中的所有持续时间均以 "dd. hh: mm: ss" 的格式指定。

>注意: "天" 中表示的属性的最大值是表示的天数的1秒。 例如, "最大值为1天" 指定为 "23:59:59"。

| 属性     | 类型   |说明| 最小值 | 最大值 | 默认值|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|控制**访问和 ID 令牌**被视为有效的时间。|10 分钟|1 天|1 hour|
|MaxInactiveTime|String|控制刷新令牌可以在客户端无法再使用它检索访问资源的新访问/刷新令牌对之前的等待时间。|10 分钟|90 天|14 天|
|MaxAgeSingleFactor|String|控制用户在最后一次通过仅一个因素进行身份验证后, 可以继续使用刷新令牌获取新的访问/刷新令牌对的时间。 由于单一因子的安全性低于多重身份验证, 因此建议将此策略设置为等于或小于 MultiFactorRefreshTokenMaxAge 的值。|10 分钟|截止-已吊销|365天或截止-已撤销|
|MaxAgeMultiFactor|String|控制用户在最后一次使用多个因素进行身份验证后, 可以继续使用刷新令牌获取新的访问/刷新令牌对的时间。|10 分钟|截止-已吊销|365天或截止-已撤销|
|MaxAgeSessionSingleFactor|String|控制用户在最后一次通过仅单个因素进行身份验证后, 可以继续使用会话令牌获取新 ID/会话令牌的时间。 由于单一因子的安全性低于多重身份验证, 因此建议将此策略设置为一个等于或小于 MultiFactorSessionTokenMaxAge 的值。|10 分钟|截止-已吊销|365或直到被吊销|
|MaxAgeSessionMultiFactor|String|控制用户在最后一次成功地使用多个因素进行身份验证后, 可以继续使用会话令牌获取新 ID/会话令牌的时间。|10 分钟|截止-已吊销|365或直到被吊销|
|Version|Integer|将值设置为1。 必需。|无|无|无|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
  "displayName":"Test Policy",
  "isOrganizationDefault":false,
  "type":"TokenLifetimePolicy",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/policy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
